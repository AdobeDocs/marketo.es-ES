---
unique-page-id: 10097202
description: Inicio de los programas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Head Start para programas de correo electrónico
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Head Start para programas de correo electrónico {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Crear un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Cuando elige una fecha y hora para un programa de correo electrónico, determina cuándo comenzará el procesamiento del programa. Si desea que sus correos electrónicos se inicien en el momento seleccionado, Head Start le da esa opción procesando el programa por adelantado.

## Inicio de cabezal estándar {#standard-head-start}

1. Haga clic en **Actividades de marketing**.

   ![](assets/one-1.png)

1. Busque y seleccione su programa de correo electrónico.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >No se puede utilizar Head Start con pruebas A/B.

1. En el mosaico Programar , programe el correo electrónico y, a continuación, seleccione la opción **Inicio del cabezal** en la ventana

   ![](assets/three-1.png)

   Con Inicio de cabezal seleccionado, el programa empezará a procesarse aproximadamente 12 horas antes de la hora programada. Una vez iniciado el procesamiento, el programa se bloquea.

   >[!CAUTION]
   >
   >Cualquier persona de la audiencia que cancele la suscripción después del bloqueo del programa seguirá recibiendo el correo electrónico. Se recomienda ajustar la notificación de cancelación de suscripción para reflejar que las cancelaciones de suscripción pueden tardar entre 1 y 2 días hábiles en procesarse.

1. Haga clic en **Aprobar programa**.

   ![](assets/four-1.png)

   Después de la aprobación del programa, puede ver cuatro estados diferentes en el mosaico Aprobación .

   * **Esperando para ejecutarse:** Una vez aprobado el programa.
   * **Procesamiento iniciado, esperando para ejecutarse:** El procesamiento está en curso.
   * **Procesamiento finalizado, esperando para ejecutarse:** Procesamiento completado, correo electrónico que ahora espera el inicio programado.
   * **Finalizado:** Programa completado.

   >[!TIP]
   >
   >¿Desea cancelar después de que el programa se bloquee pero antes de que el correo electrónico envíe? ¡No hay problema! Simplemente haga clic en **Programa de anulación** en el lado inferior derecho del mosaico Aprobación .

   >[!NOTE]
   >
   >Si desaprueba el programa de correo electrónico con menos de 12 horas de antelación a la hora de ejecución programada, pero luego cambia de opinión, deberá elegir una nueva fecha/hora que tenga al menos 12 horas de antelación con respecto a la fecha de aprobación.

## Head Start with Recipient Time Zone (Inicio del encabezado con la zona horaria del destinatario) {#head-start-with-recipient-time-zone}

Nuestra función de inicio de cabezal actual requiere que el programa se programe con al menos 12 horas de anticipación. ¿Qué significa eso para la zona horaria del destinatario? Recuerde que cuando la zona horaria del destinatario está activa, empezamos a ejecutar el programa de correo electrónico a medianoche en la zona horaria más temprana (UTC +14:00). Por lo tanto, para habilitar **both** Inicio del encabezado y Zona horaria del destinatario, los programas deben programarse **al menos 12 horas antes de la zona horaria más temprana (UTC +14:00**.)

Esto significa que si está en América/Los Ángeles y desea habilitar tanto el inicio como la zona horaria del destinatario, debe programar el programa **34 horas** por adelantado. ¿Cómo llegamos a este número?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Más información](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) acerca de cómo programar programas de correo electrónico con la zona horaria del destinatario.

>[!MORELIKETHIS]
>
>* [Programar su programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Programar programas de correo electrónico con la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

