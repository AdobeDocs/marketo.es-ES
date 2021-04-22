---
unique-page-id: 2360253
description: 'Editar el mensaje "Ver como página web": Documentos de Marketo: Documentación del producto'
title: Editar el mensaje "Ver como página web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Editar el mensaje &quot;Ver como página web&quot; {#edit-the-view-as-web-page-message}

Si necesita editar el texto &quot;[View as a Webpage](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, así es como.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Editar el mensaje &quot;Ver como página web&quot; {#edit-the-view-as-web-page-message-1}

1. En **Administración**, haga clic en **Correo electrónico**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Las siguientes variables son críticas. ¡No los borres!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La segunda parte `##MKT_TOK##` es la cookie munchkin de esa persona. Se asegura de que se les recopile correctamente al hacer clic en el vínculo.

1. Edite las versiones **View as Web Page HTML** y **View as Web Page Text** a su gusto y haga clic en **Save Changes**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Asegúrese de evitar:
>
>* Adición de direcciones URL adicionales a cualquiera de los cuadros HTML
>* Incluir HTML en la versión de texto


Ahí lo tienes. Envíe correos electrónicos de prueba para garantizar el formato.

## Texto predeterminado &quot;Ver como página web&quot; {#default-view-as-web-page-text}

Si alguna vez necesita volver al sistema predeterminado &quot;Ver como página web&quot;, copie/pegue lo siguiente:

**Ver como HTML de página web:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Ver como texto de página web:**

Para ver este correo electrónico como una página web, vaya a la siguiente dirección:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` ¡Boom! Ya has terminado.
