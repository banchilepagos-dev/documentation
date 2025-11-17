---
title: 'Ciclo de Sesión'
description: 'Proceso para iniciar, gestionar y estados de una sesión de Checkout.'
slug: 'ciclo-sesion'
order: 2
---
## Iniciar Checkout

**Crear una sesión de pago**

Para aceptar un pago a través de Checkout, es necesario crear una sesión de pago (**Checkout Session**) utilizando el método `API - Crear sesión (CreateRequest)`.

Al llamar a este servicio, se obtendrá la URL de proceso (`processUrl`) y el identificador de solicitud (`requestId`).

**Registro del Pago en Proceso**

En tu sistema, crear un registro que relacione el pago en proceso con el `requestID` proporcionado.

El estado inicial de todos los pagos es pendiente (`PENDING`).

**Redirección del Usuario**

El usuario debe ser redireccionado a la URL de proceso (`processUrl`) proporcionada por Banchile Pagos Checkout.

**Proceso de Pago o Suscripción**

En la interfaz de Checkout, el usuario completará el proceso de pago o suscripción. Checkout se encargará de recopilar todos los datos necesarios.

**Redirección de vuelta al sitio del comercio**

Una vez que el proceso de pago esté completo, el usuario puede ser redirigido de vuelta a la URL de retorno (`returnUrl`) especificada en la solicitud inicial (`CreateRequest`).

En este punto es probable que el proceso de pago haya finalizado. Para conocer el estado del pago debes esperar la notificación o consultar el estado de la sesión.

### Notificación asincrónica

Cuando una sesión tenga un estado final, Banchile Pagos enviará una notificación asincrónica a tu sitio informando la finalización del proceso de pago. Asegúrate de manejar adecuadamente esta notificación para mantener la integridad de los datos.

### Consulta de sesiones

Se debe consultar las sesiones para poder completar el ciclo de vida.

**Consulta del estado de la sesión**

Al llegar al sitio del comercio, se debe consultar el estado de la sesión.

Esto se puede lograr utilizando el método `API - Consultar sesión (getRequestInformation)`.

**Actualización y Reglas de Negocio**

Según el estado final del pago obtenido, debes ejecutar las reglas de negocio correspondientes y actualizar la información relacionada con el pago en tu sistema.

## Estados de Sesión

Las sesiones pueden atravesar diferentes estados, cada uno con su propio significado y secuencia de cambios. A continuación, presentamos los estados posibles y cómo se relacionan entre sí:

**`PENDING` Pendiente:** Se presenta en tres situaciones: en primer lugar, es el estado inicial de la sesión e indica que el proceso está en espera de acciones por parte del usuario; en segundo lugar, cuando hay transacciones rechazadas, permitiendo al usuario la oportunidad de realizar nuevos intentos; y, por ultimo, cuando existe una transacción pendiente de validación lo que indica que la sesión se encuentra en un estado de espera hasta que se confirme y valide la transacción. En resumen, es un estado de espera e indica que el proceso no ha finalizado.

**`APPROVED` Aprobado:** Este estado se presenta cuando las transacciones se han aprobado y el proceso se ha completado con éxito. *Este es un estado final de proceso.*

**`REJECTED` Rechazado:** Este estado se presenta cuando la sesión es cancelada por parte del usuario. También puede ocurrir cuando la sesión llega al tiempo de expiración sin un pago aprobado. *Este es un estado final de proceso.*

**`APPROVED_PARTIAL` Aprobado Parcial:** Se presenta en sesiones de pago parcial cuando el usuario ha pagado una parte del monto total solicitado pero otra parte aún está pendiente o ha fallado. En este momento el usuario aún puede completar la totalidad del pago con otras transacciones.

**`PARTIAL_EXPIRED` Parcial Expirado:** Se presenta en sesiones de pago parcial cuando el usuario solo pagó una parte del monto total solicitado y el tiempo disponible para completar el pago ya ha finalizado. En este momento el proceso ya ha finalizado y no se puede completar. *Este es un estado final de proceso.*

### Estados en sesiones

![image.png](Documentación%20Web%20Checkout%2026a3784920f880f5ab09dc65a61c2622/image%201.png)
