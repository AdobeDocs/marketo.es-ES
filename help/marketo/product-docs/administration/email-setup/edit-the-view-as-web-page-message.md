---
unique-page-id: 2360253
description: 'Editar el mensaje "Ver como página web": Documentos de Marketo: Documentación del producto'
title: Editar el mensaje "Ver como página web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Editar el mensaje &quot;Ver como página web&quot; {#edit-the-view-as-web-page-message}

Si necesita editar el &quot;[Ver como una página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot; texto, así es como.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Editar el mensaje &quot;Ver como página web&quot; {#edit-the-view-as-web-page-message-1}

1. Vaya a la **Administrador** .

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Las siguientes variables son críticas. ¡No los borres!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Segunda parte `##MKT_TOK##` es la cookie munchkin de esa persona. Se asegura de que se les recopile correctamente al hacer clic en el vínculo.

1. Edite el **Ver como HTML de página web** y **Ver como texto de página web** versiones a su gusto y haga clic en **Guardar cambios**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Asegúrese de evitar:
>
>* Adición de direcciones URL adicionales a cualquiera de los cuadros de HTML
>* Incluir HTML en la versión de texto


Ahí lo tienes. Envíe correos electrónicos de prueba para garantizar el formato.

## Texto predeterminado &quot;Ver como página web&quot; {#default-view-as-web-page-text}

Si alguna vez necesita volver al sistema predeterminado &quot;Ver como página web&quot;, copie/pegue lo siguiente:

**Ver como HTML de página web:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Ver como texto de página web:**

Para ver este correo electrónico como una página web, vaya a la siguiente dirección:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

¡Eso es todo!
