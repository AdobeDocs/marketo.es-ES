---
unique-page-id: 7514918
description: Obtenga información sobre los tipos de cancelación de suscripción en Marketo (Cancelada la suscripción, Marketing suspendido, Incluido en la lista de bloqueados). Utilice el campo correcto para cada escenario de sus campañas.
title: Explicación de cancelación de suscripción
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
TQID: https://experienceleague.adobe.com/zmsCI3a7GECVNiuFjtjqgDQsjelBoccugPeuzAF4c4k
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 4%

---

# Explicación de cancelación de suscripción {#understanding-unsubscribe}

Existen varios tipos diferentes de cancelaciones de suscripción integradas en Marketo. Todos se representan mediante campos en el objeto de persona, como Nombre.

Todos estos campos están incorporados en la suscripción a Marketo. Todos son de tipo booleano (casilla de verificación). Se pueden usar en pasos de flujo de Forms o [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Suscripción cancelada {#unsubscribed}

Se utiliza en la página de cancelación de suscripción estándar. Si una persona marca esta casilla o hace clic en el vínculo de cancelación de suscripción de un correo electrónico, ya no recibirá correos electrónicos de marketing. Sin embargo, recibirán [correos electrónicos operativos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing suspendido {#marketing-suspended}

El usuario establece este campo para colocar a las personas en una cancelación de suscripción temporal. Las personas solo pueden obtener este estado si se cambian manualmente o si se utiliza un paso de flujo de valor de datos de cambio.

## Correo electrónico suspendido {#email-suspended}

Este estado impide que una persona envíe correos durante 24 horas después de que se produzca una devolución grave. Después de 24 horas, la persona volverá a recibir el correo.

>[!NOTE]
>
>Los mensajes de correo electrónico suspendidos permanecerán marcados incluso después de que termine el periodo de 24 horas, por lo que puede hacer referencia a personas que históricamente han sido marcadas como tales. Para ver si la persona puede recibir correo, calcule 24 horas después del momento de la suspensión del correo electrónico.

## Incluido en la lista de bloqueados {#blocklisted}

[Use esto para personas como la competencia](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Cualquiera que desee recibir **no** correos electrónicos: operativos, de marketing, etc. No reciben correos electrónicos.

![](assets/image2015-5-18-12-3a6-3a40.png)
