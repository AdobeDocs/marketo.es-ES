---
unique-page-id: 4720145
description: Obtenga información acerca de la implementación de RTP con google tag Manager en Marketo Engage, incluida la implementación de RTP con DNL Google. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP mediante Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 3%

---

# Implementando RTP con [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta de [!DNL Google Tag Manager].

1. Agregue una nueva **[!UICONTROL Etiqueta]** > **[!UICONTROL Configuraciones de etiquetas]** > **[!UICONTROL Etiqueta personalizada de HTML].** Llámelo **RTP**.

1. Inicie sesión en su **cuenta RTP**.

1. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   a. Si ya ha recibido la etiqueta JavaScript del equipo de asistencia, continúe con el paso 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. En [!UICONTROL Dominio], busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copie la etiqueta RTP JavaScript y péguela en la nueva **etiqueta HTML personalizada** que creó (paso 1).

1. Haga clic en **[!UICONTROL Agregar regla a la etiqueta Fire]**. Seleccione **[!UICONTROL Todas las páginas]**.

1. Haga clic en **[!UICONTROL Guardar]** y [publicar la nueva versión](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Compruebe que aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios.

   a. Para ello, haga clic con el botón derecho en la página del sitio web. Vaya a **[!UICONTROL Inspeccionar elemento]**, busque **RTP** para localizar la etiqueta.
