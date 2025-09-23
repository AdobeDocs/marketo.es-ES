---
unique-page-id: 14352540
description: Prevención de las visualizaciones automáticas - Documentos de Marketo - Documentación del producto
title: Evitar las autovisualizaciones
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 2%

---

# Evitar las autovisualizaciones {#preventing-self-views}

## Información general {#overview}

Obtener falsos positivos en el seguimiento de vistas puede provocar incoherencias en los informes. Esto suele ocurrir cuando los usuarios de MSC invocan accidentalmente el píxel de seguimiento desde su cliente de correo electrónico (lo llamamos vista propia). A continuación se ofrecen algunas sugerencias para reducir significativamente e incluso eliminar las visualizaciones automáticas.

## Web ([!DNL Outlook Web App] y Gmail) {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect] almacenará una cookie en el explorador para evitar que se rastreen las vistas al abrir los correos electrónicos desde Outlook Web App y Gmail. Si sigue recibiendo autovisualizaciones, le recomendamos que haga lo siguiente:

* Asegúrese de que tiene las cookies habilitadas en el equipo.

* Si utiliza un equipo nuevo o un dispositivo móvil, asegúrese de haber iniciado sesión en la aplicación web. Esto nos permitirá reconocer su ordenador/dispositivo a partir de ahora.

## Escritorio (Windows) {#desktop-windows}

Las vistas se rastrean descargando un pequeño píxel de imagen invisible en su cliente de correo electrónico. Puede reducir significativamente la cantidad de visualizaciones automáticas en [!DNL Outlook] si deshabilita las imágenes para que se descarguen automáticamente. A continuación se muestran los pasos para hacerlo.

1. En [!DNL Outlook], haga clic en **[!UICONTROL Archivo]** en la barra de menús.

   ![](assets/win-1.png)

1. Haga clic en **[!UICONTROL Opciones]**.

   ![](assets/win-2.png)

1. En el cuadro de diálogo Opciones de [!DNL Outlook], haga clic en **[!UICONTROL Centro de confianza]**.

   ![](assets/win-3.png)

1. En [!UICONTROL Centro de confianza de Microsoft Outlook], haga clic en **[!UICONTROL Configuración del Centro de confianza]**.

   ![](assets/win-4.png)

1. Haga clic en [!UICONTROL Descarga automática] en el menú de la izquierda y active la casilla de verificación **[!UICONTROL No descargar imágenes automáticamente en elementos de correo electrónico o RSS de HTML]**.

   ![](assets/win-5.png)

1. Haga clic en **[!UICONTROL Aceptar]** en el cuadro de diálogo [!UICONTROL Centro de confianza].

   ![](assets/win-6.png)

1. Haga clic en **[!UICONTROL Aceptar]** en el cuadro de diálogo Opciones de [!DNL Outlook].

   ![](assets/win-6.png)

## Escritorio (Mac) {#desktop-mac}

Las vistas se rastrean descargando un pequeño píxel de imagen invisible en su cliente de correo electrónico. Puede reducir significativamente la cantidad de visualizaciones automáticas en [!DNL Outlook] si deshabilita las imágenes para que se descarguen automáticamente. A continuación se muestran los pasos para hacerlo.

1. En [!DNL Outlook], haga clic en **[!UICONTROL Outlook]** en la barra de menús y seleccione **[!UICONTROL Preferencias]**.

   ![](assets/mac-1.png)

1. En [!UICONTROL Correo electrónico], elija **[!UICONTROL Leyendo]**.

   ![](assets/mac-2.png)

1. En [!UICONTROL Seguridad], haga clic en el botón de opción **[!UICONTROL Nunca]**.

   ![](assets/mac-3.png)
