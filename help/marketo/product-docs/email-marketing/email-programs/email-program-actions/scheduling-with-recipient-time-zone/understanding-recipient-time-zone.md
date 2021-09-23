---
unique-page-id: 12983291
description: 'Explicación de la zona horaria del destinatario: documentos de Marketo: documentación del producto'
title: Explicación de la zona horaria del destinatario
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# Explicación de la zona horaria del destinatario {#understanding-recipient-time-zone}

Los programas de correo electrónico y participación se pueden configurar para que se entreguen según los husos horarios de los destinatarios, lo que elimina la necesidad de crear varios programas; enviar una vez y Marketo guarda automáticamente el correo electrónico hasta la hora local correcta.

>[!NOTE]
>
>Actualmente, la zona horaria del destinatario funciona **solo** con contenido de correo electrónico. No funcionará para los programas de participación predeterminados.

## Programas de email {#email-programs}

Existen dos escenarios principales cuando [se programa un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Programando el programa para que se ejecute en las próximas 25 horas.
1. Programar el programa para que se ejecute más de 25 horas en el futuro (es decir, la semana siguiente).

Para poder ajustar cada huso horario, los programas de correo electrónico programados con la zona horaria del destinatario empiezan a ejecutarse a medianoche en la zona horaria **first/first** del mundo (UTC +14:00).

## Programas de participación {#engagement-programs}

Cuando [programe un flujo de programa de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) y la zona horaria del destinatario esté activa, el reparto del programa empezará a ejecutarse a medianoche en UTC +14:00. Le pedimos que programe la primera emisión al menos 25 horas en el futuro (24 horas más tiempo para comenzar la campaña) porque la gente puede calificar para la emisión en cada zona horaria en todo el mundo. Empezando el procesamiento en este momento en UTC +14:00 garantiza que enviaremos el correo electrónico en la fecha y hora programadas para todas las personas que califiquen para este reparto.

## Calcular zona horaria {#calculating-time-zone}

Marketo calcula la zona horaria en función de la ciudad, el estado, el país o el código postal de una persona. Si no podemos calcular la zona horaria de alguien a partir de estos valores, volveremos a los campos Ciudad Inferior, Estado Inferior, País Inferior y Código Postal Inferior Inferior.

En casos en los que tenemos **solo** País o **solo** Estado disponible:

* Para los países con tres o menos zonas horarias, seleccionamos la zona horaria media.
* Para los estados con dos zonas horarias, se selecciona la anterior de las dos.

Si todavía no podemos determinar la zona horaria de alguien a partir de ninguna combinación de estos campos, asignaremos **no** una zona horaria y el correo electrónico se enviará en función de la zona horaria de suscripción a Marketo. Por lo tanto, si el programa está programado para las 9:00 de la mañana PDT, las personas sin zona horaria asignada recibirán el correo electrónico a las 9:00 (PDT).

>[!NOTE]
>
>Marketo vuelve a calcular automáticamente la zona horaria de una persona cuando cambia cualquiera de los campos de entrada anteriores.

>[!MORELIKETHIS]
>
>* [Programar programas de correo electrónico con la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start para programas de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Programar programas de participación con huso horario del destinatario](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

