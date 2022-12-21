---
unique-page-id: 7514918
description: 'Información sobre la cancelación de la suscripción: Documentos de Marketo: Documentación del producto'
title: Información sobre la cancelación de la suscripción
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 2%

---

# Información sobre la cancelación de la suscripción {#understanding-unsubscribe}

En realidad, hay varios tipos diferentes de cancelaciones de suscripción integradas en Marketo. Todos están representados por campos en el objeto person, como First Name.

>[!NOTE]
>
>Marketo está cambiando términos como Lista negra y Lista blanca a Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, es posible que vea los términos antiguos en nuestra interfaz de usuario y en las capturas de pantalla de la documentación, así como los términos nuevos en nuestro texto de documentación. Pedimos disculpas por cualquier confusión.

Todos estos campos están integrados en la suscripción a Marketo. Todos son de tipo booleano (casilla de verificación). Pueden utilizarse en Forms o [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) pasos de flujo.

## Suscripción cancelada {#unsubscribed}

Se utiliza en la página estándar de cancelación de suscripción. Si una persona marca esta casilla o hace clic en el vínculo de cancelación de suscripción en un correo electrónico, ya no recibirá correos electrónicos de marketing. Sin embargo, recibirán [correos electrónicos operativos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing suspendido {#marketing-suspended}

El usuario define este campo para colocar a las personas en una cancelación temporal de la suscripción. Las personas solo pueden obtener este estado si se cambian manualmente o si se utiliza un paso para cambiar el flujo de valor de los datos.

## Email suspendido {#email-suspended}

Este estado bloquea los envíos de correo de una persona durante 24 horas después de que se produzca un rechazo grave. Después de 24 horas, la persona volverá a ser enviada.

>[!NOTE]
>
>Correo electrónico suspendido permanecerá seleccionado aunque termine el periodo de 24 horas, por lo que puede hacer referencia a las personas que históricamente han sido marcadas como tales. Para ver si la persona es enviable, simplemente calcule 24 horas después del momento de la suspensión del correo electrónico.

## Está en la lista de bloqueos {#blocklisted}

[Utilice esto para personas como competidores](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Cualquiera que desee recibir **no** correos electrónicos: operativos, de marketing, etc. ¡No reciben nada!

![](assets/image2015-5-18-12-3a6-3a40.png)
