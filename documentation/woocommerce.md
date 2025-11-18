---
title: 'Woocommerce'
description: 'Plugins de woocommerce'
slug: 'plugin-woocommerce'
order: 8
---
 
 
 <img src="https://assets.bancochile.cl/uploads/000/089/189/f4fe06a6-f37b-49f9-9873-b58a90dcd02f/original/0.png" alt="Wordpress" class="">

<div class="title-general">
<h1> Acepta pagos con Banchile Pagos y WooCommerce </h1>
</div>

Esta guía te proporciona un paso a paso detallado para la instalación del plugin WooCommerce Gateway Banchile Pagos. Cabe destacar que todos los aspectos de esta guía se realizarán en un entorno de pruebas, con el objetivo de ilustrar a fondo su configuración.

Para llevar a cabo el proceso de integración, se asume que el comercio ya ha instalado previamente el componente WooCommerce en su sitio de WordPress.

## Por favor siga los pasos que siguen a continuación.

1. Inicia sesión en tu cuenta de WordPress.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/124/f78c08e0-95be-4b7d-8d0c-a3ac94852cd9/original/imagen_19_.png" alt="Wordpress" >

2. En el menú lateral izquierdo, dirígete a la opción de `Plugins`. Al pasar el cursor sobre ella, se desplegarán dos opciones adicionales. Selecciona la opción `Añadir nuevo`.
 
 <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/123/3d06c3d2-1c52-47ee-9189-5bf16696e9c1/original/imagen_20_.png" alt="Wordpress" >

3. Justo al lado del título `Añadir plugin`, encontrarás un botón en la parte superior que dice `Subir plugin`. Haz clic en el botón.

<img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/122/07146959-7ab3-4bfd-a639-008dd393d07b/original/imagen_21_.png" alt="Wordpress" >

 
4. Haz clic en el botón `Buscar` o `Examinar` y busca el archivo del plugin que has descargado. Asegúrate de que el archivo esté comprimido en formato ZIP.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/190/c6b47e12-6543-4bb2-bbf4-52f953838fc8/original/Plugin-Woocommerce-1.webp" alt="Wordpress" >

5. Una vez cargado el archivo ZIP, haz clic en el botón `Instalar ahora`. Ten en cuenta que la instalación del plugin puede tardar unos minutos.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/129/faca8d5c-b7e7-4039-b42f-54d4e0f5908a/original/imagen_14_.png" alt="Wordpress" >

6. Al finalizar la instalación, se mostrará un mensaje de confirmación. Asegúrate de que el mensaje indique `Plugin instalado con éxito` antes de proceder a activar y configurar el plugin.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/127/25699862-b4bb-4943-8d29-6168a79c406d/original/imagen_16_.png" alt="Wordpress" >

7. Una vez finalizada la instalación, selecciona la opción `WooCommerce` en el menú lateral izquierdo e ingresa a la opción de `Ajustes`.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/131/7371fe70-4a61-4ce2-b9b3-5fd1cbfe3578/original/imagen_23_.png" alt="Wordpress" >

8. Selecciona la opción `País/Estado` y establece el país correspondiente a tu tienda.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/130/6d1373e0-a2b1-4c38-91bd-21f29e91a87b/original/imagen_2_.jpg" alt="Wordpress" >

9. Luego, selecciona la opción `Plugins instalados` en el menú lateral izquierdo.
   a. Esto te llevará a la lista de todos los plugins instalados en tu sitio.  
   b. Busca entre tus plugins el llamado `WooCommerce Banchile Pagos Gateway` y haz clic en el botón `Configuración` que se encuentra justo debajo del título.

   <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/125/1d2545e6-130f-4301-8592-257202bd337b/original/imagen_18_.png" alt="Wordpress" class="">

10. Serás redirigido a la sección de pagos, donde podrás configurar el plugin de Banchile Pagos. Asegúrate de tener a mano los datos que te hemos enviado por correo electrónico, ya que los necesitarás para ingresarlos en esta sección.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/128/bedb7f30-44e6-4529-9d8e-260dbdb3a9b4/original/imagen_15_.png" alt="Wordpress" class="">

11. Desplázate hacia abajo utilizando el scroll hasta encontrar la siguiente configuración, y asígnala de la siguiente manera:

    - Cliente: Asegúrate de seleccionar el correcto según tu proveedor.
    - Identificador: Ingresa el dato de `Login` que se te ha enviado por correo electrónico.
    - Clave transaccional: Ingresa el dato de `SecretKey` que se te ha enviado por correo electrónico.

  <img class="border-img" src="https://assets.bancochile.cl/uploads/000/089/126/b0d374cb-2888-476b-b31b-5e05101ec830/original/imagen_17_.png" alt="Wordpress" class="">
      

El resto de la configuración es personalizable y dependerá exclusivamente de las necesidades específicas de tu comercio.

## Estados de las órdenes en WooCommerce

En WooCommerce podemos tener diferentes estados para una orden. A continuación se detallan los estados posibles de la orden con el plugin:

- **Pendiente de pago:** está en espera de que se realice el pago. Pasa automáticamente a estado Completado o Procesando dependiendo del caso.
- **Completado:** el pago ha sido realizado correctamente.
- **Procesando:** proceso de revisión de la transacción tanto para pago único (efectivo y transferencia), como para pago con autorización.
- **Reembolsado:** realiza el reembolso y actualiza el stock de la tienda con los productos devueltos.
- **Fallido:** no se pudo realizar la transacción ya sea por fondos insuficientes o por datos erróneos.

## Modo depuración

Dentro de la sección de configuración del componente existen parametrizaciones que solo se visualizan con el Modo depuración activado, dentro de ellas:

- URL de notificación.
- Ubicación tarea programada.


<style>
    .title-general{
        text-align: center;
        margin-top: 50px;
    }
    .border-img{
        border-radius:12px;
    }
</style>





 

