---
unique-page-id: 1147340
description: Envío de correos electrónicos del propietario del posible cliente - Documentos de Marketo - Documentación del producto
title: Envío de correos electrónicos del propietario del posible cliente
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Envío de correos electrónicos del propietario del posible cliente {#send-emails-from-the-lead-owner}

¿Qué sucede si desea enviar un correo electrónico a un posible cliente en nombre del propietario?  Así es como.

1. Busque el correo electrónico, selecciónelo y haga clic en **Editar borrador**.

   ![](assets/one.png)

1. Haga clic en el campo **De** (elimine cualquier nombre existente) y luego haga clic en el botón **Insertar token**.

   ![](assets/two.png)

1. Empiece a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Introduzca un valor predeterminado en el caso de que el posible cliente aún no tenga un propietario y haga clic en **Insertar**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Haga clic después del primer token, agregue un espacio y, a continuación, haga clic en el botón **Insertar token**.

   ![](assets/five.png)

1. Empiece a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Introduzca un valor predeterminado en el caso de que el posible cliente aún no tenga un propietario y haga clic en **Insertar**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Asegúrese de haber agregado un espacio entre los tokens de nombre y apellido.

1. Haga clic en el campo De correo electrónico (elimine cualquier dirección de correo electrónico existente) y haga clic en el botón Insertar token.

   ![](assets/eight.png)

1. Empiece a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Introduzca un valor predeterminado en el caso de que el posible cliente aún no tenga un propietario y haga clic en **Insertar**.

   ![](assets/ten.png)

1. Asegúrese de que los campos **Responder a** y **Asunto** estén rellenados y listo.

   ![](assets/eleven.png)
