---
unique-page-id: 1147340
description: Enviar correos electrónicos del propietario principal - Documentos de marketing - Documentación del producto
title: Enviar correos electrónicos del propietario del posible cliente
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Enviar correos electrónicos del propietario del posible cliente {#send-emails-from-the-lead-owner}

¿Qué sucede si desea enviar un correo electrónico a un posible cliente en nombre del propietario del posible cliente?  Así es como.

1. Busque su correo electrónico, selecciónelo y haga clic en **Editar borrador**.

   ![](assets/one.png)

1. Haga clic en el campo **De** (elimine cualquier nombre existente) y haga clic en el botón **Insertar token**.

   ![](assets/two.png)

1. Escriba el inicio &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Escriba un valor predeterminado en caso de que el posible cliente aún no tenga un propietario de posible cliente y haga clic en **Insertar**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Haga clic después del primer token, agregue un espacio y, a continuación, haga clic en el botón **Insertar token**.

   ![](assets/five.png)

1. Escriba el inicio &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Escriba un valor predeterminado en caso de que el posible cliente aún no tenga un propietario de posible cliente y haga clic en **Insertar**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Asegúrese de agregar un espacio entre los tokens de nombre y de apellido.

1. Haga clic en el campo Desde correo electrónico (elimine cualquier dirección de correo electrónico existente) y haga clic en el botón Insertar token.

   ![](assets/eight.png)

1. Escriba el inicio &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Escriba un valor predeterminado en caso de que el posible cliente aún no tenga un propietario de posible cliente y haga clic en **Insertar**.

   ![](assets/ten.png)

1. Asegúrese de que los campos **Responder a** y **Asunto** están rellenados y ya ha terminado.

   ![](assets/eleven.png)
