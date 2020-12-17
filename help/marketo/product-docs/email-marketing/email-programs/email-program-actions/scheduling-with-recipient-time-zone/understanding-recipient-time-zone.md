---
unique-page-id: 12983291
description: Explicación del huso horario del Destinatario - Documentos de marketing - Documentación del producto
title: Explicación del huso horario del Destinatario
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Explicación del huso horario del Destinatario {#understanding-recipient-time-zone}

Los programas de correo electrónico y participación se pueden configurar para que se entreguen según las zonas horarias de los destinatarios, lo que elimina la necesidad de crear varios programas: enviar una vez y Marketo guarda automáticamente el correo electrónico hasta la hora local correcta.

>[!NOTE]
>
>El huso horario de destinatario funciona **sólo** con contenido de correo electrónico. No funcionará para los programas de participación predeterminados.

## Programas de correo electrónico {#email-programs}

Existen dos escenarios principales cuando [programa un programa de correo electrónico](schedule-email-programs-with-recipient-time-zone.md):

1. Programando la ejecución del programa en las próximas 25 horas.
1. Programando el programa para que se ejecute más de 25 horas en el futuro (es decir, la próxima semana).

Para poder acomodar todos los husos horarios, los programas de correo electrónico programados con el inicio de huso horario de Destinatario se ejecutan a medianoche en el **primer/primer** huso horario del mundo (UTC +14:00).

## Programas de participación {#engagement-programs}

Cuando [programe un flujo de programas de participación](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) y el huso horario de Destinatario esté activo, el reparto de programas se inicio cuando se ejecute a medianoche en UTC +14:00. Le pedimos que programe la primera emisión al menos 25 horas en el futuro (24 horas + un poco de tiempo para iniciar la campaña) porque la gente puede calificar para la emisión en cada huso horario en todo el mundo. Empezar el procesamiento en este momento en UTC +14:00 garantiza que enviaremos el correo electrónico en la fecha y hora programadas para cada persona que califique para este envío.

## Calcular huso horario {#calculating-time-zone}

Marketo calcula la zona horaria en función de la ciudad, el estado, el país o el código postal de una persona. Si no podemos calcular la zona horaria de alguien a partir de estos valores, volvemos a nuestros campos Ciudad Inferior, Estado Inferior, País Inferior y Código Postal Inferido.

En los casos en los que tenemos **solamente **País o **sólo** Estado disponible:

* Para países con tres o menos husos horarios, seleccionamos la zona horaria media.
* Para los estados con dos husos horarios, seleccionamos el anterior de los dos.

Si todavía no podemos determinar el huso horario de alguien a partir de una combinación de estos campos, **no** asignaremos un huso horario y el correo electrónico se enviará en función del huso horario de suscripción de Marketing to. Por lo tanto, si el programa está programado para las 9:00 a.m. PDT, las personas sin zona horaria asignada recibirán el correo electrónico a las 9:00 a.m. PDT.

>[!NOTE]
>
>Marketo vuelve a calcular automáticamente el huso horario de una persona cuando cambia cualquiera de los campos de entrada anteriores.

>[!MORELIKETHIS]
>
>* [Programar Programas de correo electrónico con huso horario de Destinatario](schedule-email-programs-with-recipient-time-zone.md)
>* [Inicio principal para Programas de correo electrónico](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [Programar Programas de participación con huso horario de Destinatario](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>



