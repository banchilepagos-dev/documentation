---
title: 'Plugins y Componentes'
description: 'Plugins y componentes para integración con Checkout.'
slug: 'plugins-componentes'
order: 6
---

# Plugins 

Puedes usar nuestros plugins y componentes para integrarte de forma más rápida con Checkout.



<div class="plugins-grid">

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://assets.bancochile.cl/uploads/000/088/637/fcb442af-e965-449e-83c8-e5e374d553b1/original/woocommerce.png" alt="WooCommerce" class="plugin-icon">
    <h3>WooCommerce</h3>
  </div>
  <p>Plugin para WordPress. Diseñado para tiendas y comercios en línea que usan WordPress.</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>

<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://assets.bancochile.cl/uploads/000/088/635/1590f463-e2ea-46ff-99f9-bac6aa902e48/original/magento.png" alt="Magento" class="plugin-icon">
    <h3>Magento</h3>
  </div>
  <p>Plataforma de código abierto para comercio electrónico escrita en PHP.</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>


<div class="plugin-card">
  <div class="plugin-header">
    <img src="https://assets.bancochile.cl/uploads/000/088/634/8549ab8c-aa34-4bd4-ae50-cea7243a79a1/original/jumpseller.png" alt="Jumpseller" class="plugin-icon">
    <h3>Jumpseller</h3>
  </div>
  <p>Plataforma de comercio electrónico para crear tu tienda en línea.</p>
  <a href="#" class="plugin-link">Ver más →</a>
</div>
</div>



<!-- ## Librerías
---
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

</div> -->

<style>
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
