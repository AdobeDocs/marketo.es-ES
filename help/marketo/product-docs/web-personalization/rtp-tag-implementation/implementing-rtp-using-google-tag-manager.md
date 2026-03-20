---
unique-page-id: 4720145
description: Obtenga información acerca de la implementación de RTP con google tag Manager en Marketo Engage, incluida la implementación de RTP con DNL Google. Utilice esta guía para completar el siguiente paso.
title: Implementación de RTP mediante Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '165'
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

   a. Puede hacerlo haciendo clic con el botón derecho en la página del sitio web. Vaya a **[!UICONTROL Inspeccionar elemento]**, busque **RTP** para localizar la etiqueta.
