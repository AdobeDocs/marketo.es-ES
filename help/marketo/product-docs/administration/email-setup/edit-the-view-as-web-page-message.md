---
unique-page-id: 2360253
description: Personalice el texto Ver como vínculo de página web y HTML en Correo electrónico del administrador mientras mantiene intactas las variables requeridas.
title: Editar el mensaje “Ver como página web”
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
TQID: https://experienceleague.adobe.com/mREJHheKv7c16atJ17pv8S9ZGUoLnD8jd5jyk6QtgR8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 24%

---

# Editar el mensaje “Ver como página web” {#edit-the-view-as-web-page-message}

Aprenda a editar el texto &quot;[Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Editar el mensaje “Ver como página web” {#edit-the-view-as-web-page-message-1}

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Las siguientes variables son críticas. ¡No los borre!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La segunda parte `##MKT_TOK##` es la cookie [!UICONTROL Munchkin] de esa persona. Garantiza que se realice un seguimiento adecuado cuando haga clic en el vínculo.

1. Edite las versiones de **[!UICONTROL Ver como página web HTML]** y **[!UICONTROL Ver como página web Text]** a su gusto y haga clic en **[!UICONTROL Guardar cambios]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Asegúrese de evitar:
>
>* Añadir direcciones URL adicionales a cualquiera de los cuadros de HTML
>* Incluir HTML en la versión de texto

Envíe correos electrónicos de prueba para verificar el formato.

## Texto predeterminado de &quot;Ver como página web&quot; {#default-view-as-web-page-text}

Si alguna vez necesita volver al sistema predeterminado &quot;[!UICONTROL Ver como página web]&quot;, copie y pegue lo siguiente:

**[!UICONTROL Ver como HTML de página web]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL Ver como texto de página web]**:

Para ver este correo electrónico como una página web, vaya a la siguiente dirección:
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
