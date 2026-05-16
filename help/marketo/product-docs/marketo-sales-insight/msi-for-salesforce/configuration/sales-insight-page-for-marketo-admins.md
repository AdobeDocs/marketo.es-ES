---
unique-page-id: 42762409
description: Obtenga información acerca de la página Insight de ventas para administradores de Marketo. Configuración de acciones de acceso y configuración de MSI.
title: Página de Insight de ventas para administradores de Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/FTOgWRDvY14tovIUclyWrED5DBXcHXH8APcprG-DlK4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 416
ht-degree: 3%

---

# [!DNL Sales Insight] página para administradores de Marketo {#sales-insight-page-for-marketo-admins}

Los administradores de Marketo tienen ciertos privilegios en [!DNL Sales Insight]. Descubra cuáles son a continuación.

## Configuración de API de SOAP {#soap-api-configuration}

Estas credenciales se usan para conectar su cuenta de [!DNL Salesforce] a su instancia de Marketo para usar MSI en [!DNL Salesforce].

![](assets/one-1.png)

## Configuración de API de REST {#rest-api-configuration}

Estas credenciales se usan para conectar su cuenta de [!DNL Salesforce] a su instancia de Marketo, con el fin de usar el panel de información de MSI en [!DNL Salesforce].

![](assets/two-1.png)

## Configuración de puntuación de persona {#person-score-settings}

* **[!UICONTROL Estrellas]**: Las estrellas representan la puntuación total del posible cliente en comparación con otros posibles clientes.
* **[!UICONTROL Llamas]**: Las llamas representan urgencia, cuánto ha cambiado recientemente la puntuación de un posible cliente.

De manera predeterminada, [!DNL Marketo Sales Insight] usa el campo Puntuación de posibles clientes para calcular las estrellas y las llamas. Pero si desea elegir un campo diferente, así es como:

1. En el área **[!UICONTROL Administrador]** de Marketo, haga clic en **[!UICONTROL Insight de ventas]**.

   ![](assets/four.png)

1. En [!UICONTROL Configuración de puntuación de posibles clientes], haga clic en **[!UICONTROL Editar]**.

   ![](assets/five.png)

1. Seleccione el campo que desee utilizar para las estrellas.

   ![](assets/six.png)

1. Seleccione el campo que desee utilizar para las llamas.

   ![](assets/seven.png)

1. Haga clic en **[!UICONTROL Guardar]**. Sales insight tardará algún tiempo en volver a calcular. Puede comprobar su CRM más tarde para ver las estrellas y las llamas.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Si aún no tienes tus campos de puntuación personalizados, así es como [crearlos](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Estrellas y llamas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Configuración {#settings}

![](assets/nine.png)

**Configuración de cancelación de suscripción:**

Puede elegir la siguiente configuración para cancelar la suscripción a [!UICONTROL Sin plantilla], [!UICONTROL correos electrónicos estándar] y [!UICONTROL correos electrónicos operativos]

* [!UICONTROL Respetar configuración de cancelación de suscripción]
* [!UICONTROL Respetar configuración de cancelación de suscripción cuando más de 1 destinatario]
* [!UICONTROL Respetar la configuración de cancelación de suscripción cuando más de 5 destinatarios]
* [!UICONTROL Omitir configuración de cancelación de suscripción]

**Habilitar la capacidad para bloquear plantillas:**

Cuando se habilita, los usuarios de MSI no podrán editar las plantillas al enviar correos electrónicos desde [!DNL Salesforce]

**Habilitar fuente RSS:**

Cuando está habilitada, los usuarios de MSI pueden ver su fuente de posibles clientes en una fuente RSS (además de la fuente de posibles clientes de [!DNL Salesforce]). La fuente RSS solo puede funcionar si la característica &quot;[!UICONTROL Caducidad del token]&quot; está deshabilitada.

**Caducidad del token:**

La caducidad del token se controla en el Administrador de funciones. Para habilitarlo o deshabilitarlo, comuníquese con [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Cuando se habilita, todos los tokens de Marketo caducan en un plazo de 10 minutos. Cuando está desactivado, los tokens de Marketo no caducan.

Los tokens generados antes de habilitar la caducidad del token no tendrán una hora de caducidad con la que validarse, por lo que no caducarán aunque la función esté habilitada actualmente.

Los tokens generados después de habilitar la caducidad del token tendrán un tiempo de caducidad de 10 minutos, por lo que caducarán en 10 minutos incluso después de que la función esté deshabilitada.

El comportamiento del token se basará en el momento en que se generó (cuando la función de caducidad del token estaba habilitada/deshabilitada, en lugar de su estado actual).
