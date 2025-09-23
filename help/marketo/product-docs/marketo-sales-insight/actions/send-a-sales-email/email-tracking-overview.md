---
description: Información general sobre el seguimiento de correo electrónico - Documentos de Marketo - Documentación del producto
title: Información general de seguimiento de correo electrónico
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# Información general de seguimiento de correo electrónico {#email-tracking-overview}

## Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que hay en cada correo electrónico que envía. Cada correo electrónico contiene un ID de mensaje único que nos permite tener algunos de los mejores resultados de seguimiento de respuestas.

>[!PREREQUISITES]
>
>Conexión con el servidor de correo electrónico: [!DNL Sales Connect] debe estar conectado con su bandeja de entrada para que sepamos cuándo ha llegado una nueva respuesta. Necesitarás tener tu cuenta de [!DNL Sales Connect] conectada a Gmail. Si utiliza Outlook, tendremos que integrarlo con su servidor de Exchange.

Si [!DNL Sales Connect] no puede rastrear la respuesta de su posible cliente a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas ni registrar esa respuesta en Salesforce. ¿Qué significa que cualquier dirección de correo electrónico puede responder?

Esto significa que si envía un correo electrónico a <flynn@flynnsarcade.com> y él responde con <kevinf@flynnsarcade.com>, podremos realizar un seguimiento de la respuesta. Además, si envía un correo electrónico a <flynn@flynnsarcade.com> y CC <alan@encom.com>, y Alan le devuelve una respuesta, también detectará la respuesta y finalizará la campaña.

## Cómo seguir los archivos adjuntos del correo electrónico {#how-to-track-your-email-attachments}

[!DNL Sales Connect] ofrece seguimiento en los archivos adjuntos (.doc, .ppt, .pdf) para que pueda ver cuándo se han abierto o descargado y qué páginas está viendo el destinatario. Le permitiremos usar nuestra función de archivos adjuntos rastreables desde la [aplicación web](https://toutapp.com/login) y Gmail (o aplicaciones de Google).

>[!NOTE]
>
>El seguimiento de archivos adjuntos solo está disponible para nuestros planes de equipo (a partir de nuestro plan de inicio g3).

**Cómo enviar su primer archivo adjunto rastreable**

1. Escribe un correo electrónico o edita una plantilla y, a continuación, haz clic en el botón **[!UICONTROL Contenido]**.

1. Cargue el archivo adjunto y envíelo. Se admiten PDF, [!DNL Word] documentos y [!DNL Powerpoint] presentaciones.

1. Seleccione **[!UICONTROL Agregar al correo electrónico]**.

1. Haz clic en **[!UICONTROL Enviar]** y activa tu Live Feed. Verá sus destinatarios a medida que abran y pasen página a través de los archivos adjuntos.

>[!TIP]
>
>Si no desea rastrear un archivo adjunto, simplemente haga clic en Adjuntar archivos y no se rastreará este archivo adjunto.

## Cómo funciona el seguimiento de visitas {#how-view-tracking-works}

Rastreamos las aperturas de correos electrónicos colocando una imagen invisible dentro de los correos electrónicos que envía.

Si alguien responde a su correo electrónico pero [!DNL Sales Connect] dice que no se vio, es probable que el destinatario no habilitara imágenes dentro de su cliente de correo electrónico (por ejemplo, haga clic en el mensaje &quot;haga clic aquí para descargar imágenes&quot; del correo electrónico).

Algunas sugerencias para obtener mejores estadísticas de seguimiento en los correos electrónicos:

* Incluya una imagen en los correos electrónicos (como un logotipo) para animar al destinatario a permitir que las imágenes vean el mensaje.
* Incluya un vínculo como call to action en el correo electrónico.

## Probar correo electrónico no mostrado como visto {#test-email-not-showed-as-viewed}

Incluso si ha enviado el mensaje a otra dirección de correo electrónico, no registraremos su visualización de los correos electrónicos que se haya enviado a sí mismo en la fuente en directo. Nuestro seguimiento se basa en dispositivos. Siempre y cuando esté usando un equipo con el cual haya iniciado sesión en [!DNL Sales Connect], filtraremos esa actividad.

¿La razón? [!DNL Sales Connect] es inteligente y los usuarios activos nunca nos perdonarían si apareciera su propia información en la actividad de fuente en directo cada vez que miran un correo electrónico que han enviado.
