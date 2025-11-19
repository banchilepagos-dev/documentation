---
title: "Plugins y Componentes"
description: "Plugins y componentes para integración con Checkout."
slug: "plugins-componentes"
sections:
  - magento
  - prestashop
  - woocommerce
order: 6
---

# Plugins

Puedes usar nuestros plugins y componentes para integrarte de forma más rápida con Checkout.

<div class="plugins-grid">

<div class="plugin-card" >
  <div class="plugin-header">
    <img src="https://assets.bancochile.cl/uploads/000/088/637/fcb442af-e965-449e-83c8-e5e374d553b1/original/woocommerce.png" alt="WooCommerce" class="plugin-icon">
    <h3>WooCommerce</h3>
  </div>
  <p>Plugin para WordPress. Diseñado para tiendas y comercios en línea que usan WordPress.</p>
  <a href="#woocommerce" class="plugin-link">Ver más →</a>
</div>

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://assets.bancochile.cl/uploads/000/088/635/1590f463-e2ea-46ff-99f9-bac6aa902e48/original/magento.png" alt="Magento" class="plugin-icon">
    <h3>Magento</h3>
  </div>
  <p>Plataforma de código abierto para comercio electrónico escrita en PHP.</p>
  <a href="#documentation#plugins-componentes#magento" class="plugin-link">Ver más →</a>
</div>

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://assets.bancochile.cl/uploads/000/088/634/8549ab8c-aa34-4bd4-ae50-cea7243a79a1/original/jumpseller.png" alt="Jumpseller" class="plugin-icon">
    <h3>Jumpseller</h3>
  </div>
  <p>Plataforma de comercio electrónico para crear tu tienda en línea.</p>
  <a href="#prestashop" class="plugin-link">Ver más →</a>
</div>
</div>

<!-- 
<div class="plugins-grid">

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://cdn.worldvectorlogo.com/logos/php-1.svg" alt="PHP" class="plugin-icon">
    <h3>PHP</h3>
  </div>
  <p>Lenguaje de programación de código abierto, especialmente adecuado para el desarrollo web</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://cdn.worldvectorlogo.com/logos/c--4.svg" alt="C#" class="plugin-icon">
    <h3>C#</h3>
  </div>
  <p>Lenguaje de programación moderno y orientado a objetos desarrollado por Microsoft</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://cdn.worldvectorlogo.com/logos/java.svg" alt="Java" class="plugin-icon">
    <h3>Java</h3>
  </div>
  <p>Lenguaje de programación de alto nivel y orientado a objetos</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://cdn.worldvectorlogo.com/logos/python-5.svg" alt="Python" class="plugin-icon">
    <h3>Python</h3>
  </div>
  <p>Lenguaje de programación versátil y de alto nivel, ampliamente utilizado en el desarrollo de aplicaciones modernas.</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>

</div>  -->




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

## PrestaShop

  <img src="https://assets.bancochile.cl/uploads/000/089/206/02795c80-29d5-4119-a75e-f68cdee7ce0a/original/00.png" alt="Portada prestashop" class="">

<div class="title-general">
    <h3 id="prestashop">Acepta pagos con Banchile Pagos y PrestaShop</h3>
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

## Woocommerce

 <img src="https://assets.bancochile.cl/uploads/000/089/189/f4fe06a6-f37b-49f9-9873-b58a90dcd02f/original/0.png" alt="Wordpress" class="">

<div class="title-general">
<h3 id="woocommerce"> Acepta pagos con Banchile Pagos y WooCommerce </h3>
</div>

Esta guía te proporciona un paso a paso detallado para la instalación del plugin WooCommerce Gateway Banchile Pagos. Cabe destacar que todos los aspectos de esta guía se realizarán en un entorno de pruebas, con el objetivo de ilustrar a fondo su configuración.

Para llevar a cabo el proceso de integración, se asume que el comercio ya ha instalado previamente el componente WooCommerce en su sitio de WordPress.

### Por favor siga los pasos que siguen a continuación.

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

### Estados de las órdenes en WooCommerce

En WooCommerce podemos tener diferentes estados para una orden. A continuación se detallan los estados posibles de la orden con el plugin:

- **Pendiente de pago:** está en espera de que se realice el pago. Pasa automáticamente a estado Completado o Procesando dependiendo del caso.
- **Completado:** el pago ha sido realizado correctamente.
- **Procesando:** proceso de revisión de la transacción tanto para pago único (efectivo y transferencia), como para pago con autorización.
- **Reembolsado:** realiza el reembolso y actualiza el stock de la tienda con los productos devueltos.
- **Fallido:** no se pudo realizar la transacción ya sea por fondos insuficientes o por datos erróneos.

### Modo depuración

Dentro de la sección de configuración del componente existen parametrizaciones que solo se visualizan con el Modo depuración activado, dentro de ellas:

- URL de notificación.
- Ubicación tarea programada.


