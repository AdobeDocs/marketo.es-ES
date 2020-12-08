---
unique-page-id: 1147356
description: Explicación del registro de Eventos de correo electrónico - Documentos de marketing - Documentación del producto
title: Explicación del registro de Eventos de correo electrónico
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


# Explicación del registro de Eventos de correo electrónico {#understanding-email-event-logging}

Al enviar mensajes de correo electrónico, Marketo registra diferentes puntos de datos en los registros de actividad de la persona. Aquí están los básicos.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

| Evento | Descripción |
|---|---|
| Enviado | Se registra cada vez que se envía un mensaje de correo electrónico desde los servidores de marketing, independientemente de si se ha enviado realmente. Los correos electrónicos devueltos siguen registrándose como &quot;Enviados&quot;. |
| Enviado | Se registra cada vez que el servidor de correo de destinatario acepta un correo electrónico. Esto no significa que evite filtros de spam. Sólo puede haber 1 envío por cada correo electrónico enviado. |
| Devuelto | Algunas devoluciones duras son el resultado de bloqueos de spam, por lo que no trataremos de enviar un correo electrónico a esa persona durante 24 horas en ninguna campaña. Otros rebotes duros como las bandejas de entrada inexistentes son permanentes, y nunca volveremos a enviar correos electrónicos a la persona desde ninguna campaña. |
| Suave devuelta | Se registra cuando una respuesta del servidor no está clara, hay problemas con el buzón de correo o con el servidor en general. Ponemos a estas personas a través de una lógica de reintentos durante 24-36 horas para un posible envío futuro. Esto no descalifica a la persona de otros envíos. |
| Abierto | Se registra cuando un destinatario vista un correo electrónico con imágenes NO bloqueadas. Solo se registra un evento abierto por correo electrónico, por persona y por campaña inteligente. Si abren el mismo correo electrónico desde su bandeja de entrada dos veces, no se registrará más de una vez. |
| Clic | Se registra cada vez que se carga una dirección URL decorada del correo electrónico en el explorador (el resultado es hacer clic en el vínculo). Generalmente es el destinatario que hace clic, pero también puede ser un corte/pegado. |
| No suscrito | Se registra cuando una persona hace clic en el vínculo de cancelación de suscripción de un correo electrónico y envía el formulario de cancelación de suscripción. |

>[!CAUTION]
>
>Si el mismo correo electrónico se envía dos veces a la misma persona desde la misma campaña, el evento **Abierto** se registrará un máximo de 1 vez.

