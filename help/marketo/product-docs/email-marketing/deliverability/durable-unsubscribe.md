---
unique-page-id: 10094576
description: Cancelación duradera de la suscripción - Documentos de marketing - Documentación del producto
title: Cancelación de suscripción duradera
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Cancelación de suscripción duradera {#durable-unsubscribe}

Marketing ha mejorado el comportamiento de la funcionalidad de cancelación de suscripción para que sea &quot;duradera&quot;. Hemos agregado un estado de correo electrónico principal, que es independiente del indicador de cancelación de suscripción visible en el registro de detalles de la persona.

Si el indicador de cancelación de suscripción se establece de false a true, el estado del correo electrónico maestro se actualiza y el cambio se propaga a otras personas con la misma dirección de correo electrónico. Si se elimina y se vuelve a crear una persona, o si se crea un nuevo registro con la misma dirección de correo electrónico, el indicador de cancelación de suscripción **no se sobrescribirá** .

>[!NOTE]
>
>La anulación de suscripción duradera funciona en todas las particiones de toda la base de datos de Marketing.

## Actualizar el indicador de cancelación de suscripción de True a False (por ejemplo, volver a suscribir a una persona) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Hay varias formas de volver a suscribirse a una persona.

En Salesforce, **desactive** el campo Exclusión correo electrónico en el registro del posible cliente o contacto. Esto se sincronizará con Marketing.

![](assets/one.png)

En Marketing, **desactive** el cuadro sin suscribir en la ficha Información del registro de la persona.

![](assets/two.png)

Ejecute un paso para **cambiar el valor** de los datos como se muestra a continuación en una o varias personas.

![](assets/three.png)

Actualice una persona existente mediante la API de SOAP.

## Creación de una nueva persona {#creating-a-new-person}

Cuando se crea una nueva persona, el usuario de Marketing la compara con la tabla de estado del correo electrónico principal. Si la persona ya no estaba suscrita, actualizaremos el registro para cancelar la suscripción.

## Cambio de una dirección de correo electrónico {#changing-an-email-address}

Si cambia la dirección de correo electrónico de una persona a una dirección de correo electrónico no suscrita, esa persona dejará de estar suscrita. Este cambio puede producirse en Marketing o en Salesforce.

Si cambia una dirección de correo electrónico sin suscribir a una que esté suscrita, esa persona se suscribirá.

## Nueva suscripción {#re-subscribing}

De la misma manera que una cancelación de suscripción haría que todas las personas con la misma dirección de correo electrónico dejaran de estar suscritas, una nueva suscripción de hecho podría volver a suscribirse a todas las personas con la misma dirección de correo electrónico.

## Registro de actividades {#activity-log}

Valor de los datos Las definiciones de cambio para *updateLeadEmailStatus* y *resetLeadEmailStatus* se encuentran en [este artículo](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)de la comunidad.

>[!NOTE]
>
>**Artículos relacionados**
>
>[Explicación de la cancelación de suscripción](understanding-unsubscribe.md)

