---
unique-page-id: 7514918
description: Explicación de la cancelación de la suscripción - Documentos de marketing - Documentación del producto
title: Explicación de la cancelación de suscripción
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Explicación de la cancelación de suscripciones {#understanding-unsubscribe}

En realidad hay varios tipos diferentes de cancelaciones integradas en Marketing. Todos están representados por campos en el objeto de persona, como Nombre.

>[!NOTE]
>
>Marketing está en proceso de cambiar términos como Lista negra y Lista blanca a Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, puede ver los términos antiguos en nuestra interfaz de usuario y en las capturas de pantalla de documentación, así como los nuevos términos en el texto de la documentación. Pedimos disculpas por cualquier confusión.

Todos estos campos están integrados en la suscripción de marketing. Todos son de tipo booleano (casilla de verificación). Pueden utilizarse en pasos de flujo de Forms o [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Suscrito {#unsubscribed}

Se utiliza en la página de cancelación de suscripción estándar. Si una persona marca esta casilla o hace clic en el vínculo de cancelación de suscripción en un mensaje de correo electrónico, ya no recibirá correos electrónicos de marketing. Sin embargo, recibirán [correos electrónicos operativos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Mercadotecnia suspendida {#marketing-suspended}

Este campo lo define el usuario para colocar personas en una cancelación temporal de suscripción. Las personas solo pueden obtener este estado si se modifican manualmente o si se utiliza un paso para cambiar el flujo del valor de los datos.

## Correo electrónico suspendido {#email-suspended}

Este estado bloquea el envío de correo de una persona durante 24 horas después de que se produzca una devolución forzada. Después de 24 horas, la persona volverá a ser enviada.

>[!NOTE]
>
>El correo electrónico suspendido se seguirá comprobando incluso después de que haya finalizado el período de 24 horas, por lo que puede referirse a personas que históricamente han sido marcadas como tales. Para ver si la persona puede enviarse por correo, basta con calcular 24 horas después del momento de la suspensión del correo electrónico.

## Incluido en la lista de bloqueados {#blocklisted}

[Usa esto para personas como competidoras](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Cualquiera que desee recibir **correos electrónicos no**: operacionales, de mercadotecnia, etc. ¡No tienen nada!

![](assets/image2015-5-18-12-3a6-3a40.png)
