---
unique-page-id: 2953373
description: Obtenga información sobre cómo configurar los pies de página para cancelar la suscripción en Marketo Sales Insight. Configure los vínculos de cancelación de suscripción y el cumplimiento para los correos electrónicos de ventas.
title: Configuración de los pies de página de cancelación de suscripción en Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/9HUCspCSN2LZQzpNJhCI3yiMVzwOYMxyp06UDJQyT2Y
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 210
ht-degree: 4%

---

# Configurar pies de página para cancelar la suscripción en [!DNL Marketo Sales Insight] {#configure-unsubscribe-footers-in-marketo-sales-insight}

Los correos electrónicos de ventas sitúan automáticamente el pie de página de cancelación de suscripción en la parte inferior. Sin embargo, puede ajustar la configuración para satisfacer sus necesidades.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!NOTE]
>
>**Definición**
>
>**Correos electrónicos de ventas** son los enviados desde [!DNL Sales Insight] (no incluye los enviados desde el complemento de Outlook de Marketo).

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/one-1.png)

1. Haga clic en **[!UICONTROL Insight de ventas]** y luego en **[!UICONTROL Editar configuración]**.

   ![](assets/two-1.png)

   Hay varias opciones. Primero vamos a echar un vistazo a los tipos de correos electrónicos para los que puede cambiar la configuración.

   ![](assets/three-1.png)

   * **[!UICONTROL Sin plantilla]** - Compuesto manualmente por el usuario de ventas.
   * **[!UICONTROL Correo electrónico estándar]**: correos electrónicos basados en una plantilla.
   * **[!UICONTROL Correo electrónico operativo]**: Correos electrónicos que omiten los límites de cancelación de suscripción, marketing suspendido y comunicaciones (se envían independientemente de qué).

   Tiene la opción de establecer un comportamiento diferente para cada tipo.

   >[!CAUTION]
   >
   >**[!UICONTROL Respetar la configuración de cancelación de suscripción]**: los posibles clientes no suscritos NO recibirán el correo electrónico aunque el correo electrónico publicado esté &quot;operativo&quot;
   >
   >**[!UICONTROL Ignorar configuración de cancelación de suscripción]**: los posibles clientes no suscritos recibirán el correo electrónico

1. Realice los cambios que desee y haga clic en **[!UICONTROL Guardar]**.

   >[!TIP]
   >
   >Las dos últimas opciones permiten incluir o excluir dinámicamente el pie de página de cancelación de suscripción en función del número de destinatarios (mayor que 1 o mayor que 5).

   ![](assets/four-1.png)

¡Uy! Un poco complicado, pero bastante flexible, ¿verdad?
