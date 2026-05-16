---
unique-page-id: 2360251
description: Cambie el texto predeterminado de cancelación de suscripción y los vínculos adjuntos a los correos electrónicos de marketing en Correo electrónico del administrador.
title: Editar el mensaje de cancelación de suscripción
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
TQID: https://experienceleague.adobe.com/2wAcUvsELVvNhk0HpdNdkWJLopFn3IC4X-lUSQlCs5Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 140
ht-degree: 9%

---

# Editar el mensaje de cancelación de suscripción {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Cuando envía correos electrónicos de marketing (que no son [operativos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), el texto de cancelación de suscripción y los vínculos se anexan a la parte inferior. Puede cambiar los valores predeterminados.

## Dónde realizar la edición {#where-to-make-the-edit}

1. Vaya a la sección **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Las siguientes variables son críticas. ¡No los borre!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Edite las versiones de **[!UICONTROL Cancelar suscripción a HTML]** y **[!UICONTROL Cancelar suscripción a texto]** a su gusto y haga clic en **[!UICONTROL Guardar cambios]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

>[!TIP]
>
>* Recuerde hacer la prueba. No quiere que sus correos electrónicos de marketing tengan vínculos de cancelación de suscripción rotos.
>
>* Puede personalizar la posición del HTML de cancelación de suscripción en su correo electrónico mediante [tokens](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texto predeterminado de cancelación de suscripción {#default-unsubscribe-text}

Si alguna vez necesita volver al mensaje predeterminado de cancelación de suscripción del sistema, copie/pegue lo siguiente:

[!UICONTROL Cancelar suscripción a HTML]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>`
<br>
[!UICONTROL Cancelar la suscripción del texto]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Editar el mensaje &quot;Ver como página web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
