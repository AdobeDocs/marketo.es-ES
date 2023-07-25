---
unique-page-id: 1900573
description: 'Adición de un token de sistema como vínculo en un correo electrónico: documentos de Marketo, documentación del producto'
title: Añadir un token de sistema como vínculo en un correo electrónico
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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
>Estos tokens **no** se puede seleccionar a menos que se encuentre dentro de un vínculo de anclaje. Además, pueden **no** estar incrustado en un My Token.

A continuación se indica cómo añadirlos a un correo electrónico:

1. Busque y seleccione su correo electrónico y, a continuación, haga clic en **Editar borrador**.

   ![](assets/one-1.png)

1. Haga doble clic en un área editable.

   ![](assets/two-1.png)

1. Resalte el texto que desee convertir en un vínculo que tenga el token y haga clic en el **Insertar/editar vínculo** botón.

   ![](assets/three-1.png)

1. Introduzca el token en Link URL y haga clic en **Insertar**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copie o pegue el token que desee: **`{{system.forwardToFriendLink}}`** o **`{{system.unsubscribeLink}}`** o **`{{system.viewAsWebpageLink}}`**

1. Clic **Guardar**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Si utiliza este método para agregar el token del sistema &quot;viewAsWebpageLink&quot;, puede **no** reemplácelo con tokens. En su lugar utilice [Añadir un vínculo de Ver como página web a un correo electrónico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) que permite sobrescribir &quot;viewAsWebPageLink&quot; mediante tokens.

>[!NOTE]
>
>No te olvides de [aprobar el correo electrónico](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) cuando termine.

¡Bien hecho! Ahora sabe cómo agregar un token de sistema como vínculo en un correo electrónico.
