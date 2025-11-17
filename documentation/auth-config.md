---
title: 'Autenticación'
description: 'Configuración y ejemplos de autenticación para la API de Checkout.'
slug: 'configuracion-autenticacion'
order: 2
---
# **Autenticación**

Conoce el protocolo de autenticación de Checkout API y cómo generar tu autenticación.

Para interactuar con la API de Checkout debes autenticar tus peticiones. De esta forma identificamos y validamos la información para que tus operaciones sean seguras. La API utiliza *Web Services Security UsernameToken Profile 1.1*.

---

## Credenciales API

Para integrarse con Checkout debes contar con tus credenciales `login` y `secretKey`.

- **login:** Identificador del sitio. Puede considerarse público, pues viaja como dato plano en las peticiones API.
- **secretKey:** Llave secreta del sitio, debe ser privada. A partir de este dato se generará un nuevo `tranKey` que será enviado en las peticiones.

> Estas credenciales son propias de tu sitio y deben ser tratadas de forma segura. No compartas tus credenciales en áreas de acceso público como GitHub, código del lado cliente u otros lugares de fácil acceso para terceros.

---

## Objeto Authentication

El parámetro `auth` debe ser enviado en todas las peticiones API y contiene el grupo de propiedades necesarias para verificar la autenticación.

**Propiedades:**
- `auth.login` (string): Identificador del sitio
- `auth.tranKey` (string): Credencial tranKey generado (ver explicación siguiente)
- `auth.nonce` (string): Valor aleatorio para cada solicitud, codificado en Base64.
- `auth.seed` (string): Fecha actual, generada en formato ISO 8601.

**Ejemplo de autenticación:**

```json
{
  "auth": {
    "login": "aabbccdd1234567890aabbccdd123456",
    "tranKey": "ABC123example456trankey+789abc012def3456ABC=",
    "nonce": "enQ4dXh3YWhkMWM=",
    "seed": "2023-06-21T09:56:06-05:00"
  }
  // ...
}
```

---

## Cómo generar tu autenticación

Debes conocer y preparar los siguientes datos:

- **login:** Credencial `login` provista al iniciar tu integración. Identificador del sitio.
- **secretKey:** Credencial `secretKey` provista al iniciar tu integración. Llave secreta del sitio.
- **seed:** La fecha en la que se genera la autenticación. En formato ISO 8601. Ejemplo: `2023-06-21T09:56:06-05:00`
- **nonce:** Valor arbitrario que identifica cada petición como única. Debe ser codificado en base 64 al enviarse. Ejemplo: `base64('927342197')`
- **tranKey:** Se genera en cada solicitud, de forma programática, aplicando la fórmula `Base64(SHA-256(nonce + seed + secretKey))` según el lenguaje de programación utilizado.

---

### Ejemplos de generación en diferentes lenguajes

#### PHP
```php
$login = "siteLogin";
$secretKey = "siteSecretKey";
$seed = date('c');
$rawNonce = rand();

$tranKey = base64_encode(hash('sha256', $rawNonce.$seed.$secretKey, true));
$nonce = base64_encode($rawNonce);

$body = [
  "auth" => [
    "login" => $login,
    "tranKey" => $tranKey,
    "nonce" => $nonce,
    "seed" => $seed,
  ],
  // ... other params
];
```

#### JavaScript
```js
const crypto = require('crypto');

const login = "siteLogin";
const secretKey = "siteSecretKey";
const seed = new Date().toISOString();
const rawNonce = Math.floor(Math.random() * 1000000);

const tranKey = Buffer.from(crypto.createHash('sha256').update(rawNonce + seed + secretKey).digest(), 'binary').toString('base64');
const nonce = Buffer.from(rawNonce.toString()).toString('base64');

const body = {
  auth: {
    login: login,
    tranKey: tranKey,
    nonce: nonce,
    seed: seed,
  },
  // ... other params
};
```

#### Python
```python
import base64, hashlib, random, datetime

login = "siteLogin"
secret_key = "siteSecretKey"

seed = datetime.datetime.now(datetime.timezone.utc).isoformat()
raw_nonce = random.getrandbits(128).to_bytes(16, byteorder="big")
nonce = base64.b64encode(raw_nonce).decode("utf-8")
tran_key = base64.b64encode(hashlib.sha256(raw_nonce + seed.encode() + secret_key.encode()).digest()).decode("utf-8")

return {
  "login": login,
  "tranKey": tran_key,
  "nonce": nonce,
  "seed": seed,
}
```

---

## Posibles errores

| Código   | Causa                                                                                 |
|----------|---------------------------------------------------------------------------------------|
| 100      | UsernameToken no proporcionado (encabezado de la autorización mal formado).           |
| 101      | Identificador de sitio no existe (login incorrecto o no se encuentra en el ambiente). |
| 102      | El hash de TranKey no coincide (tranKey incorrecto o mal formado).                    |
| 103      | Fecha de la semilla mayor de 5 minutos.                                               |
| 104      | Sitio inactivo.                                                                       |
| 105      | Sitio expirado.                                                                       |
| 106      | Credenciales expiradas.                                                               |
| 107      | Mala definición del UsernameToken (no cumple con el encabezado WSSE).                 |
| 200      | Saltar el encabezado de autenticación SOAP.                                           |
| 10001    | Contacte a Soporte.                                                                   |

---

## Errores frecuentes

**Mensaje de error "Autenticación mal formada":**  
Se presenta cuando el sistema no detecta que se está enviando login, tranKey, seed o nonce en la estructura auth enviada. También puede presentarse si se envían estos datos pero de manera incorrecta, por ejemplo, sin el parámetro content-type "application/json", lo que provoca que el servidor interprete la petición como texto en vez de un arreglo de datos. Puedes validar esto haciendo la petición a la URL [https://dnetix.co/p2p/client](https://dnetix.co/p2p/client) y capturando la respuesta, sirve como espejo de la petición para comprobar los parámetros y el *body* del mensaje.

**Error conectando al servicio con el mensaje ERROR: javax.net.ssl.SSLHandshakeException: Remote host closed connection during handshake:**  
Tus servidores requieren TLSv1.2 para recibir la solicitud, debido a la norma PCI. Por favor revisa el cifrado y el protocolo utilizado para conectar al servidor. Si usas Java, ten presente que solo las versiones posteriores a la 8 tienen soporte completo.

**SoapFault responde con el mensaje "Authentication Failed 103":**  
En el proceso de autenticación, Placetopay revisa el campo Created, que debe estar en GMT o tiempo local usando el tiempo de zona. Si obtienes esta respuesta, es porque tu tiempo no es preciso con el tiempo real. Solo permitimos 5 minutos de diferencia entre los tiempos. Puedes usar NTP para mantener la precisión del reloj.

**Dando los mismos valores EXACTOS que en los ejemplos anteriores a la BASE64(SHA256($Nonce + $Created . $secretKey)) estoy obteniendo un password digest diferente:**  
Recuerda que BASE64 debe realizarse sobre el output "raw" de SHA256 y en todos los lenguajes de programación puede requerirse una configuración específica. Por ejemplo, en PHP `base64_encode(hash('sha256' … , true))` retorna el output raw del algoritmo SHA256.