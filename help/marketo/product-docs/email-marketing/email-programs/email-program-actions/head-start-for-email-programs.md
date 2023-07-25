---
unique-page-id: 10097202
description: Head Start para programas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Head Start para programas de correo electrónico
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Head Start para programas de correo electrónico {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Crear un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Al elegir una fecha y hora para un programa de correo electrónico, determina cuándo comenzará a procesarse el programa. Si desea que sus correos electrónicos se lancen en el momento seleccionado, Head Start le da esa opción al procesar el programa por adelantado.

## Head Start estándar {#standard-head-start}

1. Clic **Actividades de marketing**.

   ![](assets/one-1.png)

1. Busque y seleccione su programa de correo electrónico.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start no se puede usar con las pruebas A/B.

1. En el mosaico Programar, programe el correo electrónico y, a continuación, seleccione la **Head Start** cuadro.

   ![](assets/three-1.png)

   Con Head Start seleccionado, el programa comenzará a procesarse aproximadamente 12 horas antes de la hora programada. Una vez iniciado el procesamiento, el programa se bloquea.

   >[!CAUTION]
   >
   >Cualquier persona de la audiencia que cancele la suscripción después del bloqueo del programa seguirá recibiendo el correo electrónico. Recomendamos ajustar la notificación de cancelación de suscripción para reflejar que las cancelaciones de suscripción pueden tardar entre 1 y 2 días hábiles en procesarse.

1. Clic **Aprobar programa**.

   ![](assets/four-1.png)

   Después de la aprobación del programa, hay cuatro estados diferentes que puede ver en el mosaico Aprobación.

   * **Esperando a ejecutarse:** Una vez aprobado el programa.
   * **Procesamiento iniciado, esperando para ejecutarse:** El procesamiento está en curso.
   * **Procesamiento finalizado, esperando para ejecutarse:** Procesamiento completado, correo electrónico que ahora espera la hora programada para el inicio.
   * **Finalizado:** Programa completado.

   >[!TIP]
   >
   >¿Desea cancelar después de que el programa se bloquee pero antes de que se envíe el correo electrónico? ¡No hay problema! Simplemente haga clic en **Anular programa** en la parte inferior derecha del mosaico Aprobación.

   >[!NOTE]
   >
   >Si desaprueba su programa de correo electrónico con menos de 12 horas antes de su tiempo de ejecución programado, pero luego cambia de opinión, deberá elegir una nueva fecha/hora que sea al menos 12 horas antes de la fecha en que lo apruebe.

## Head Start con zona horaria del destinatario {#head-start-with-recipient-time-zone}

Nuestra función actual de Head Start requiere que el programa se programe con al menos 12 horas de anticipación. ¿Qué significa eso para la zona horaria del destinatario? Recuerde que cuando la zona horaria del destinatario está activa, el programa de correo electrónico se inicia a medianoche en la zona horaria más temprana (UTC +14:00). Por lo tanto, para habilitar **ambos** Zona horaria de Head Start y de los destinatarios, es necesario programar los programas **al menos 12 horas antes de la zona horaria más temprana (UTC +14:00)**.)

Esto significa que si se encuentra en América/Los Ángeles y desea habilitar tanto Head Start como la Zona horaria del destinatario, debe programar el programa **34 horas** por adelantado. ¿Cómo llegamos a este número?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Más información](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) Obtenga información sobre cómo programar programas de correo electrónico con la zona horaria del destinatario.

>[!MORELIKETHIS]
>
>* [Programe su programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Programar programas de correo electrónico con zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
