---
unique-page-id: 10094576
description: 'Baja duradera: Documentos de Marketo: Documentación del producto'
title: Baja duradera
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Baja duradera {#durable-unsubscribe}

Marketo ha mejorado el comportamiento de la funcionalidad de cancelación de suscripción para que sea &quot;duradera&quot;. Se ha añadido un estado de correo electrónico principal, independiente del indicador de cancelación de suscripción visible en el registro de detalles de la persona.

Si el indicador de cancelación de suscripción se establece de false a true, el estado del correo electrónico maestro se actualiza y el cambio se propaga a otras personas con la misma dirección de correo electrónico. Si se elimina y se vuelve a crear una persona, o si se crea un nuevo registro con la misma dirección de correo electrónico, el indicador de cancelación de suscripción **not** sobrescribirse.

>[!NOTE]
>
>La cancelación de la suscripción duradera funciona en todas las particiones de toda la base de datos de Marketo.

## Actualizar el indicador de cancelación de suscripción de Verdadero a Falso (por ejemplo, Volver a suscribir a una Persona) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Existen varias formas de volver a suscribirse a una persona.

En Salesforce, **clear** el campo Exclusión de correo electrónico en el registro del posible cliente o contacto. Esto se sincronizará con Marketo.

![](assets/one.png)

En Marketo, **clear** la casilla cancelar suscripción de la ficha Información del registro de la persona.

![](assets/two.png)

Ejecute un **Cambiar valor de datos** paso de flujo como se muestra a continuación en una o varias personas.

![](assets/three.png)

Actualizar una persona existente a través de la API SOAP.

## Creación de una nueva persona {#creating-a-new-person}

Cuando se crea una nueva persona, Marketo la comprueba según la tabla de estado del correo electrónico maestro. Si la persona se ha dado de baja anteriormente, actualizaremos el registro para cancelar la suscripción.

## Cambio de una dirección de correo electrónico {#changing-an-email-address}

Si cambia la dirección de correo electrónico de una persona a una dirección de correo electrónico que cancela la suscripción, dicha persona se cancelará la suscripción. Este cambio puede producirse en Marketo o en Salesforce.

Si cambia una dirección de correo electrónico sin suscripción a una que está suscrita, esa persona se suscribirá.

## Volver a suscribirse {#re-subscribing}

De la misma manera que una cancelación de la suscripción haría que todas las personas con la misma dirección de correo electrónico dejaran de suscribirse, una nueva suscripción de hecho volvería a suscribirse a todas las personas con la misma dirección de correo electrónico.

## Registro de actividades {#activity-log}

Definiciones del cambio de valor de datos para _updateLeadEmailStatus_ y _resetLeadEmailStatus_ se encuentra en [este artículo de la comunidad](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Información sobre la cancelación de la suscripción](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
