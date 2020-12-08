---
unique-page-id: 2360253
description: Editar el mensaje "Vista como página web" - Documentos de marketing - Documentación del producto
title: Editar el mensaje "Vista como página web"
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Editar el mensaje &quot;Vista como página web&quot; {#edit-the-view-as-web-page-message}

Si necesita editar el texto &quot; [Vista como página](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)web&quot;, así es como.

>[!NOTE]
>
>**Se requieren permisos de administración**

## Editar el mensaje &quot;Vista como página web&quot; {#edit-the-view-as-web-page-message-1}

1. En **Administración**, haga clic en **Correo electrónico**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Las siguientes variables son críticas. ¡No los elimine!
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK#
   >    
   >    
   >La segunda parte ##MKT_TOK## es la cookie munchkin de esa persona. Se asegura de que se les recopile correctamente al hacer clic en el vínculo.

1. Edite la **Vista como HTML** de página web y **Vista como texto de página web **versiones a su gusto y haga clic en **Guardar cambios**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Asegúrese de evitar:
>
>* Añadir direcciones URL adicionales a cualquiera de los cuadros HTML
>* Colocación de HTML en la versión de texto

>



Ahí lo tienes. Envíe mensajes de correo electrónico de prueba para garantizar el formato.

## Texto predeterminado de &quot;Vista como página web&quot; {#default-view-as-web-page-text}

Si alguna vez necesita volver a la &quot;Vista como página Web&quot; predeterminada del sistema, copie o pegue lo siguiente:

**Vista como HTML de página web:**
`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **Vista como texto de página web:**

Para vista este correo electrónico como página web, vaya a la siguiente dirección:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` ¡Boom! Has terminado.
