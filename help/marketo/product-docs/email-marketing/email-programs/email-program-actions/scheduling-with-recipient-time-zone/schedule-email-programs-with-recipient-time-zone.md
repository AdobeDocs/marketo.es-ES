---
unique-page-id: 12982903
description: Programar Programas de correo electrónico con huso horario de Destinatario - Documentos de marketing - Documentación del producto
title: Programar Programas de correo electrónico con huso horario de Destinatario
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---


# Programar Programas de correo electrónico con huso horario de Destinatario {#schedule-email-programs-with-recipient-time-zone}

Existen dos escenarios posibles al programar un programa de correo electrónico mientras el huso horario de Destinatario está habilitado:

1. Programando la ejecución del programa **dentro de** las próximas 25 horas
1. Programando el programa para que se ejecute **más** de 25 horas en el futuro (es decir, la semana siguiente)

## Escenario 1: Dentro de las 25 horas {#scenario-within-hours}

Supongamos que aprueba un programa por correo electrónico con la zona horaria de Destinatario habilitada y una hora de entrega programada en las próximas 25 horas. Es posible que haya personas en su lista inteligente que vivan en zonas horarias en las que la hora programada ya ha pasado.

En este escenario, le permitimos decidir qué hacer con este subconjunto de personas cualificadas. Haga clic en el icono de engranaje situado junto a **Huso horario de Destinatario** en el mosaico **Programación** del programa de correo electrónico.

![](assets/image2017-12-5-10-3a46-3a42.png)

Esto le ofrece dos opciones:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definición**
>
>* **Entregar el día siguiente en el huso** horario de destinatario: si el correo electrónico está programado para que salga el martes a las 9:00 a.m., las personas cualificadas que viven en zonas horarias en las que ya ha pasado la hora programada recibirán el correo electrónico el  ** miércoles a las 9:00 a.m.
   >
   >
* **Entregar utilizando la hora** predeterminada del programa: si el correo electrónico está programado para que se publique el martes a las 9:00 a.m., las personas cualificadas que vivan en zonas horarias en las que ya haya transcurrido la hora programada recibirán el correo electrónico  _en función de la configuración_ del huso horario de su suscripción. Por lo tanto, si su [configuración del huso horario de suscripción](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) está establecida en PDT América/Los Ángeles, estos destinatarios seguirán recibiendo el correo electrónico el martes a las 9:00am PDT (en cualquier momento que se encuentre en sus propios husos horarios).


>[!NOTE]
>
>[Obtenga ](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) más información sobre cómo Marketing calcula los husos horarios de los destinatarios.

Analicemos este escenario con más detalle. Digamos que está en San Francisco, programando un correo electrónico a las 7:00am para un envío **9:00am**. En su lista inteligente, hay personas de las siguientes regiones:

* San Francisco
* Texas
* Nueva York
* Italia

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 am ya ha pasado en Nueva York e Italia, por lo que personas cualificadas en estas dos zonas horarias recibirán el correo electrónico basado en la **Configuración de huso horario**:

* **Entregar el día siguiente en el huso horario de destinatario:** miércoles a las 9:00 a.m. en sus respectivos husos horarios,  **O**

* **Entregar utilizando la hora** predeterminada del programa: Martes a las 9:00am PDT (Nueva York - 12:00pm EDT e Italia - 6:00pm CET).

Una vez aprobado el programa, se inicio que se ejecute en 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Aunque el programa realizará el inicio del _proceso_ de enviar correos electrónicos en 15 minutos, los mensajes de correo electrónico no se _enviarán_ en ese momento. Los destinatarios seguirán recibiendo correos electrónicos basados en la **configuración del huso horario** que elija.

## Escenario 2: Más de 25 horas {#scenario-more-than-hours}

En este segundo escenario, se aprueba un programa por correo electrónico con **Huso horario de Destinatario** habilitado y un tiempo de entrega programado que supere las 25 horas en el futuro. En este caso, el programa se ejecutará en inicio a la hora programada en el **huso horario más temprano** del mundo (UTC + 14:00). Es posible que haya personas que califiquen para su lista inteligente en todos los husos horarios del mundo, por lo que, a partir del primer huso horario, podemos enviar el correo electrónico en la fecha y hora programadas a todos los destinatarios de sus respectivos husos horarios.

**Inicio de cabezal**

Ahora, hablemos de cómo [Inicio de cabeza](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funciona con **Huso horario de Destinatario**. Nuestra función de Inicio de cabezal actual requiere que el programa se programe con al menos 12 horas de anticipación. ¿Qué significa eso para la zona horaria del Destinatario? Recuerde que cuando el huso horario de Destinatario está habilitado, se ejecuta el inicio de ejecución del programa de correo electrónico a la hora programada en el primer huso horario (UTC +14:00). Por lo tanto, para habilitar **tanto** Inicio principal como Huso horario de Destinatario, los programas de correo electrónico deben programarse **al menos 12 horas antes de la hora programada en UTC +14:00.**

Esto significa que si se encuentra en América/Los Ángeles y desea habilitar tanto el Inicio principal como el huso horario del Destinatario, debe programar el programa **34 horas** con antelación. ¿Cómo llegamos a este número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

En resumen, los programas de correo electrónico programados con el huso horario de Destinatario deben ejecutarse a la hora programada en el primer huso horario (es decir, donde llega a la medianoche primero) para poder alojar cada huso horario. Así que, si programas un programa por correo electrónico...

* **con un tiempo de envío  _dentro_  de las 25 horas**, los inicios de programa funcionan en 15 minutos. Los destinatarios que ya hayan pasado la hora programada recibirán el correo electrónico en función de la configuración del huso horario seleccionada.
* **con una hora de envío  _superior_  a 25 horas en el futuro**, los inicios de programa se ejecutan a la hora programada en la zona horaria más temprana (UTC +14:00).
* **con Inicio** principal, los inicios de programa procesan 12 horas antes de la hora programada en la zona horaria más temprana (UTC +14:00).

>[!CAUTION]
>
>Cualquier persona que cancele la suscripción entre el momento en que inicio el envío de su correo electrónico y el momento en que se entrega, seguirá recibiendo el correo electrónico. Le recomendamos que ajuste la notificación de cancelación de suscripción para reflejar que la cancelación de suscripciones puede tardar entre 1 y 2 días laborables en procesarse.

>[!MORELIKETHIS]
>
>* [Explicación del huso horario del Destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Inicio principal para Programas de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Anular Envío de Programas de correo electrónico programados con el huso horario de Destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

