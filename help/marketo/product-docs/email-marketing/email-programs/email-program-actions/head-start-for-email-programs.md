---
unique-page-id: 10097202
description: Inicio principal para Programas de correo electrónico - Documentos de marketing - Documentación del producto
title: Inicio principal para Programas de correo electrónico
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---


# Inicio principal para Programas de correo electrónico {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Crear un Programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Cuando se elige una fecha y hora para un Programa de correo electrónico, se determina cuándo comenzará el procesamiento del programa. Si desea que los mensajes de correo electrónico se inicien a la hora seleccionada, el Inicio de encabezado le ofrece esa opción procesando el programa por adelantado.

## Inicio de cabezal estándar {#standard-head-start}

1. Haga clic en **Actividades de mercadotecnia**.

   ![](assets/one-1.png)

1. Busque y seleccione su Programa de correo electrónico.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >El Inicio de cabezal no se puede utilizar con la prueba A/B.

1. En el mosaico Programar, programe el correo electrónico y, a continuación, seleccione el cuadro **Inicio de encabezado**.

   ![](assets/three-1.png)

   Con el Inicio de cabezal seleccionado, el programa empezará a procesarse aproximadamente 12 horas antes de la hora programada. Una vez procesados los inicios, el programa se bloquea.

   >[!CAUTION]
   >
   >Cualquier persona de su audiencia que cancele la suscripción después de la interrupción del programa seguirá recibiendo el correo electrónico. Le recomendamos que ajuste la notificación de cancelación de suscripción para reflejar que la cancelación de suscripciones puede tardar entre 1 y 2 días laborables en procesarse.

1. Haga clic en **Aprobar Programa**.

   ![](assets/four-1.png)

   Después de la aprobación del programa, puede que aparezcan cuatro estados diferentes en el mosaico Aprobación.

   * **Esperando para ejecutar:** una vez aprobado el programa.
   * **Procesamiento iniciado, esperando para ejecutarse:** Procesamiento en curso.
   * **Procesamiento terminado, esperando para ejecutarse:** procesamiento completado, correo electrónico que está esperando el inicio programado.
   * **Finalizado:** Programa completado.

   >[!TIP]
   >
   >¿Desea cancelar después de que el programa se bloquee pero antes de que el correo electrónico se envíe? ¡No hay problema! Haga clic en **Anular Programa** en la parte inferior derecha del mosaico Aprobación.

   >[!NOTE]
   >
   >Si desaprueba su programa de correo electrónico con menos de 12 horas de antelación con respecto a la hora de ejecución programada, pero luego cambia de opinión, deberá elegir una nueva fecha y hora con al menos 12 horas de antelación con respecto a la fecha de aprobación.

## Inicio principal con zona horaria de Destinatario {#head-start-with-recipient-time-zone}

Nuestra función de Inicio de cabezal actual requiere que el programa se programe con al menos 12 horas de anticipación. ¿Qué significa eso para el huso horario de Destinatario? Recuerde que cuando el huso horario de Destinatario está activo, se ejecuta el inicio de ejecutar el programa de correo electrónico a medianoche en el huso horario más antiguo (UTC +14:00). Por lo tanto, para habilitar **tanto** Inicio principal como Huso horario de Destinatario, los programas deben programarse **al menos 12 horas antes del primer huso horario (UTC +14:00**).

Esto significa que si se encuentra en América/Los Ángeles y desea habilitar tanto el Inicio principal como el huso horario del Destinatario, debe programar el programa **34 horas** con antelación. ¿Cómo llegamos a este número?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Obtenga ](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) más información sobre cómo programar programas de correo electrónico con el huso horario de Destinatario.

>[!MORELIKETHIS]
>
>* [Programar su Programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Programar Programas de correo electrónico con huso horario de Destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Explicación del huso horario del Destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