<div class="plugins-list">
  
  <a class="plugin-link" data-page="jumpseller" href="/plugins-componentes/jumbseller">jumbselle →</a>
</div>

<!-- 
<script>
(function(){
  const container = document.getElementById('plugin-dynamic-container');
  async function load(path, push=true){
    const url = path.startsWith('/') ? path : '/plugins-componentes/' + path;
    const res = await fetch(url);
    if(!res.ok) { container.innerHTML = '<p>Error cargando contenido.</p>'; return; }
    const html = await res.text();
    // Extrae solo el contenido principal (ajusta el selector a tu generador)
    const tmp = document.createElement('div');
    tmp.innerHTML = html;
    const main = tmp.querySelector('main, article, #__content, .content, body') || tmp;
    // Opcional: toma solo lo que está después del primer h1
    container.innerHTML = main.innerHTML;
    if(push) history.pushState({sub:path}, '', url);
    // Scroll suave al inicio del contenido
    container.scrollIntoView({behavior:'smooth', block:'start'});
  }
  // Interceptar clics
  document.addEventListener('click', (e)=>{
    const a = e.target.closest('a.plugin-link[data-page]');
    if(!a) return;
    e.preventDefault();
    load(a.getAttribute('href').replace(location.origin,''));
  });
  // Soporta navegación atrás/adelante
  window.addEventListener('popstate', (e)=>{
    const sub = e.state?.sub;
    if(sub) load(sub, false);
    else container.innerHTML = '';
  });
  // Carga inicial si llega directo a sub-página y quieres mostrarla integrada
  const path = location.pathname.replace(/\/$/,'');
  const match = path.match(/\/plugins-componentes\/(magento|prestashop|woocommerce)$/);
  if(match) load(match[0], false);
})();
</script> -->


<style>
#plugin-dynamic-container {
  margin-top: 2rem;
  border-top: 1px solid #e2e8f0;
  padding-top: 1.5rem;
  min-height: 200px;
}
.plugins-list a {
  display:inline-block;
  margin:.5rem 1rem .5rem 0;
  text-decoration:none;
  font-weight:600;
  color:#0033A0;
}
.plugins-list a:hover { text-decoration:underline; }
.destacado-hash {
  outline: 3px solid #0033A0;
  padding: 4px 8px;
  border-radius: 6px;
  background: rgba(0,51,160,.06);
}
@media (prefers-color-scheme: dark) {
  .destacado-hash {
    background: rgba(96,165,250,.15);
  }
}

.title-general{
  text-align: center;
  margin-top: 50px;
  }
.border-img{
  border-radius:12px;
   }
.plugins-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

/* Estilos base para light mode (por defecto) */
.plugin-card {
  background-color: #ffffff;
  border: 1px solid #e2e8f0;
  border-radius: 12px;
  padding: 1.5rem;
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.plugin-card:hover {
  border-color: #0033A0;
  transform: translateY(-4px);
  box-shadow: 0 8px 16px rgba(0, 51, 160, 0.15);
}

.plugin-header {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.plugin-icon {
  width: 48px;
  height: 48px;
  object-fit: contain;
}

.plugin-card h3 {
  color: #1e293b;
  font-size: 1.25rem;
  font-weight: 600;
  margin: 0;
}

.plugin-card p {
  color: #64748b;
  font-size: 0.95rem;
  line-height: 1.6;
  margin: 0;
  flex-grow: 1;
}

.plugin-link {
  color: #0033A0;
  text-decoration: none;
  font-weight: 500;
  display: inline-flex;
  align-items: center;
  gap: 0.25rem;
  transition: color 0.2s ease;
}

.plugin-link:hover {
  color: #0056d6;
  text-decoration: underline;
}

/* Dark mode automático con media query */
@media (prefers-color-scheme: dark) {
  .plugin-card {
    background-color: rgba(30, 41, 59, 0.9);
    border-color: #475569;
  }
  
  .plugin-card:hover {
    border-color: #60a5fa;
    box-shadow: 0 8px 16px rgba(96, 165, 250, 0.3);
  }
  
  .plugin-card h3 {
    color: #f1f5f9;
  }
  
  .plugin-card p {
    color: #cbd5e1;
  }
  
  .plugin-link {
    color: #60a5fa;
  }
  
  .plugin-link:hover {
    color: #93c5fd;
  }
}

/* Dark mode manual class support */
.dark .plugin-card {
  background-color: rgba(30, 41, 59, 0.9);
  border-color: #475569;
}

.dark .plugin-card:hover {
  border-color: #60a5fa;
  box-shadow: 0 8px 16px rgba(96, 165, 250, 0.3);
}

.dark .plugin-card h3 {
  color: #f1f5f9;
}

.dark .plugin-card p {
  color: #cbd5e1;
}

.dark .plugin-link {
  color: #60a5fa;
}

.dark .plugin-link:hover {
  color: #93c5fd;
}
</style>
