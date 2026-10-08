---
unique-page-id: 1147340
description: Obtenga información sobre cómo enviar correos electrónicos desde la dirección del propietario del posible cliente. Utilice la opción Enviar del propietario del posible cliente para que los correos electrónicos muestren el remitente correcto.
title: Envío de correos electrónicos del propietario del posible cliente
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/iOBonqrup6ZV9QGhW-i1FpabLVBOKrNxz4xqThcexZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 6%
---
# Envío de correos electrónicos del propietario del posible cliente {#send-emails-from-the-lead-owner}

¿Qué sucede si desea enviar un correo electrónico a un posible cliente en nombre del propietario?  Así es cómo se hace.

1. Busque el correo electrónico, selecciónelo y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/one.png)

1. Haga clic en el campo **[!UICONTROL De]** (elimine cualquier nombre existente) y luego haga clic en el botón **Insertar token**.

   ![](assets/two.png)

1. Empiece a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Introduzca un valor predeterminado en el caso de que el posible cliente aún no tenga un propietario y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Haga clic después del primer token, agregue un espacio y, a continuación, haga clic en el botón **Insertar token**.

   ![](assets/five.png)

1. Empiece a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Introduzca un valor predeterminado en el caso de que el posible cliente aún no tenga un propietario y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Asegúrese de haber agregado un espacio entre los tokens de nombre y apellido.

1. Haga clic en el campo **[!UICONTROL Dirección desde]** (elimine cualquier dirección de correo electrónico existente) y luego haga clic en el botón **Insertar token**.

   ![](assets/eight.png)

1. Empiece a escribir &quot;`{{lead.Lead Owner`&quot; y seleccione el token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Introduzca un valor predeterminado en el caso de que el posible cliente aún no tenga un propietario y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/ten.png)

1. Asegúrese de que los campos **[!UICONTROL Responder a]** y **[!UICONTROL Asunto]** estén rellenados y que ha finalizado.

   ![](assets/eleven.png)
