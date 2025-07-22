---
unique-page-id: 1147356
description: Explicación del registro de eventos de correo electrónico - Documentos de Marketo - Documentación del producto
title: Explicación del registro de eventos de correo electrónico
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Explicación del registro de eventos de correo electrónico {#understanding-email-event-logging}

Al enviar correos electrónicos, Marketo registra diferentes puntos de datos en los registros de actividad de la persona. Aquí están los básicos.

| Evento | Descripción |
|---|---|
| [!UICONTROL Enviado] | Se registra cada vez que se envía un correo electrónico desde los servidores de Marketo, independientemente de si se entrega realmente. Los correos electrónicos rechazados siguen registrándose como &quot;Enviados&quot;. |
| [!UICONTROL Entregado] | Se registra cada vez que el servidor de correo del destinatario acepta un correo electrónico. Esto no significa que se eviten los filtros de correo no deseado. Solo puede haber una entrega por cada correo electrónico enviado. |
| [!UICONTROL Rechazado fuerte] | Algunas devoluciones duras son el resultado de bloques de correo no deseado, por lo que no intentaremos enviar un correo electrónico a esa persona durante 24 horas en ninguna campaña. Otras devoluciones duras como bandejas de entrada inexistentes son permanentes y nunca volveremos a enviar un correo electrónico a la persona desde ninguna campaña. |
| [!UICONTROL Rechazado suave] | Se registra cuando la respuesta del servidor no es clara, el buzón está lleno o hay problemas generales con el servidor. Ponemos a estas personas a través de una lógica de reintentos durante 24-36 horas para un posible envío futuro. Esto no descalifica a la persona de otros envíos. |
| [!UICONTROL Abierto] | Se registra cuando un destinatario ve un correo electrónico con imágenes NO bloqueadas. Solo se registra un evento abierto por correo electrónico, por persona y por campaña inteligente. Si abren el mismo correo electrónico desde su bandeja de entrada dos veces, no se registrará más de una vez. |
| [!UICONTROL Se hizo clic] | Se registra cada vez que se carga una URL representada del correo electrónico en el explorador (resultado de hacer clic en el vínculo). Normalmente, es el clic del destinatario, pero también puede ser un corte o pegado. |
| [!UICONTROL Canceló la suscripción] | Se registra cuando una persona hace clic en el vínculo de cancelación de suscripción de un correo electrónico y envía el formulario de cancelación de suscripción. |

>[!CAUTION]
>
>Si se envía el mismo correo electrónico a la misma persona dos veces desde la misma campaña, el evento **[!UICONTROL Opened]** se registrará una vez como máximo.
