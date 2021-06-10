---
unique-page-id: 1900573
description: 'Añadir un token del sistema como un vínculo en un mensaje de correo electrónico: Marketo Docs: documentación del producto'
title: Añadir un token del sistema como vínculo en un correo electrónico
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Agregar un token del sistema como un vínculo en un mensaje de correo electrónico {#add-a-system-token-as-a-link-in-an-email}

Puede utilizar estos tokens del sistema para personalizar la posición de los vínculos especiales en los correos electrónicos.

Los siguientes tokens pueden utilizarse como vínculos en un correo electrónico o una plantilla de correo electrónico:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Estos tokens **no** se pueden seleccionar a menos que se encuentre dentro de un vínculo de anclaje. Además, pueden **no** incrustarse en un token My.

A continuación se muestra cómo agregarlas a un correo electrónico:

1. Busque y seleccione su correo electrónico y, a continuación, haga clic en **Editar borrador**.

   ![](assets/one-1.png)

1. Haga doble clic en un área editable.

   ![](assets/two-1.png)

1. Resalte el texto que desea convertir en un vínculo que tenga el token y haga clic en el botón **Insertar/Editar vínculo**.

   ![](assets/three-1.png)

1. Introduzca el token en la URL del vínculo y haga clic en **Insert**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copie/pegue el token que desee: **`{{system.forwardToFriendLink}}`** o **`{{system.unsubscribeLink}}`** o **`{{system.viewAsWebpageLink}}`**

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Si utiliza este método para agregar el token del sistema &quot;viewAsWebpageLink&quot;, puede **no** anularlo con tokens. En su lugar, utilice el método [Add a View as Web Page Link to an Email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) que le permite anular el &quot;viewAsWebPageLink&quot; con tokens.

>[!NOTE]
>
>No olvide [aprobar su correo electrónico](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) cuando termine.

¡Bien hecho! Ahora sabe cómo añadir un token del sistema como vínculo en un correo electrónico.
