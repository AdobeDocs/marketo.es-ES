---
unique-page-id: 2360251
description: Editar el mensaje de cancelación de suscripciones - Documentos de marketing - Documentación del producto
title: Editar el mensaje de cancelación de suscripción
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Editar el mensaje de cancelación de suscripción {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Se requieren permisos de administración**

Al enviar correos electrónicos de marketing (no [operativos](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), el texto de cancelación de suscripción y los vínculos se anexan a la parte inferior. Puede cambiar los valores predeterminados. Así es como.

## Editar el mensaje de cancelación de suscripción {#edit-the-unsubscribe-message-1}

1. En **Administración**, haga clic en **Correo electrónico**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >Las siguientes variables son críticas. ¡No los elimine!
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscription=1&amp;mkt_tok=##MKT_TOK#**


1. Edite las versiones **Cancelar suscripción de HTML** y **Cancelar suscripción de texto** a su gusto y haga clic en **Guardar cambios**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Ahí lo tienes. **¡Asegúrate de probar!** No desea que sus correos electrónicos de marketing hayan roto los vínculos de cancelación de suscripciones.

>[!TIP]
>
>Puede personalizar la posición del HTML de cancelación de suscripción en el correo electrónico mediante [tokens](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texto predeterminado de cancelación de suscripción {#default-unsubscribe-text}

Si alguna vez necesita volver a la cancelación de suscripción predeterminada del sistema, copie/pegue lo siguiente:

Cancelar suscripción de HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Cancelar suscripción de texto:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Editar el mensaje &quot;Vista como página web&quot;](edit-the-view-as-web-page-message.md)

>



