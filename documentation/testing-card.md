---
title: 'Tarjetas de prueba'
description: 'Pruebas con tarjetas de crédito y débito en ambiente de desarrollo.'
slug: 'testing-card'
order: 5
---

import { TestCardNumbers } from '@/components/TestCardNumber';

# Números de tarjeta de pruebas

Es importante definir que estas tarjetas solo tienen dicho comportamiento en el ambiente de pruebas

En todos los casos excepto donde se especifique el CVV y la fecha de expiración puede ser cualquiera con tal de que sea vigente para que su comportamiento aplique.

Para las pruebas con 3DS en el comportamiento se describe su resultado

* **Y**: Autenticado sin fricción
* **C**: Solicita autenticación con Fricción (Desafío)
* **D**: Autenticación Desacoplada
* **A**: Intento de Autenticación
* **N**: No autenticado

<details>
<summary><strong>VISA</strong></summary>

<div class="card-table-container">

| Número | Comportamiento |
|--------|----------------|
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000081')" title="Click para copiar">`4110760000000081` </span> | Aprueba |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110770010002837')" title="Click para copiar">`4110770010002837` </span> | Aprueba |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4381080000000029')" title="Click para copiar">`4381080000000029` </span> | Aprueba |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4111111111111111')" title="Click para copiar">`4111111111111111` </span> | Aprueba 3DS-Y |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000008')" title="Click para copiar">`4110760000000008` </span> | Aprueba 3DS-C |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000016')" title="Click para copiar">`4110760000000016` </span> | Rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4005580000000040')" title="Click para copiar">`4005580000000040` </span> | Rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4716375184092180')" title="Click para copiar">`4716375184092180` </span> | Rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4381080000000011')" title="Click para copiar">`4381080000000011` </span> | Rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4716375184092180')" title="Click para copiar">`4716375184092180` </span> | Rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000032')" title="Click para copiar">`4110760000000032` </span> | Deja la transacción en estado pendiente y se resuelve a aprobado 3DS-C |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000040')" title="Click para copiar">`4110760000000040` </span> | Deja la transacción en estado pendiente y se resuelve a rechazado 3DS-A |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4048370000000037')" title="Click para copiar">`4048370000000037` </span> | Deja la transacción en estado pendiente y se resuelve a rechazado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000073')" title="Click para copiar">`4110760000000073` </span> | Deja la transacción en estado pendiente y se resuelve a aprobado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000065')" title="Click para copiar">`4110760000000065` </span> | Arroja una excepción en el proceso 3DS-N |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000024')" title="Click para copiar">`4110760000000024` </span> | Se tarda 180 segundos en responder y queda en estado aprobado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000115')" title="Click para copiar">`4110760000000115` </span> | Se tarda 180 segundos en responder y queda en estado rechazado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4110760000000057')" title="Click para copiar">`4110760000000057` </span> | Aprueba si el monto es inferior a 200USD de lo contrario rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4012888888881881')" title="Click para copiar">`4012888888881881` </span> | Aprueba si se proporciona la expiración 11/28 y el cvv 917 de lo contrario rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4381080000000003')" title="Click para copiar">`4381080000000003` </span> | Deja la transacción en estado pendiente y se resuelve a rechazado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4509564638437551')" title="Click para copiar">`4509564638437551` </span> | Deja la transacción en estado pendiente y se resuelve a aprobado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4864921336824366')" title="Click para copiar">`4864921336824366` </span> | Deja la transacción en estado pendiente y se resuelve a rechazado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4931974429847108')" title="Click para copiar">`4931974429847108` </span> | Deja la transacción en estado pendiente y se resuelve a rechazado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4532034637206853')" title="Click para copiar">`4532034637206853` </span> | Deja la transacción en procesamiento manual y si se procesa queda en estado rechazado |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('4666666666666669')" title="Click para copiar">`4666666666666669` </span> | Se tarda 180 segundos en responder y queda en estado aprobado |

</div>

</details>

<details>
<summary><strong> MASTERCARD</strong> </summary>

<div class="card-table-container">

| Número | Comportamiento |
|--------|----------------|
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5367680000000005')" title="Click para copiar">`5367680000000005` 📋</span> | Aprueba |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5180300000000005')" title="Click para copiar">`5180300000000005` 📋</span> | Aprueba 3DS-Y |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5292594382060745')" title="Click para copiar">`5292594382060745` 📋</span> | Aprueba 3DS-C |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5367680000000013')" title="Click para copiar">`5367680000000013` 📋</span> | Rechaza |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5180300000000039')" title="Click para copiar">`5180300000000039` 📋</span> | Rechaza 3DS-N |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5180300000000047')" title="Click para copiar">`5180300000000047` 📋</span> | Deja la transacción en estado pendiente y se resuelve a aprobado 3DS-C |
| <span class="copyable-card" onclick="navigator.clipboard.writeText('5180300000000054')" title="Click para copiar">`5180300000000054` 📋</span> | Deja la transacción en estado pendiente y se resuelve a rechazado **3DS-A** |

