---
title: 'Navegadores compatibles'
description: 'Navegadores y versiones compatibles con Checkout.'
slug: 'navegadores-compatibles'
order: 7
---

# Navegadores Compatibles

Web Checkout está diseñado para ofrecer una experiencia segura y estable en las versiones modernas de los navegadores más utilizados a nivel mundial.

Para garantizar la seguridad y brindar la mejor experiencia posible a la mayoría de nuestros clientes, no ofrecemos soporte para navegadores que ya no reciben actualizaciones de seguridad y que son utilizados por solo una pequeña fracción de los usuarios.

## Entendiendo el soporte de navegadores

En Web Checkout, nos esforzamos por ofrecer la mejor experiencia posible para nuestros clientes, por lo que hemos definido una política de soporte de navegadores que se basa en los siguientes principios:

- Cubrimos navegadores y versiones de navegadores que tengan más del 0.5 % de participación a nivel mundial.
- Cubrimos las ultimas dos versiones de cada navegador.
- No cubrimos navegadores que ya no reciben actualizaciones de seguridad o que han sido declarados obsoletos (dead).
- No cubrimos Opera Mini, ya que no es compatible con las tecnologías modernas utilizadas en Web Checkout.
- No cubrimos Internet Explorer 11, ya que no es compatible tecnológicamente y ha sido declarado obsoleto e inseguro por Microsoft.

Estos valores corresponden a la regla Browserslist `> 0.5%, last 2 versions, not dead, not op_mini all, not IE 11` [Ver Más](https://browserslist.dev/?q=PiAwLjUlLCBsYXN0IDIgdmVyc2lvbnMsIG5vdCBkZWFkLCBub3Qgb3BfbWluaSBhbGwsIG5vdCBJRSAxMQ%3D%3D).


> Es probable que algunos navegadores por fuera de la regla se soporten con funcionalidades limitadas, pero no se garantiza su correcto funcionamiento.

<style>
/* Estilos para callouts con soporte de dark/light mode */
blockquote {
  border-left: 4px solid #3b82f6;
  padding: 1rem 1.5rem;
  margin: 1.5rem 0;
  border-radius: 8px;
  background-color: #eff6ff;
  color: #1e293b;
  position: relative;
  transition: all 0.3s ease;
}

blockquote p {
  margin: 0;
  line-height: 1.6;
}

blockquote p:first-child::before {
  content: "ℹ️";
  font-size: 1.2rem;
  margin-right: 0.5rem;
  vertical-align: middle;
}

/* Dark mode con media query */
@media (prefers-color-scheme: dark) {
  blockquote {
    background-color: rgba(59, 130, 246, 0.1);
    border-left-color: #60a5fa;
    color: #e0e7ff;
  }
}

/* Dark mode con clase manual */
.dark blockquote {
  background-color: rgba(59, 130, 246, 0.1);
  border-left-color: #60a5fa;
  color: #e0e7ff;
}
</style>