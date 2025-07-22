---
unique-page-id: 9437340
description: 'Implementación de RTP con Tealium Tag Manager: Documentos de Marketo, documentación del producto'
title: Implementación de RTP con Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

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
