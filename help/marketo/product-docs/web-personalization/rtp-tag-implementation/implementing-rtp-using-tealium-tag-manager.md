---
unique-page-id: 9437340
description: Obtenga información acerca de la implementación de rtp con el administrador de etiquetas de telio en Marketo Engage, incluida la implementación de rtp con dnl. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP mediante Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
TQID: https://experienceleague.adobe.com/zMs2Dii5RERdH8tKb86a6EhxXUx2IpbZkDOCklUvvY4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 233
ht-degree: 3%

---

# Implementar RTP utilizando el Administrador de etiquetas [!DNL Tealium] {#implementing-rtp-using-tealium-tag-manager}

Para implementar su etiqueta RTP, siga las instrucciones de instalación a continuación.

1. Inicie sesión en su cuenta de [!DNL Tealium] Tag Manager.

1. Vaya a la pestaña [!UICONTROL Etiquetas] y agregue la etiqueta de contenedor personalizada [!UICONTROL Tealium], que se encuentra en la pestaña [!UICONTROL Misc] del mercado de etiquetas.

1. En el campo [!UICONTROL Título], escriba **Marketo RTP** y haga clic en **[!UICONTROL Finalizar]**.

1. Guarde los cambios.

   >[!NOTE]
   >
   >Aún no es necesario publicar el nuevo contenedor.

1. Una vez guardado el perfil, haga clic en su nombre/dirección de correo electrónico en la esquina superior derecha de la consola de Tealium iQ.

1. En el menú [!UICONTROL Administrador], haga clic en **[!UICONTROL Administrar plantillas]** en [!UICONTROL Administrador de cuentas].

1. Seleccione **[!UICONTROL Contenedor personalizado Tealium]: Marketo RTP** de la lista desplegable para abrir la plantilla de etiqueta.

1. Inicie sesión en su cuenta de RTP.

1. Vaya a [!UICONTROL Configuración de la cuenta].

   >[!NOTE]
   >
   >Si ya ha recibido su etiqueta JavaScript del equipo de asistencia, continúe con el paso 11.

1. En Dominio, busque el dominio correspondiente y haga clic en **[!UICONTROL Generar etiqueta]**.

1. Copie la etiqueta JavaScript de RTP y péguela entre [!UICONTROL Start Tag Library Code] y [!UICONTROL End Tag Library Code] en su plantilla de perfil de Tealium.

   >[!NOTE]
   >
   >**Pasos importantes**
   >
   >Quite las etiquetas `<!-- RTP tag -->` y `<!-- End of RTP tag -->` del código que coloque en este archivo.
   >
   >Elimine las etiquetas `<script type='text/javascript'>` y `</script>` del código que coloque en este archivo.

1. Haga clic en **[!UICONTROL Guardar plantilla de perfil]** y publique su nuevo perfil.
