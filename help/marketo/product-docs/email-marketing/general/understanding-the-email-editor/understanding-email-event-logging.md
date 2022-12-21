---
unique-page-id: 1147356
description: 'Información sobre el registro de eventos de correo electrónico: Documentos de Marketo: Documentación del producto'
title: Información sobre el registro de eventos de correo electrónico
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 3%

---

# Información sobre el registro de eventos de correo electrónico {#understanding-email-event-logging}

Al enviar correos electrónicos, Marketo registra diferentes puntos de datos en los registros de actividad de la persona. Aquí están los básicos.

| Evento | Descripción |
|---|---|
| Enviado | Se registra cada vez que se envía un correo electrónico desde los servidores de Marketo, independientemente de si realmente se envía. Los correos electrónicos devueltos siguen registrándose como &quot;Enviados&quot;. |
| Entregado | Se registra cada vez que el servidor de correo del destinatario acepta un correo electrónico. Esto no significa que se hayan evitado los filtros de spam. Solo puede haber 1 entrega por cada correo electrónico enviado. |
| Se rechazó permanentemente | Algunos rechazos graves son el resultado de bloques de correo no deseado, por lo que no intentaremos enviar un correo electrónico a esa persona durante 24 horas en ninguna campaña. Otras devoluciones duras como bandejas de entrada inexistentes son permanentes y nunca volveremos a enviar un correo electrónico a la persona desde ninguna campaña. |
| Rechazado leve | Se registra cuando una respuesta del servidor no es clara, el buzón está lleno o hay problemas generales con el servidor. Pasamos a estas personas una lógica de reintentos de 24 a 36 horas para un posible envío futuro. Esto no descalifica a la persona de otros correos. |
| Abierto | Se registra cuando un destinatario ve un correo electrónico con imágenes NO bloqueadas. Solo se registra un evento de apertura por correo electrónico, por persona y por campaña inteligente. Si abren el mismo correo electrónico dos veces desde su bandeja de entrada, no se registrará más de una vez. |
| Hizo clic en | Se registra cada vez que se carga una URL decorada del correo electrónico en el explorador (como resultado de hacer clic en el vínculo ). Normalmente es el destinatario que hace clic, pero también puede ser un corte o pegado. |
| Suscripción cancelada | Se registra cuando una persona hace clic en el vínculo de cancelación de suscripción de un correo electrónico y envía el formulario de cancelación de suscripción. |

>[!CAUTION]
>
>Si el mismo correo electrónico se envía a la misma persona dos veces desde la misma campaña, la variable **Abierto** se registrará un máximo de 1 vez.
