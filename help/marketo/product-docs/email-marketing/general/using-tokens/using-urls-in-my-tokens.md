---
unique-page-id: 11382535
description: Aprenda a utilizar direcciones URL en Mis tokens. Almacene y haga referencia a direcciones URL en tokens para vínculos y páginas de aterrizaje en correos electrónicos.
title: Uso de los URL en Mis tókenes
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
TQID: https://experienceleague.adobe.com/d7nzJcfEeJutTNuo95NXcT1eTQXBdNZJoEq5-BdTxs0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 4%

---

# Uso de los URL en Mis tókenes {#using-urls-in-my-tokens}

Siga los pasos a continuación para usar [!UICONTROL Mis tokens] para insertar direcciones URL en sus correos electrónicos.

1. Seleccione su programa y haga clic en **[!UICONTROL Mis tokens]**.

   ![](assets/one-4.png)

1. Seleccione el **[!UICONTROL Texto]** Mi token, arrástrelo y suéltelo en el lienzo.

   ![](assets/two-4.png)

1. Asigne un nombre único al token, escriba una dirección URL (sin el https://) y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**Usando http/https...**
   >
   >* Para asegurarse de que se hace un seguimiento de los clics en el correo electrónico, haga que **no** escriba https:// _en_ el valor del token. Utilícelo fuera del token, como se muestra en el paso 7.
   >
   >* Recomendamos encarecidamente no dejar fuera el http/https. Si lo hace, la [versión web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} de su correo electrónico podría procesarse incorrectamente.

1. Seleccione el correo electrónico en el programa.

   ![](assets/four-3.png)

1. Haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/five-3.png)

1. Haga doble clic en el área de texto para editarla.

   ![](assets/six-1.png)

1. En cualquier parte del correo electrónico, escriba `https://` (sin dejar espacio después) y haga clic en el icono Insertar token.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Por supuesto, también tiene la opción de ingresar `http://` si su sitio no utiliza https.

1. Busque mi token, selecciónelo y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/eight.png)

1. Resalte el https:// y el token y, a continuación, pulse Ctrl/Cmd+X (Ctrl = Windows/Cmd = Mac) para cortar el texto.

   ![](assets/nine.png)

1. Resalte el texto que desee que muestre el vínculo y haga clic en el icono [!UICONTROL Insertar/Editar vínculo].

   ![](assets/ten.png)

1. Presione Ctrl/Cmd+V para pegar el contenido en el cuadro **[!UICONTROL URL]** y haga clic en **[!UICONTROL Insertar]**.

   ![](assets/eleven.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/twelve.png)

   ¡Y has terminado! La dirección URL se rellenará después del envío y, gracias a que pone https:// delante del token, se generará un vínculo al que se puede realizar un seguimiento.
