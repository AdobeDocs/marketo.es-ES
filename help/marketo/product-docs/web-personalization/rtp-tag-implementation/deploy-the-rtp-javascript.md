---
unique-page-id: 4719332
description: Obtenga información acerca de la implementación del javascript rtp en Marketo Engage, incluida la implementación del javascript rtp. Utilice esta guía para completar el siguiente paso.
title: Implementación de JavaScript RTP
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XUylNa8clUib-aMhpAR8fjeu4pHRA8KSQydSH1AVxF8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 4%

---

# Implementación de JavaScript RTP {#deploy-the-rtp-javascript}

Para generar y configurar su etiqueta RTP, siga las instrucciones de instalación que se indican a continuación

## [!UICONTROL Generar etiqueta] {#generate-tag}

1. Inicie sesión en su cuenta de RTP. Vaya a **[!UICONTROL Configuración de la cuenta]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. En **[!UICONTROL Dominio]** y **[!UICONTROL Configuración del dominio]**, busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copie y pegue la etiqueta Web Personalization (RTP) en el sitio web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie la etiqueta RTP JavaScript y péguela como el primer script en el encabezado de sus páginas, entre las etiquetas `<head> </head>`.

   Asegúrese de que la etiqueta aparece en todas las páginas, incluidas las páginas de aterrizaje y los subdominios. Para comprobarlo, haga clic con el botón derecho en la página del sitio web. Vaya a Ver Source de página en un explorador web. Buscar: &quot;RTP&quot;.

1. [!UICONTROL Etiqueta] se cambió a **[!UICONTROL ON]**.

   Confirme que la opción [!UICONTROL Tag] está establecida en [!UICONTROL ON]. Debería empezar a ver el flujo de datos en la pestaña de la organización.

   Ya está configurado con la etiqueta RTP y listo para empezar a [crear segmentos](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) y campañas en tiempo real.

1. Compruebe que la etiqueta está en todas las páginas.
