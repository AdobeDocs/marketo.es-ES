---
unique-page-id: 4720215
description: Obtenga información acerca de la implementación de rtp en wordpress enterprise en Marketo Engage, incluida la implementación de rtp en wordpress. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP en Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '120'
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
b. Pegue la etiqueta Javascript RTP justo después del código existente.

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
