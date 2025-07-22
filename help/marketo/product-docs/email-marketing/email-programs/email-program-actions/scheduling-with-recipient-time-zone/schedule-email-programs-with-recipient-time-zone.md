---
unique-page-id: 12982903
description: Programar programas de correo electrónico con la zona horaria del destinatario - Documentos de Marketo - Documentación del producto
title: Programar programas de correo electrónico con zona horaria del destinatario
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Programar programas de correo electrónico con zona horaria del destinatario {#schedule-email-programs-with-recipient-time-zone}

Existen dos situaciones potenciales al programar un programa de correo electrónico mientras la zona horaria del destinatario está activada:

1. Programando el programa para ejecutar **en** las próximas 25 horas
1. Programando el programa para que se ejecute **más** de 25 horas en el futuro (es decir, la semana que viene)

## Escenario 1: en 25 horas {#scenario-within-hours}

Supongamos que aprueba un programa de correo electrónico con la zona horaria del destinatario habilitada y una hora de envío programada en las próximas 25 horas. Es posible que tenga personas en la lista inteligente que vivan en zonas horarias en las que la hora programada ya haya pasado.

En este escenario, le permitimos decidir qué hacer con este subconjunto de personas calificadas. Haga clic en el icono de engranaje situado junto a **[!UICONTROL Zona horaria del destinatario]** en el mosaico **[!UICONTROL Programar]** del programa de correo electrónico.

![](assets/image2017-12-5-10-3a46-3a42.png)

Esto le ofrece dos opciones:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definición**
>
>* **[!UICONTROL Enviar al día siguiente en el huso horario del destinatario]**: si el correo electrónico está programado para salir el martes a las 9:00am, las personas calificadas que vivan en zonas horarias en las que ya haya pasado el huso horario programado recibirán el correo electrónico el *miércoles* a las 9:00am.
>
>* **[!UICONTROL Enviar usando la hora predeterminada del programa]**: si el correo electrónico está programado para salir el martes a las 9:00am, las personas calificadas que vivan en zonas horarias donde ya ha pasado la hora programada recibirán el correo electrónico _según la configuración de la zona horaria de la suscripción_. Por lo tanto, si la configuración de la zona horaria de la suscripción [1&rbrace; está establecida en PDT América/Los Ángeles, estos destinatarios seguirán recibiendo el correo electrónico del martes a las 9](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) PDT (la hora que esté en sus propias zonas horarias).:00am

>[!NOTE]
>
>[Más información](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) sobre cómo calcula Marketo las zonas horarias para los destinatarios.

Consideremos este escenario con más detalle. Supongamos que está en San Francisco, programando un correo electrónico a las 7:00am para un envío de **9:00am**. En la lista inteligente hay personas de las siguientes regiones:

* San Francisco
* Texas
* Nueva York
* Italia

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00am ya ha pasado en Nueva York e Italia, por lo que las personas calificadas en estas dos zonas horarias recibirán el correo electrónico según la **Configuración de zona horaria**:

* **[!UICONTROL Enviar al día siguiente en el huso horario del destinatario]:** Miércoles a las 9:00am en sus respectivos husos horarios, **OR**

* **[!UICONTROL Envío con la hora establecida predeterminada del programa]**: martes a las 9:00am PDT (Nueva York - 12:00pm EDT e Italia - 6:00pm CET).

Una vez aprobado el programa, comienza a ejecutarse en 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Aunque el programa iniciará el _proceso_ de envío de correos electrónicos en 15 minutos, no se enviarán _correos electrónicos_ en ese momento. Los destinatarios seguirán recibiendo correos electrónicos según la **[!UICONTROL configuración de huso horario]** que elija.

## Escenario 2: más de 25 horas {#scenario-more-than-hours}

En este segundo escenario, usted aprueba un programa de correo electrónico con **[!UICONTROL Zona horaria del destinatario]** habilitada y una hora de entrega programada de más de 25 horas en el futuro. En este caso, el programa comenzará a ejecutarse a la hora programada en la zona horaria **más temprana** del mundo (UTC + 14:00). Puede haber personas que cumplan los requisitos para su lista inteligente en cada zona horaria del mundo, por lo que empezar en la zona horaria más temprana nos permite enviar el correo electrónico en la fecha u hora programadas a todos los destinatarios en sus respectivas zonas horarias.

**Head Start**

Ahora hablemos de cómo funciona [[!UICONTROL Head Start]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) con la **[!UICONTROL zona horaria del destinatario]**. Nuestra función actual de Head Start requiere que el programa se programe con al menos 12 horas de anticipación. ¿Qué significa eso para la zona horaria del destinatario? Recuerde que cuando la zona horaria del destinatario está habilitada, se inicia la ejecución del programa de correo electrónico a la hora programada en la zona horaria más temprana (UTC +14:00). Por lo tanto, para habilitar **tanto** como la zona horaria de Head Start y Destinatario, los programas de correo electrónico deben programarse **al menos 12 horas antes de la hora programada en UTC +14:00.**

Esto significa que si se encuentra en América/Los Ángeles y desea habilitar Head Start y la zona horaria del destinatario, debe programar el programa con **34 horas** de anticipación. ¿Cómo llegamos a este número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

En resumen, los programas de correo electrónico programados con Zona horaria de destinatario deben comenzar a ejecutarse a la hora programada en la zona horaria más temprana (es decir, donde llega primero a la medianoche) para adaptarse a cada zona horaria. Así que, si programas un programa de correo electrónico...

* **con un tiempo de entrega de _en_ 25 horas**, el programa comenzará a ejecutarse en un plazo de 15 minutos. Los destinatarios que ya hayan superado la hora programada recibirán el correo electrónico en función de la configuración de zona horaria que haya elegido.
* **con un tiempo de entrega de _más de_ 25 horas en el futuro**, el programa se empezará a ejecutar a la hora programada en la zona horaria más temprana (UTC +14:00).
* **con Head Start**, el programa comienza a procesarse 12 horas antes de la hora programada en la zona horaria más temprana (UTC +14:00).

>[!CAUTION]
>
>Cualquier persona que cancele la suscripción entre el momento en que inicie su envío de correo electrónico y el momento en que se envíe realmente seguirá recibiendo el correo electrónico. Recomendamos ajustar la notificación de cancelación de suscripción para reflejar que las cancelaciones de suscripción pueden tardar entre 1 y 2 días hábiles en procesarse.

>[!MORELIKETHIS]
>
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start para programas de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Anular la entrega de programas de correo electrónico programados con la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
