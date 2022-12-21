---
unique-page-id: 14352540
description: Prevención de autovistas - Documentos de Marketo - Documentación del producto
title: Prevención de autovistas
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Prevención de autovistas {#preventing-self-views}

## Resumen {#overview}

Obtener falsos positivos en el seguimiento de vista puede provocar incoherencias en los informes. Esto suele ocurrir cuando los usuarios de MSC invocan accidentalmente el píxel de seguimiento de su cliente de correo electrónico (lo llamamos vista automática). A continuación se ofrecen algunos consejos para reducir e incluso eliminar las opiniones personales de forma significativa.

## Web (Outlook Web App y Gmail) {#web-outlook-web-app-and-gmail}

Sales Connect almacenará una cookie en el explorador para evitar que se rastreen las vistas al abrir los correos electrónicos de Outlook Web App y Gmail. Si sigue recibiendo autovistas, le recomendamos que haga lo siguiente:

* Asegúrese de tener habilitadas las cookies en su equipo.

* Si utiliza un equipo o dispositivo móvil nuevo, asegúrese de haber iniciado sesión en la aplicación web. Esto nos permitirá reconocer el equipo/dispositivo a partir de ahora.

## Escritorio (Windows) {#desktop-windows}

Las vistas se rastrean descargando un pequeño píxel de imagen invisible en su cliente de correo electrónico. Puede reducir significativamente la cantidad de autovistas en Outlook desactivando las imágenes para que se descarguen automáticamente. A continuación se muestran los pasos de cómo.

1. En Outlook, haga clic en **Archivo** en la barra de menús.

   ![](assets/win-1.png)

1. Haga clic en **Opciones**.

   ![](assets/win-2.png)

1. En el cuadro de diálogo Opciones de Outlook, haga clic en **Centro de confianza**.

   ![](assets/win-3.png)

1. En el Centro de confianza de Microsoft Outlook, haga clic en **Configuración del centro de confianza**.

   ![](assets/win-4.png)

1. Haga clic en Descarga automática en el menú de la izquierda y seleccione la opción **No descargue imágenes automáticamente en el correo electrónico del HTML o en los elementos RSS** en el Navegador.

   ![](assets/win-5.png)

1. Haga clic en **OK** en el cuadro de diálogo Centro de confianza.

   ![](assets/win-6.png)

1. Haga clic en **OK** en el cuadro de diálogo Opciones de Outlook.

   ![](assets/win-6.png)

## Escritorio (Mac) {#desktop-mac}

Las vistas se rastrean descargando un pequeño píxel de imagen invisible en su cliente de correo electrónico. Puede reducir significativamente la cantidad de autovistas en Outlook desactivando las imágenes para que se descarguen automáticamente. A continuación se muestran los pasos de cómo.

1. En Outlook, haga clic en **Outlook** en la barra de menús y seleccione **Preferencias**.

   ![](assets/mac-1.png)

1. En Correo electrónico, elija **Lectura**.

   ![](assets/mac-2.png)

1. En Seguridad, haga clic en la **Nunca** botón de opción.

   ![](assets/mac-3.png)
