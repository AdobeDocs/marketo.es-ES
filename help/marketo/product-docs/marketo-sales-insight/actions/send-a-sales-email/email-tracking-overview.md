---
description: Información general sobre el seguimiento de correo electrónico - Documentos de Marketo - Documentación del producto
title: Información general sobre el seguimiento de correo electrónico
hide: true
hidefromtoc: true
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Información general sobre el seguimiento de correo electrónico {#email-tracking-overview}

## Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que está en cada correo electrónico que envía. Cada correo electrónico contiene un ID de mensaje único que nos permite tener uno de los mejores seguimientos de respuestas.

>[!PREREQUISITES]
>
>Conexión con el servidor de correo electrónico: Sales Connect debe estar conectado a su bandeja de entrada para saber cuándo ha llegado una nueva respuesta. Necesitará tener la cuenta de Conexión de Ventas conectada a Gmail. Si utiliza Outlook, tendremos que integrarlo con su servidor de intercambio.

Si Sales Connect no puede rastrear la respuesta del cliente potencial a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas o en el registro de que responde a Salesforce. ¿Qué queremos decir con cualquier dirección de correo electrónico que pueda responder?

Esto significa que si envía un correo electrónico a flynn@flynnsarcade.com y responde con kevinf@flynnsarcade.com, podemos rastrear la respuesta. Además, si envía un correo electrónico a flynn@flynnsarcade.com y a CC alan@encom.com, y Alan le reescribe, también detectará la respuesta y finalizará la campaña.

## Cómo rastrear los archivos adjuntos de correo electrónico {#how-to-track-your-email-attachments}

Sales Connect ofrece un seguimiento de los archivos adjuntos (.doc, .ppt, .pdf) para que pueda ver cuándo se han abierto o descargado y qué páginas está buscando el destinatario. Le permitiremos utilizar nuestra función de archivos adjuntos rastreables desde ambos [aplicación web](https://toutapp.com/login) y Gmail (o aplicaciones de Google).

>[!NOTE]
>
>El seguimiento de archivos adjuntos solo está disponible para nuestros planes de equipo (a partir de nuestro plan g3startup).

**Cómo enviar el primer archivo adjunto rastreable**

1. Redacte un correo electrónico o edite una plantilla y, a continuación, haga clic en el botón **Contenido** botón.

1. Cargue el archivo adjunto y envíelo. Admitimos PDF, documentos de Word y presentaciones de PowerPoint.

1. Select **Añadir a correo electrónico**.

1. Haga clic en **Enviar** y activa tu fuente de lanzamiento. Verá los destinatarios a medida que se abren y se desplazan por sus archivos adjuntos.

>[!TIP]
>
>Si no desea rastrear un archivo adjunto, simplemente haga clic en Adjuntar archivos y este archivo adjunto no se rastreará.

## Cómo funciona el seguimiento de vista {#how-view-tracking-works}

Para rastrear las aperturas de correo electrónico, colocamos una imagen invisible dentro de los correos electrónicos que envía.

Si alguien responde a su correo electrónico pero Sales Connect dice que no se ha visto, es probable que el destinatario no haya activado las imágenes en su cliente de correo electrónico (es decir, haga clic en el mensaje &quot;haga clic aquí para descargar imágenes&quot; del correo electrónico).

Algunas sugerencias para obtener mejores estadísticas de seguimiento en los correos electrónicos:

* Incluya una imagen en los correos electrónicos (como un logotipo) para que se anime al destinatario a que active las imágenes para ver el mensaje.
* Incluya un vínculo como llamada a la acción en el correo electrónico.

## Probar correo electrónico no mostrado como visto {#test-email-not-showed-as-viewed}

Aunque hayas enviado tu mensaje a otra dirección de correo electrónico, no te registraremos viendo ningún correo electrónico que te hayas enviado en la fuente en directo. Nuestro seguimiento se basa en dispositivos; siempre que utilice un equipo con el que haya iniciado sesión en Conexión de ventas, filtraremos esa actividad.

¿La razón? Sales Connect es inteligente y nuestros usuarios activos nunca nos perdonarían si su propia información apareciera en la actividad de la fuente en directo cada vez que miraban un correo electrónico que enviaban.
