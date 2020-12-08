---
unique-page-id: 7514918
description: Explicación de la cancelación de la suscripción - Documentos de marketing - Documentación del producto
title: Explicación de la cancelación de suscripción
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Explicación de la cancelación de suscripción {#understanding-unsubscribe}

En realidad hay varios tipos diferentes de cancelaciones integradas en Marketing. Todos están representados por campos en el objeto de persona, como Nombre.

>[!NOTE]
>
>Marketing está en proceso de cambiar términos como Lista negra y Lista blanca a Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, puede ver los términos antiguos en nuestra interfaz de usuario y en las capturas de pantalla de documentación, así como los nuevos términos en el texto de la documentación. Pedimos disculpas por cualquier confusión.

Todos estos campos están integrados en la suscripción de marketing. Todos son de tipo booleano (casilla de verificación). Se pueden usar en Forms o en los pasos del flujo [Cambiar valor](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) de datos.

## No suscrito {#unsubscribed}

Se utiliza en la página de cancelación de suscripción estándar. Si una persona marca esta casilla o hace clic en el vínculo de cancelación de suscripción en un mensaje de correo electrónico, ya no recibirá correos electrónicos de marketing. Sin embargo, recibirán correos electrónicos [](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)operativos.

## Comercialización suspendida {#marketing-suspended}

Este campo lo define el usuario para colocar personas en una cancelación temporal de suscripción. Las personas solo pueden obtener este estado si se modifican manualmente o si se utiliza un paso para cambiar el flujo del valor de los datos.

## Correo electrónico suspendido {#email-suspended}

Este estado bloquea el envío de correo de una persona durante 24 horas después de que se produzca una devolución forzada. Después de 24 horas, la persona volverá a ser enviada.

>[!NOTE]
>
>El correo electrónico suspendido se seguirá comprobando incluso después de que haya finalizado el período de 24 horas, por lo que puede referirse a personas que históricamente han sido marcadas como tales. Para ver si la persona puede enviarse por correo, basta con calcular 24 horas después del momento de la suspensión del correo electrónico.

## Incluido en la lista de bloqueados {#blocklisted}

[Usa esto para personas como competidoras](http://docs.marketo.com/x/uwOQ). Cualquiera que **no quiera recibir** correos electrónicos: operativos, de marketing, etc. ¡No tienen nada!

![](assets/image2015-5-18-12-3a6-3a40.png)

