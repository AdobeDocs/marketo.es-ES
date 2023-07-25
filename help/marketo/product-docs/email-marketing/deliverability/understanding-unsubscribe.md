---
unique-page-id: 7514918
description: Conceptos básicos de cancelación de suscripción - Documentos de Marketo - Documentación del producto
title: Explicación de cancelación de suscripción
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 2%

---

# Explicación de cancelación de suscripción {#understanding-unsubscribe}

En realidad, hay varios tipos diferentes de cancelaciones de suscripción integradas en Marketo. Todos se representan mediante campos en el objeto de persona, como Nombre.

>[!NOTE]
>
>Marketo está cambiando términos como Lista negra y Lista blanca por Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, es posible que vea los términos antiguos en nuestras capturas de pantalla de la interfaz de usuario y la documentación, y los nuevos términos en nuestro texto de documentación. Pedimos disculpas por cualquier confusión.

Todos estos campos están incorporados en la suscripción a Marketo. Todos son de tipo booleano (casilla de verificación). Pueden utilizarse en Forms o [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) pasos de flujo.

## Suscripción cancelada {#unsubscribed}

Se utiliza en la página de cancelación de suscripción estándar. Si una persona marca esta casilla o hace clic en el vínculo de cancelación de suscripción de un correo electrónico, ya no recibirá correos electrónicos de marketing. Sin embargo, recibirán [correos electrónicos operativos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing suspendido {#marketing-suspended}

El usuario establece este campo para colocar a las personas en una cancelación de suscripción temporal. Las personas solo pueden obtener este estado si se cambian manualmente o si se utiliza un paso de flujo de valor de datos de cambio.

## Email suspendido {#email-suspended}

Este estado impide que una persona envíe correos durante 24 horas después de que se produzca una devolución grave. Después de 24 horas, la persona volverá a recibir el correo.

>[!NOTE]
>
>Los mensajes de correo electrónico suspendidos permanecerán marcados incluso después de que termine el periodo de 24 horas, por lo que puede hacer referencia a personas que históricamente han sido marcadas como tales. Para ver si la persona puede recibir correo, simplemente calcule 24 horas después del momento de la suspensión del correo electrónico.

## Está en la lista de bloqueos {#blocklisted}

[Utilícelo para personas como la competencia](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Cualquiera que desee recibir **no** correos electrónicos: operativos, de marketing, etc. ¡No reciben nada!

![](assets/image2015-5-18-12-3a6-3a40.png)
