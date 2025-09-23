---
unique-page-id: 12983291
description: Explicación de la zona horaria del destinatario - Documentos de Marketo - Documentación del producto
title: Explicación de zona horaria del destinatario
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Explicación de zona horaria del destinatario {#understanding-recipient-time-zone}

Los programas de correo electrónico y participación se pueden configurar para que se entreguen según los husos horarios de los destinatarios, lo que elimina la necesidad de crear varios programas: enviar una vez y Marketo retiene automáticamente el correo electrónico hasta la hora local correcta.

>[!NOTE]
>
>La zona horaria de [!UICONTROL destinatario] funciona actualmente **solo** con contenido de correo electrónico. No funcionará para programas de participación predeterminados.

## Programas de correo electrónico {#email-programs}

Hay dos escenarios principales cuando [se programa un correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Programando el programa para que se ejecute en las próximas 25 horas.
1. Programar el programa para que se ejecute durante más de 25 horas en el futuro (es decir, la semana que viene).

Para dar cabida a cada zona horaria, los programas de correo electrónico programados con [!UICONTROL Zona horaria del destinatario] comienzan a ejecutarse a medianoche en la zona horaria **primera/más antigua** del mundo (UTC +14:00).

## Programas de participación {#engagement-programs}

Cuando [programe un flujo de programa de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) y la [!UICONTROL zona horaria del destinatario] esté activa, el lanzamiento del programa comenzará a ejecutarse a medianoche en UTC +14:00. Necesitamos que programes el primer reparto al menos 25 horas en el futuro (24 horas + algún tiempo para comenzar la campaña) porque las personas pueden calificar para el reparto en cada zona horaria en todo el mundo. Comenzar a procesar en este momento en UTC +14:00 garantiza que el correo electrónico se envíe en la fecha y hora programadas para cada persona que califique para este reparto.

## Cálculo de zona horaria {#calculating-time-zone}

Marketo calcula la zona horaria en función de la ciudad, el estado, el país o el código postal de una persona. Si no podemos calcular la zona horaria de alguien a partir de estos valores, volvemos a los campos Ciudad deducida, Estado deducido, País deducido y Código postal deducido.

En casos en los que tenemos **solamente** país o **solamente** estado disponibles:

* Para los países con tres o menos zonas horarias, seleccionamos la zona horaria media.
* Para los estados con dos zonas horarias, se selecciona la anterior de las dos.

Si todavía no podemos determinar la zona horaria de alguien a partir de cualquier combinación de estos campos, **no** asignaremos una zona horaria y el correo electrónico se enviará según la zona horaria de suscripción de Marketo. Por lo tanto, si su programa está programado para 9:00am PDT, las personas sin zona horaria asignada se enviarán por correo electrónico a 9:00am PDT.

>[!NOTE]
>
>Marketo recalcula automáticamente la zona horaria de una persona cuando cambia cualquiera de los campos de entrada anteriores.

>[!MORELIKETHIS]
>
>* [Programar programas de correo electrónico con [!UICONTROL Zona horaria del destinatario]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start para programas de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Programar programas de participación con [!UICONTROL Zona horaria del destinatario]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
