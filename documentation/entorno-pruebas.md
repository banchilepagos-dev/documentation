---
title: 'Cómo Integrarse y Pasar a Producción'
description: 'Para integrarse y pasar a producción debes tener en cuenta los ambientes disponibles en cada etapa'
slug: 'como-integrarse-produccion-web-checkout'
order: 2
---

## Prueba tu integración
Debes iniciar tu integración en nuestro ambiente de pruebas y cuando todo esté en orden pasarte al ambiente de productivo.

## URLs de Checkout

| Modo       | URL                                         |
|------------|---------------------------------------------|
| Pruebas    | https://checkout.test.banchilepagos.cl             |
| Producción | https://checkout.banchilepagos.cl                  |

## Números de tarjeta de pruebas

Es importante definir que estas tarjetas solo tienen dicho comportamiento en el ambiente de pruebas

En todos los casos excepto donde se especifique el CVV y la fecha de expiración puede ser cualquiera con tal de que sea vigente para que su comportamiento aplique.

Para las pruebas con 3DS en el comportamiento se describe su resultado

- Y: Autenticado sin fricción
- C: Solicita autenticación con Fricción (Desafío)
- D: Autenticación Desacoplada
- A: Intento de Autenticación
- N: No autenticado


<h1 class="icos-visa">VISA</h1>

| Número              | Comportamiento                                                                              |
|---------------------|---------------------------------------------------------------------------------------------|
| 4110760000000081    | Aprueba                                                                                      |
| 4110770010002837    | Aprueba                                                                                      |
| 4381080000000029    | Aprueba                                                                                      |
| 4111111111111111    | Aprueba 3DS-Y                                                                                |
| 4110760000000008    | Aprueba 3DS-C                                                                                |
| 4110760000000016    | Rechaza                                                                                      |
| 4005580000000040    | Rechaza                                                                                      |
| 4716375184092180    | Rechaza                                                                                      |
| 4381080000000011    | Rechaza                                                                                      |
| 4716375184092180    | Rechaza                                                                                      |
| 4110760000000032    | Deja la transacción en estado pendiente y se resuelve a aprobado 3DS-C                       |
| 4110760000000040    | Deja la transacción en estado pendiente y se resuelve a rechazado 3DS-A                      |
| 4048370000000037    | Deja la transacción en estado pendiente y se resuelve a rechazado                            |
| 4110760000000073    | Deja la transacción en estado pendiente y se resuelve a aprobado                             |
| 4110760000000065    | Arroja una excepción en el proceso 3DS-N                                                     |
| 4110760000000024    | Se tarda 180 segundos en responder y queda en estado aprobado                                |
| 4110760000000115    | Se tarda 180 segundos en responder y queda en estado rechazado                               |
| 4110760000000057    | Aprueba si el monto es inferior a 200USD de lo contrario rechaza                            |
| 4012888888881881    | Aprueba si se proporciona la expiración 11/28 y el cvv 917 de lo contrario rechaza           |
| 4381080000000003    | Deja la transacción en estado pendiente y se resuelve a rechazado                            |
| 4509564638437551    | Deja la transacción en estado pendiente y se resuelve a aprobado                             |
| 4864921336824366    | Deja la transacción en estado pendiente y se resuelve a rechazado                            |
| 4931974429847108    | Deja la transacción en estado pendiente y se resuelve a rechazado                            |
| 4532034637206853    | Deja la transacción en procesamiento manual y si se procesa queda en estado rechazado         |
| 4666666666666669    | Se tarda 180 segundos en responder y queda en estado aprobado  

## Mastercard
| Número              | Comportamiento                                                        |
|---------------------|-----------------------------------------------------------------------|
| 5367680000000005    | Aprueba                                                               |
| 5180300000000005    | Aprueba 3DS-Y                                                         |
| 5292594382060745    | Aprueba 3DS-C                                                         |
| 5367680000000013    | Rechaza                                                               |
| 5180300000000039    | Rechaza 3DS-N                                                         |
| 5180300000000047    | Deja la transacción en estado pendiente y se resuelve a aprobado 3DS-C |
| 5180300000000054    | Deja la transacción en estado pendiente y se resuelve a rechazado 3DS-A|


## Códigos postales disponibles para prueba de AVS
**Para realizar un proceso exitoso usa 55555 como código postal**
| ZIP Code | Comportamiento                                                                            |
|----------|-------------------------------------------------------------------------------------------|
| 55555    | Retorna transacción aprobada con AVS exitoso (Y)                                          |
| 44444    | Retorna transacción aprobada con AVS fallido (A) y reembolsar la transacción              |
| 33333    | Retorna transacción aprobada con AVS fallido (A) rechaza el reembolso, pero cuando se consulta el reembolso fue exitoso. |


## OTP para casos de prueba

**Para que el proceso de OTP sea exitoso en el proceso de validación de OTP de estos servicios, cualquier otro código es un rechazo**

- 123456
- 000000