</div>

</details>

<style>
details {
  border: 1px solid #e5e7eb;
  border-radius: 8px;
  padding: 1rem;
  margin: 1.5rem 0;
  background-color: #f9fafb;
  transition: background-color 0.3s ease, border-color 0.3s ease;
}

/* Dark mode styles */
@media (prefers-color-scheme: dark) {
  details {
    background-color: rgba(31, 41, 55, 0.8);
    border-color: #374151;
  }
  
  details summary {
    color: #ffffff;
  }
  
  details[open] summary {
    border-bottom-color: #0033A0;
    color: #ffffff;
  }
  
  .copyable-card:hover {
    background-color: rgba(55, 65, 81, 0.8);
  }
  
  .copyable-card:active {
    background-color: rgba(75, 85, 99, 0.8);
  }
  
  .card-table-container table {
    color: #ffffff;
  }
  
  .card-table-container th {
    background-color: rgba(55, 65, 81, 0.8);
    border-bottom-color: #4b5563;
    color: #ffffff;
  }
  
  .card-table-container td {
    border-bottom-color: #374151;
    color: #ffffff;
  }
  
  .card-table-container tr:hover {
    background-color: rgba(55, 65, 81, 0.6);
  }
  
  .card-table-container code {
    background-color: rgba(55, 65, 81, 0.8);
    color: #93c5fd;
  }
}

/* Manual dark mode class support (for frameworks like Tailwind) */
.dark details {
  background-color: rgba(31, 41, 55, 0.8);
  border-color: #374151;
}

.dark details summary {
  color: #ffffff;
}

.dark details[open] summary {
  border-bottom-color: #0033A0;
  color: #ffffff;
}

.dark .copyable-card:hover {
  background-color: rgba(55, 65, 81, 0.8);
}

.dark .copyable-card:active {
  background-color: rgba(75, 85, 99, 0.8);
}

.dark .card-table-container table {
  color: #ffffff;
}

.dark .card-table-container th {
  background-color: rgba(55, 65, 81, 0.8);
  border-bottom-color: #4b5563;
  color: #ffffff;
}

.dark .card-table-container td {
  border-bottom-color: #374151;
  color: #ffffff;
}

.dark .card-table-container tr:hover {
  background-color: rgba(55, 65, 81, 0.6);
}

.dark .card-table-container code {
  background-color: rgba(55, 65, 81, 0.8);
  color: #93c5fd;
}

details summary {
  cursor: pointer;
  font-size: 1.1rem;
  padding: 0.5rem;
  user-select: none;
  transition: all 0.2s ease;
}

details summary:hover {
  background-color: #eff6ff;
  border-radius: 4px;
}

details[open] summary {
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #3b82f6;
}

.copyable-card {
  cursor: pointer;
  transition: all 0.2s ease;
  display: inline-block;
}

.copyable-card:hover {
  background-color: #eff6ff;
  border-radius: 4px;
  padding: 2px 4px;
  transform: scale(1.02);
}

.copyable-card:active {
  background-color: #dbeafe;
}
</style>

<script>
// Agregar feedback visual al copiar
document.querySelectorAll('.copyable-card').forEach(el => {
  el.addEventListener('click', function() {
    const originalText = this.innerHTML;
    this.innerHTML = originalText.replace('', '✅');
    setTimeout(() => {
      this.innerHTML = originalText;
    }, 1000);
  });
});
</script>

## Códigos postales disponibles para prueba de AVS

Para realizar un proceso exitoso usa 55555 como código postal

ZIP Code | Comportamiento
---------|----------
55555 | Retorna transacción aprobada con AVS exitoso (Y)
44444 | Retorna transacción aprobada con AVS fallido (A) y reembolsar la transacción
33333 | Retorna transacción aprobada con AVS fallido (A) rechaza el reembolso, pero cuando se consulta el reembolso fue exitoso.

## OTP para casos de prueba

Para que el proceso de OTP sea exitoso en el proceso de validación de OTP de estos servicios, cualquier otro código es un rechazo

* 123456
* 000000

## OTP en 3DS

Cuando la autenticación de 3DS requira challenge (OTP) el código aceptado es **12345**