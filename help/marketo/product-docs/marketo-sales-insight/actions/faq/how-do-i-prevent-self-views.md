---
description: ¿Cómo evito las visualizaciones automáticas? - Documentos de Marketo - Documentación del producto
title: ¿Cómo evito las vistas automáticas?
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# ¿Cómo evito las auto-visualizaciones? {#how-do-i-prevent-self-views}

Obtener falsos positivos en el seguimiento de vistas puede provocar incoherencias en los informes. Esto suele ocurrir cuando los usuarios de Marketo Sales invocan accidentalmente el píxel de seguimiento desde su cliente de correo electrónico (lo llamamos &quot;vista propia&quot;). A continuación se ofrecen algunas sugerencias para reducir significativamente e incluso eliminar las visualizaciones automáticas.

## Web (Outlook Web App y Gmail) {#web-outlook-web-app-and-gmail}

Marketo Sales almacenará una cookie en su navegador para evitar que se rastreen las vistas al abrir sus correos electrónicos desde Outlook Web App y Gmail. Si sigue recibiendo autovisualizaciones, le recomendamos que haga lo siguiente:

* Asegúrese de que tiene las cookies habilitadas en el equipo.

* Si utiliza un equipo nuevo o un dispositivo móvil, asegúrese de haber iniciado sesión en la aplicación web. Esto nos permitirá reconocer su ordenador/dispositivo a partir de ahora.

## Escritorio (Windows) {#desktop-windows}

Las vistas se rastrean descargando un pequeño píxel de imagen invisible en su cliente de correo electrónico. Puede reducir considerablemente la cantidad de visualizaciones automáticas en Outlook si deshabilita las imágenes para que se descarguen automáticamente. A continuación se muestran los pasos para hacerlo.

1. En Outlook, haga clic en **Archivo** en la barra de menús.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Haga clic en **Opciones**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. En el cuadro de diálogo Opciones de Outlook, haga clic en **Centro de confianza**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. En el Centro de confianza de Microsoft Outlook, haga clic en **Configuración del Centro de confianza**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Haga clic en Descarga automática en el menú de la izquierda y active la casilla de verificación **No descargar imágenes automáticamente en el correo electrónico del HTML o en los elementos RSS**.

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Haga clic en **Aceptar** en el cuadro de diálogo Centro de confianza.

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Haga clic en **Aceptar** en el cuadro de diálogo Opciones de Outlook.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Escritorio (Mac) {#desktop-mac}

Las vistas se rastrean descargando un pequeño píxel de imagen invisible en su cliente de correo electrónico. Puede reducir considerablemente la cantidad de visualizaciones automáticas en Outlook si deshabilita las imágenes para que se descarguen automáticamente. A continuación se muestran los pasos para hacerlo.

1. En Outlook, haga clic en **Outlook** en la barra de menús y seleccione **Preferencias**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. En Correo electrónico, elija **Leyendo**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. En Seguridad, haga clic en el botón de opción **Nunca**.

   ![](assets/how-do-i-prevent-self-views-10.png)
