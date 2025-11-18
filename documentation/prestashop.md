  <img src="https://assets.bancochile.cl/uploads/000/089/206/02795c80-29d5-4119-a75e-f68cdee7ce0a/original/00.png" alt="Portada prestashop" class="">

<div class="title-general">
    <h1>Acepta pagos con Banchile Pagos y PrestaShop</h1>
</div>

En esta guía, se explicará paso a paso la instalación del plugin de Banchile Pagos para PrestaShop. Cada parámetro de configuración descrito en esta guía se realizará en un entorno de pruebas con el fin de ilustrar detalladamente su configuración.

Descarga nuestro plugin para integrarlo con la plataforma de PrestaShop.

Para comenzar, inicia sesión en tu cuenta de PrestaShop.

1. Iniciar sesión Prestashop
   <img src="https://assets.bancochile.cl/uploads/000/089/208/cb1dcefb-e65e-4666-aba1-d71b2e12a6a5/original/Plugin-Prestashop-placetopay-unoCCzVyBdI.webp" alt="inicio" class="border-img">

2. En el menú lateral izquierdo, dirígete a la opción ‘Módulos’. Al hacer clic, se desplegarán dos opciones adicionales, y deberás seleccionar ‘Catálogo de módulos’.
  <img src="https://assets.bancochile.cl/uploads/000/089/210/a1ce678a-6e5f-4c9a-a160-b4066d2eba25/original/Plugin-Prestashop-placetopay-dosCotRrDoa.webp" alt="modulo-prestashop" class="border-img">
  

3. Una vez en esta vista, encontrarás en la parte superior un botón que dice ‘Subir módulo’. Haz clic en él.
   <img src="https://assets.bancochile.cl/uploads/000/089/209/7ffc7a91-757a-4389-b129-71b67a7bc8b7/original/Plugin-Prestashop-placetopay-tresBOe_DmLe.webp" alt="btn-modulo" class="border-img">

4. Se abrirá un modal en el que podrás arrastrar el plugin o buscar el archivo del plugin que has descargado recientemente. Asegúrate de subir el archivo exactamente tal como está, comprimido en formato ZIP.
   <img src="https://assets.bancochile.cl/uploads/000/089/213/f298a991-d8dc-4d3f-b388-f78408ef32fa/original/Plugin-Prestashop-placetopay-cuatrorS4gHYGl.webp" alt="modal-prestashop" class="border-img">

5. Una vez finalizada la instalación, selecciona la opción ‘Internacional’ en el menú lateral izquierdo e ingresa a la opción de ‘Localización’.

  <img src="https://assets.bancochile.cl/uploads/000/089/212/9fcd8f1e-f2c0-448d-ab79-7adf7506c0f3/original/Plugin-Prestashop-placetopay-cuatro-1BFuEseOm.webp" alt="seleccion-internacional" class="border-img">

6. Selecciona la opción ‘País predeterminado’ y establece el país correspondiente a tu tienda.

  <img src="https://assets.bancochile.cl/uploads/000/089/211/c677ca00-99d5-43b4-962c-cafc64b56022/original/Plugin-Prestashop-placetopay-cuatro-2BUvMUPu7.webp" alt="pais-seleccion" class="border-img">

7. Luego, puedes hacer clic en el botón ‘Configurar’ o dirigirte al menú lateral izquierdo y buscas la sección de ‘Personalizar’. A continuación, busca la opción ‘Módulos’ y haz clic en ella. Se desplegarán dos opciones, y deberás seleccionar ‘Gestor de módulos’.

<img src="https://assets.bancochile.cl/uploads/000/089/214/3a3dd92c-9181-44d2-888e-86fe9af1df78/original/Plugin-Prestashop-placetopay-cincoDjKWvwfS.webp" alt="" class="border-img">

8. Una vez en el Gestor de módulos, deberías visualizar el plugin de Banchile Pagos. Allí verás un botón que dice Actualizar con una flecha al junto. Al hacer clic en la flecha, se desplegarán más opciones. Haz clic en la opción de ‘Configurar’.

  <img src="https://assets.bancochile.cl/uploads/000/089/219/3bae845c-d995-47d6-a9ea-ae22e00df188/original/01_3.png" alt="" class="border-img">

9. Una vez en la configuración, desplázate hacia abajo hasta encontrar la opción de ‘Configuración de conexión’, donde configuraremos nuestro plugin de la siguiente manera:

a. **Estoy integrado con:** Asegúrate de seleccionar el correcto según tu proveedor.

b. **En modo:** Selecciona la opción ‘Producción’.

c. **Login:** Ingresa el dato de ‘Login’ que se te ha enviado por correo electrónico.

d. **TranKey:** Ingresa el dato de ‘SecretKey’ que se te ha enviado por correo electrónico.

Finaliza la configuración haciendo clic en ‘Guardar’.

  <img src="https://assets.bancochile.cl/uploads/000/089/204/5f8a0ab1-d181-4f92-a355-d1f424d4fa8e/original/02_2.png" alt="" class="border-img">

El resto de la configuración es personalizable y dependerá exclusivamente de las necesidades específicas de tu comercio.

En Prestashop podemos tener diferentes estados para una orden. A continuación se detallan los estados posibles de la orden con el plugin:

- **Pendiente de pago:** está en espera de que se realice el pago. Pasa automáticamente a estado Completado o Procesando dependiendo del caso.
- **Completado:** el pago ha sido realizado correctamente.
- **Procesando:** proceso de revisión de la transacción tanto para pago único (efectivo y transferencia), como para pago con autorización.
- **Reembolsado:** realiza el reembolso y actualiza el stock de la tienda con los productos devueltos.
- **Fallido:** no se pudo realizar la transacción ya sea por fondos insuficientes o por datos erróneos.



https://assets.bancochile.cl/uploads/000/089/205/aa159972-b497-4f82-b81c-2166bb58fee6/original/01_2.png



<style>
    .title-general{
        text-align: center;
        margin-top: 50px;
    }
    .border-img{
        border-radius:12px;
    }
</style>




