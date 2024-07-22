---
unique-page-id: 10094576
description: 'Cancelación de suscripción duradera: documentación de Marketo: documentación del producto'
title: Cancelación de suscripción duradera
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 35f5b33b01462b1cd00e29360daee465c7f18cf0
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Cancelación de suscripción duradera {#durable-unsubscribe}

Marketo ha mejorado el comportamiento de la funcionalidad de cancelación de suscripción para que sea &quot;duradera&quot;. Hemos añadido un estado de correo electrónico principal, que es independiente del indicador de cancelación de suscripción visible en el registro de detalles de la persona.

Si el indicador de cancelación de suscripción se establece de falso a verdadero, el estado del correo electrónico principal se actualiza y el cambio se propaga a otras personas con la misma dirección de correo electrónico. Si se quita una persona y se vuelve a crear, o si se crea un nuevo registro con la misma dirección de correo electrónico, el indicador de cancelación de suscripción **no** se sobrescribirá.

>[!NOTE]
>
>La cancelación de suscripción duradera funciona en todas las particiones de toda la base de datos de Marketo.

## Actualizar el indicador de cancelación de suscripción de Verdadero a Falso (por ejemplo, Volver a suscribir a una persona) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Existen varias formas de volver a suscribir a una persona.

En Salesforce, **borre** el campo Exclusión de correo electrónico en el registro del posible cliente/contacto. Se sincronizará con Marketo.

![](assets/one.png)

En Marketo, **borre** la casilla de cancelación de la suscripción en la ficha Información del registro de la persona.

![](assets/two.png)

Ejecute un paso de flujo de **Cambiar valor de datos** como se muestra a continuación en una o varias personas.

![](assets/three.png)

SOAP Actualizar una persona existente mediante la API de.

## Creación de una nueva persona {#creating-a-new-person}

Cuando se crea una persona nueva, Marketo la compara con la tabla de estado del correo electrónico principal. Si la persona canceló la suscripción anteriormente, actualizaremos el registro para cancelar la suscripción.

## Cambio de una dirección de correo electrónico {#changing-an-email-address}

Si cambia la dirección de correo electrónico de una persona a una dirección de correo electrónico sin suscribirse, se cancela la suscripción de esa persona. Este cambio se puede producir en Marketo o en Salesforce.

Si cambia una dirección de correo electrónico sin suscribir a una que está suscrita, esa persona se suscribirá.

## Volver a suscribirse {#re-subscribing}

Al igual que una cancelación de suscripción haría que todas las personas con la misma dirección de correo electrónico se cancelaran, una nueva suscripción volvería a suscribir a todas las personas con la misma dirección de correo electrónico.

>[!MORELIKETHIS]
>
>[Descripción de la cancelación de suscripción](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
