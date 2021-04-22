---
unique-page-id: 2360251
description: 'Edición del mensaje de cancelación de la suscripción: documentos de Marketo: documentación del producto'
title: Editar el mensaje de cancelación de suscripción
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Editar el mensaje de cancelación de suscripción {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Al enviar correos electrónicos de marketing (que no sean [operacionales](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), el texto de cancelación de la suscripción y los vínculos se agregan a la parte inferior. Puede cambiar los valores predeterminados. Así es como.

## Editar el mensaje de cancelación de suscripción {#edit-the-unsubscribe-message-1}

1. En **Administración**, haga clic en **Correo electrónico**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >Las siguientes variables son críticas. ¡No los borres!
   >
   >* **%mkt_opt_out_prefix%**
   >* **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK#**


1. Edite las versiones **Unsubscribe HTML** y **Unsubscribe Text** a su gusto y haga clic en **Save Changes**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Ahí lo tienes. _¡Asegúrate de probar!_ No desea que sus correos electrónicos de marketing tengan vínculos de cancelación de suscripción rotos.

>[!TIP]
>
>Puede personalizar la posición del HTML de cancelación de suscripción en su correo electrónico utilizando [tokens](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texto predeterminado para cancelar la suscripción {#default-unsubscribe-text}

Si alguna vez necesita volver a la cancelación de suscripción predeterminada del sistema, copie/pegue lo siguiente:

Cancelar suscripción a HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Cancelar suscripción Texto:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Editar el mensaje &quot;Ver como página web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
