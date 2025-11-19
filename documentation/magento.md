---
title: "magento"
slug: "plugins-componentes#magento"
order: 1
---

## Magento

  <img src="https://assets.bancochile.cl/uploads/000/089/117/b8befae6-1af0-480b-9e1f-37ea94fd0d23/original/imagen_6_.png" alt="Portada Magento" class="">

<div class="title-general">
    <h3 id="magento">Acepta pagos con Banchile Pagos y Magento</h3>
</div>
En esta guía, se explicará paso a paso la instalación del plugin de Placetopay para Magento.

Cada parámetro de configuración descrito en esta guía se realizará en un entorno de pruebas con el fin de ilustrar detalladamente su configuración.

Para realizar las respectivas configuraciones se debe tener la tienda de Magento instalada correctamente.

1. Inicia sesión en tu cuenta de Magento.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/118/95c8bcde-f40c-4e0c-8e85-1b6100b28dc7/original/imagen_1_.jpg" alt="Login Magento">

2. Una vez que hayas instalado correctamente el plugin en tu consola, regresa al navegador donde tienes abierta tu cuenta de Magento. En el menú lateral izquierdo, busca la opción ‘Stores’. Al hacer clic en ella, se desplegarán opciones adicionales, entre las cuales seleccionaremos ‘Configuración’.
   <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/112/98350cdd-fd4e-48c6-8a38-15b4b4a26fdb/original/imagen_11_.png" alt="Config Magento">

3. Dentro de la sección de ‘Configuración’, busca en el panel lateral de opciones el menú desplegable llamado ‘General’.

<img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/110/caee0697-ed2d-4562-88ab-c3bc4f1b2a11/original/imagen_13_.png
 " alt="general Magento">

4. Una vez dentro del apartado ‘General’, buscaremos la opción ‘Default country’ y haremos clic en ella para seleccionar el pais correspondiente a la tienda.

 <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/111/d76ee573-72cd-4005-b6ec-0b3e42818040/original/imagen_12_.png" alt="Country Magento">

5. Volvemos a la sección de ‘Configuración’, busca en el panel lateral de opciones el menú desplegable llamado ‘Sales’. Al desplegarlo, encontrarás la opción de ‘Payment Methods’

<img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/113/d82ccbe5-ab7d-4d2f-a310-70cb7c80bf6c/original/imagen_10_.png" alt="Country Magento">

6. Si la instalación en la consola se realizó correctamente, deberá aparecer en la vista de ‘Payment Methods’ el plugin de Placetopay. Junto al plugin, veremos un botón que dice ‘Configure’, al cual haremos clic  
   metodos de pagos PlacetoPay

<img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/114/79c2966e-37b2-4040-a48e-471cb564f48d/original/imagen_9_.png" alt="Country Magento">

Una vez dentro de la configuración del plugin, buscaremos la opción ‘Connection Settings’ y haremos clic en ella para desplegar su información.  
<img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/116/90404bb4-ecf0-40f3-86a6-96042204acfe/original/imagen_7_.png" alt="Country Magento">

Al desplegar esta opción encontraremos varias opciones para configurar nuestro plugin, entre ellas las que nos interesa son:

a. I am integrated with: Asegúrate de seleccionar el correcto según tu proveedor.

b. Mode: Selecciona la opción ‘Producción’.

c. Production Login: Ingresa el dato de ‘Login’ que se te ha enviado por correo electrónico.

d. Production TranKey: Ingresa el dato de ‘SecretKey’ que se te ha enviado por correo electrónico.

<img src="https://assets.bancochile.cl/uploads/000/089/115/7d0f4e75-8185-450e-bc8f-8452092baf7e/original/imagen_8_.png" alt="secret key Magento">

El resto de la configuración es personalizable y dependerá exclusivamente de las necesidades específicas de tu comercio.

### Estados de las órdenes en Magento

En Magento podemos tener diferentes estados para una orden. A continuación se detallan los estados posibles de la orden con el plugin:

- Pendiente de pago: está en espera de que se realice el pago. Pasa automáticamente a estado Completado o Procesando dependiendo del caso.

- Completado: el pago ha sido realizado correctamente.

- Procesando: proceso de revisión de la transacción tanto para pago único (efectivo y transferencia), como para pago con autorización.

- Reembolsado: realiza el reembolso y actualiza el stock de la tienda con los productos devueltos.

- Fallido: no se pudo realizar la transacción ya sea por fondos insuficientes o por datos erróneos.