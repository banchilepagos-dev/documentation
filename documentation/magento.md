---
title: 'Magento'
description: 'Plugins y componentes para integración con Checkout.'
slug: 'plugins-componentes'
order: 7
---


  <img src="https://assets.bancochile.cl/uploads/000/089/117/b8befae6-1af0-480b-9e1f-37ea94fd0d23/original/imagen_6_.png" alt="Portada Magento" class="">

<div class="title-general">
    <h1>Acepta pagos con Banchile Pagos y Magento</h1>
</div>
En esta guía se explica paso a paso la instalación y configuración del plugin de Banchile Pagos para Magento.

Cada parámetro de configuración descrito en esta guía se realizará en un entorno de pruebas con el fin de ilustrar detalladamente su configuración.

Para utilizar Banchile Pagos es necesario contar con una cuenta activa.  
Si aún no tienes una, comunícate con nosotros. Si deseas obtener más información, ponte en contacto con nuestro equipo de ventas.

## Requisitos
- Tener Magento instalado y funcionando correctamente.
- Tener una cuenta activa de Banchile Pagos (Login y SecretKey).

## 1. Inicia sesión en tu cuenta de Magento
1. Accede al panel de administración de tu tienda Magento.
2. En el menú lateral izquierdo realiza los pasos siguientes para instalar y configurar el plugin.

## 2. Instalación del plugin
Ingresa a tu consola e instala el plugin con los comandos proporcionados por Banchile Pagos o por la documentación del plugin.

```bash
# Ejecuta aquí los comandos de instalación del plugin (proporcionados por Banchile Pagos)
# Ejemplo (sustituir por los comandos reales):
# composer require Banchile Pagos/magento-plugin
# php bin/magento module:enable Banchile Pagos_Module
# php bin/magento setup:upgrade
# php bin/magento cache:flush
```

Una vez que hayas instalado correctamente el plugin en la consola, regresa al navegador donde tienes abierta tu cuenta de Magento.

## 3. Navegar a la configuración en Magento
1. En el menú lateral izquierdo, selecciona **Stores**.
2. Dentro de **Stores**, selecciona **Configuration**.

### 3.1 Ajustes generales
1. En la sección de **Configuration**, en el panel lateral busca el desplegable **General**.
2. Dentro de **General**, localiza la opción **Default Country** y selecciona el país correspondiente a la tienda.

### 3.2 Métodos de pago
1. Vuelve a la sección **Configuration** y en el panel lateral abre el desplegable **Sales**.
2. Selecciona **Payment Methods**.
3. Si la instalación se realizó correctamente, verás el plugin de Banchile Pagos en la lista de métodos de pago. Haz clic en el botón **Configure** junto al plugin.

## 4. Configuración del plugin (Connection Settings)
Dentro de la configuración del plugin, busca la sección **Connection Settings** y despliega sus opciones. Las principales opciones a configurar son:

- I am integrated with: Selecciona el proveedor correcto según tu integración.
- Mode: Selecciona la opción **Producción**.
- Production Login: Ingresa el valor de **Login** que se te ha enviado por correo electrónico.
- Production TranKey: Ingresa el valor de **SecretKey** que se te ha enviado por correo electrónico.

El resto de la configuración es personalizable y dependerá de las necesidades específicas de tu comercio.

## 5. Estados de las órdenes en Magento (con el plugin Banchile Pagos)
Magento puede manejar diferentes estados para una orden. Con el plugin de Banchile Pagos, los estados posibles son:

- Pendiente de pago: La orden está en espera de que se realice el pago. Puede pasar automáticamente a **Completado** o **Procesando** según corresponda.
- Completado: El pago ha sido realizado correctamente.
- Procesando: Orden en revisión de la transacción (aplica a pago único como efectivo o transferencia, o a pagos con autorización).
- Reembolsado: Se ha realizado el reembolso y se actualiza el stock de la tienda con los productos devueltos.
- Fallido: No se pudo realizar la transacción (fondos insuficientes, datos erróneos u otros motivos).

---
Notas finales:
- Realiza pruebas en el entorno de pruebas antes de pasar a producción.
- Guarda y prueba cada cambio de configuración para asegurar el correcto funcionamiento del flujo de pago.




https://assets.bancochile.cl/uploads/000/089/110/caee0697-ed2d-4562-88ab-c3bc4f1b2a11/original/imagen_13_.png
https://assets.bancochile.cl/uploads/000/089/112/98350cdd-fd4e-48c6-8a38-15b4b4a26fdb/original/imagen_11_.png

https://assets.bancochile.cl/uploads/000/089/111/d76ee573-72cd-4005-b6ec-0b3e42818040/original/imagen_12_.png

https://assets.bancochile.cl/uploads/000/089/113/d82ccbe5-ab7d-4d2f-a310-70cb7c80bf6c/original/imagen_10_.png

https://assets.bancochile.cl/uploads/000/089/114/79c2966e-37b2-4040-a48e-471cb564f48d/original/imagen_9_.png
https://assets.bancochile.cl/uploads/000/089/114/79c2966e-37b2-4040-a48e-471cb564f48d/original/imagen_9_.png
https://assets.bancochile.cl/uploads/000/089/115/7d0f4e75-8185-450e-bc8f-8452092baf7e/original/imagen_8_.png
https://assets.bancochile.cl/uploads/000/089/116/90404bb4-ecf0-40f3-86a6-96042204acfe/original/imagen_7_.png
https://assets.bancochile.cl/uploads/000/089/118/95c8bcde-f40c-4e0c-8e85-1b6100b28dc7/original/imagen_1_.jpg


<style>
    .title-general{
        text-align: center;
        margin-top: 50px;
    }
</style>