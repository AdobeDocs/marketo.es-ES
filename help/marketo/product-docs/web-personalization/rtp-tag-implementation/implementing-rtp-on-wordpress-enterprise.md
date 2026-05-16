---
unique-page-id: 4720215
description: Obtenga información acerca de la implementación de rtp en wordpress enterprise en Marketo Engage, incluida la implementación de rtp en wordpress. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP en Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 120
ht-degree: 10%

---

# Implementación de RTP en Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar su [!UICONTROL etiqueta RTP], siga las instrucciones de instalación a continuación:

1. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, siga con el paso 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. En [!UICONTROL Dominio], busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie la etiqueta RTP JavaScript.

1. Inicie sesión en su cuenta de [!DNL WordPress] como usuario administrador

   a. En **[!UICONTROL Aspecto]**, vaya a **[!UICONTROL JavaScript personalizado]**.
b. Pegue la etiqueta JavaScript de RTP justo después del código existente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Cuando pegue el código, EXCLUYA las siguientes etiquetas:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Inserte la secuencia de comandos SOLAMENTE.

1. Haga clic en **[!UICONTROL Actualizar]**.
