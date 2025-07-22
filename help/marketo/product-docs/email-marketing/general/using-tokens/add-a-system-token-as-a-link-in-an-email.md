---
unique-page-id: 1900573
description: 'Adición de un token de sistema como vínculo en un correo electrónico: documentos de Marketo, documentación del producto'
title: Añadir un token de sistema como vínculo en un correo electrónico
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Añadir un token de sistema como vínculo en un correo electrónico {#add-a-system-token-as-a-link-in-an-email}

Puede utilizar estos tokens del sistema para personalizar la posición de los vínculos especiales en los correos electrónicos.

Los siguientes tokens se pueden utilizar como vínculos en un correo electrónico o una plantilla de correo electrónico:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Se podrá hacer clic en estos tokens **no** a menos que se encuentren dentro de un vínculo de anclaje. Además, **no** pueden incrustarse en un token My.

A continuación se indica cómo añadirlos a un correo electrónico:

1. Busque y seleccione su correo electrónico, luego haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/one-1.png)

1. Haga doble clic en un área editable.

   ![](assets/two-1.png)

1. Resalte el texto que desee convertir en un vínculo que tendrá el token y haga clic en el botón **[!UICONTROL Insertar/Editar vínculo]**.

   ![](assets/three-1.png)

1. Escriba el token en la URL del vínculo y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copie o pegue el token que desee: **`{{system.forwardToFriendLink}}`**, **`{{system.unsubscribeLink}}`** o **`{{system.viewAsWebpageLink}}`**

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Si usa este método para agregar el token del sistema &quot;viewAsWebpageLink&quot;, puede **no** anularlo con tokens. En su lugar, use el método [Agregar una vista como vínculo de página web a un correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md), que le permite invalidar &quot;viewAsWebPageLink&quot; mediante tokens.

>[!NOTE]
>
>No olvides [aprobar el correo electrónico](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) cuando hayas terminado.

¡Bien hecho! Ahora sabe cómo agregar un token de sistema como vínculo en un correo electrónico.
