---
unique-page-id: 1147340
description: Envío de correos electrónicos desde el propietario potencial - Documentos de Marketo - Documentación del producto
title: Enviar correos electrónicos del propietario del posible cliente
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Enviar correos electrónicos del propietario del posible cliente {#send-emails-from-the-lead-owner}

¿Qué sucede si desea enviar un correo electrónico a un posible cliente en nombre del propietario del posible cliente?  Así es como.

1. Busque su correo electrónico, selecciónelo y haga clic en **Editar borrador**.

   ![](assets/one.png)

1. Haga clic en el **De** (elimine cualquier nombre existente) y haga clic en el botón **Insertar token** botón.

   ![](assets/two.png)

1. Comience a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Introduzca un valor predeterminado en caso de que el posible cliente aún no tenga un propietario de posible cliente y haga clic en **Insertar**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Haga clic después del primer token, añada un espacio y, a continuación, haga clic en el botón **Insertar token** botón.

   ![](assets/five.png)

1. Comience a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Introduzca un valor predeterminado en caso de que el posible cliente aún no tenga un propietario de posible cliente y haga clic en **Insertar**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Asegúrese de que ha añadido un espacio entre los tokens de nombre y apellido.

1. Haga clic en el campo De correo electrónico (elimine cualquier dirección de correo electrónico existente) y haga clic en el botón Insertar token .

   ![](assets/eight.png)

1. Comience a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione **`{{lead.Lead Owner Email Address}}`** token.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Introduzca un valor predeterminado en caso de que el posible cliente aún no tenga un propietario de posible cliente y haga clic en **Insertar**.

   ![](assets/ten.png)

1. Asegúrese de que la variable **Responder** y **Asunto** los campos están rellenados, ¡y ya ha terminado!

   ![](assets/eleven.png)
