---
unique-page-id: 12982903
description: Programar programas de correo electrónico con la zona horaria del destinatario - Documentos de Marketo - Documentación del producto
title: Programar programas de correo electrónico con la zona horaria del destinatario
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Programar programas de correo electrónico con la zona horaria del destinatario {#schedule-email-programs-with-recipient-time-zone}

Hay dos escenarios posibles al programar un programa de correo electrónico mientras está habilitada la zona horaria del destinatario:

1. Programación de la ejecución del programa **en** las siguientes 25 horas
1. Programación de la ejecución del programa **more** más de 25 horas en el futuro (es decir, la semana siguiente)

## Escenario 1: En un plazo de 25 horas {#scenario-within-hours}

Supongamos que aprueba un programa de correo electrónico con la zona horaria del destinatario habilitada y una hora de envío programada dentro de las próximas 25 horas. Puede tener personas en la lista inteligente que viven en zonas horarias en las que ya ha pasado la hora programada.

En este escenario, le permitimos decidir qué hacer con este subconjunto de personas cualificadas. Haga clic en el icono de engranaje situado junto a **Zona horaria del destinatario** en el **Programación** mosaico del programa de correo electrónico.

![](assets/image2017-12-5-10-3a46-3a42.png)

Esto le ofrece dos opciones:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definición**
>
>* **Enviar el día siguiente en el huso horario del destinatario**: si el correo electrónico está programado para que salga el martes a las 9:00 a.m., las personas cualificadas que vivan en zonas horarias en las que ya haya pasado la hora programada recibirán el correo electrónico en *Miércoles* a las 9:00 am.
>
>* **Entrega mediante la hora predeterminada establecida del programa**: si el correo electrónico está programado para que salga el martes a las 9:00 a. m., las personas cualificadas que vivan en zonas horarias en las que ya haya pasado la hora programada recibirán el correo electrónico _en función de la configuración de la zona horaria de suscripción_. Así que, si su [configuración de zona horaria de suscripción](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) están configurados en PDT América/Los Ángeles, estos destinatarios seguirán recibiendo el correo electrónico el martes a las 9:00 (PDT) (a cualquier hora que pueda estar en sus propios husos horarios).


>[!NOTE]
>
>[Más información](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) acerca de cómo calcula Marketo las zonas horarias de los destinatarios.

Consideremos este escenario con más detalle. Digamos que estás en San Francisco, programando un correo electrónico a las 7:00 am para un **9:00 am** enviar. En la lista inteligente, hay personas de las siguientes regiones:

* San Francisco
* Texas
* Nueva York
* Italia

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 am ya ha pasado en Nueva York e Italia, por lo que personas cualificadas en estas dos zonas horarias recibirán el correo electrónico basado en la variable **Configuración de zona horaria**:

* **Envíe el día siguiente en el huso horario del destinatario:** Miércoles a las 9:00 am en sus respectivos husos horarios, **O**

* **Entrega mediante la hora predeterminada establecida del programa**: Martes a las 9:00am PDT (Nueva York - 12:00pm EDT e Italia - 6:00pm CET).

Una vez aprobado el programa, comienza a ejecutarse en 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Aunque el programa iniciará el _proceso_ de enviar correos electrónicos en 15 minutos, los correos electrónicos no se _entrega_ en ese momento. Los destinatarios seguirán recibiendo correos electrónicos basados en la variable **Configuración de zona horaria** elija.

## Escenario 2: Más de 25 horas {#scenario-more-than-hours}

En esta segunda situación, apruebe un programa de correo electrónico con **Zona horaria del destinatario** y una hora de envío programada que supere las 25 horas en el futuro. En este caso, el programa empezará a ejecutarse a la hora programada en la **soon** zona horaria en el mundo (UTC + 14:00). Puede haber personas que cumplen los requisitos para su lista inteligente en cada zona horaria de todo el mundo, por lo que el inicio en la zona horaria más temprana nos permite enviar el correo electrónico en la fecha y hora programadas a todos los destinatarios en sus respectivas zonas horarias.

**Inicio con ventaja**

Ahora, hablemos de cómo [Inicio del cabezal](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funciona con **Zona horaria del destinatario**. Nuestra función de inicio de cabezal actual requiere que el programa se programe con al menos 12 horas de anticipación. ¿Qué significa eso para la zona horaria del destinatario? Recuerde que cuando la Zona horaria del destinatario está habilitada, empezamos a ejecutar el programa de correo electrónico a la hora programada en la zona horaria más temprana (UTC +14:00). Por lo tanto, para habilitar **both** Inicio del encabezado y Zona horaria del destinatario, los programas de correo electrónico deben programarse **al menos 12 horas antes de la hora programada en UTC +14:00.**

Esto significa que si está en América/Los Ángeles y desea habilitar tanto el inicio como la zona horaria del destinatario, debe programar el programa **34 horas** por adelantado. ¿Cómo llegamos a este número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

En resumen, los programas de correo electrónico programados con la zona horaria del destinatario deben empezar a ejecutarse a la hora programada en la zona horaria más temprana (es decir, donde llega a la medianoche primero) para poder ajustarse a cada zona horaria. Por lo tanto, si programa un programa de correo electrónico...

* **con una hora de envío _en_ 25 horas**, el programa empieza a ejecutarse en 15 minutos. Los destinatarios que ya hayan pasado la hora programada recibirán un correo electrónico basado en la configuración del huso horario seleccionada.
* **con una hora de envío _more than_ 25 horas en el futuro**, el programa comienza a ejecutarse a la hora programada en la zona horaria más temprana (UTC +14:00).
* **con inicio del cabezal**, el programa comienza a procesarse 12 horas antes de la hora programada en la zona horaria más temprana (UTC +14:00).

>[!CAUTION]
>
>Cualquier persona que cancele la suscripción entre el momento en que inicie el envío de su correo electrónico y el momento en que se envíe seguirá recibiendo el correo electrónico. Se recomienda ajustar la notificación de cancelación de suscripción para reflejar que las cancelaciones de suscripción pueden tardar entre 1 y 2 días hábiles en procesarse.

>[!MORELIKETHIS]
>
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start para programas de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Anular la entrega de programas de correo electrónico programados con el huso horario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

