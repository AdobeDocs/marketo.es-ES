---
unique-page-id: 2360301
description: Aprenda a establecer campos de puntuación para estrellas y llamas en Sales Insight. Asigne campos de puntuación de Marketo a la visualización MSI en Salesforce.
title: Establecer los campos de puntuación que se utilizarán para Estrellas y Llamas en Insight de ventas
exl-id: 640f6d53-71ee-4a6d-b28a-82f3825b8f8e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/ShowS2zjGEHvU9BRJNIlX6XdY127funYi-sjsE9YTNU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 169
ht-degree: 10%

---

# Definir los campos de puntuación que se usarán para [!UICONTROL Stars] y [!UICONTROL Flames] en [!DNL Sales Insight] {#set-score-fields-to-be-used-for-stars-and-flames-in-sales-insight}

>[!NOTE]
>
>**Se requieren permisos de administrador**

De manera predeterminada, [!DNL Marketo Sales Insight] usa el campo **[!UICONTROL Puntuación de posibles clientes]** para calcular las estrellas y las llamas. Pero si desea elegir un campo diferente, así es como:

>[!TIP]
>
>Si aún no tienes tus campos de puntuación personalizados, así es como [crearlos](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!NOTE]
>
>**Definición**
>
>* **[!UICONTROL Estrellas]**: Las estrellas representan la puntuación total del posible cliente en comparación con otros posibles clientes.
>* **[!UICONTROL Llamas]**: Las llamas representan la urgencia, cuánto ha cambiado recientemente la puntuación de un posible cliente.
>

1. En **[!UICONTROL Administrador]**, haga clic en **[!UICONTROL Insight de ventas]**.

   ![](assets/image2014-9-16-13-3a27-3a19.png)

1. En **[!UICONTROL Configuración de puntuación de posibles clientes]**, haga clic en **[!UICONTROL Editar]**.

   ![](assets/image2014-9-16-13-3a27-3a33.png)

1. Seleccione el campo que desee usar para **[!UICONTROL Stars]**.

   ![](assets/image2014-9-16-13-3a27-3a45.png)

1. Seleccione el campo que desee usar para **[!UICONTROL Llamas]**.

   ![](assets/image2014-9-16-13-3a28-3a1.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-16-13-3a28-3a18.png)

   >[!NOTE]
   >
   >[!DNL Sales insight] tardará algún tiempo en volver a calcular. Puede comprobar su CRM más tarde para ver las estrellas y las llamas.

   >[!MORELIKETHIS]
   >
   >[Prioridad, urgencia, puntuación relativa y elementos más probables](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
