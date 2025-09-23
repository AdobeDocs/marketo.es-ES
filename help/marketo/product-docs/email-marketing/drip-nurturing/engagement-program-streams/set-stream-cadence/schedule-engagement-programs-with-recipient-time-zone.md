---
unique-page-id: 12982909
description: Programar programas de participación con la zona horaria del destinatario - Documentos de Marketo - Documentación del producto
title: Planificar programas de participación con la zona horaria del destinatario
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 8%

---

# Planificar programas de participación con la zona horaria del destinatario {#schedule-engagement-programs-with-recipient-time-zone}

Cuando se programa un flujo de programa de participación y la zona horaria del destinatario está activa, el lanzamiento del programa comenzará a ejecutarse a medianoche en la primera zona horaria (UTC +14:00). Es necesario que programes el primer reparto **al menos 25 horas** en el futuro, ya que puede haber personas que califiquen para el reparto en todas las zonas horarias del mundo. Comenzar a procesar en este momento en el primer huso horario garantiza que entregaremos el correo electrónico en la fecha y hora programadas para cada destinatario.

1. En el programa de participación, vaya a la pestaña **[!UICONTROL Transmisiones]** y haga clic en la programación de cadencia de una transmisión para editarla.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Establece la configuración de cadencia](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) como lo harías normalmente y luego marca la casilla **[!UICONTROL Zona horaria del destinatario]**. Recuerde que su primer lanzamiento debe ser al menos 25 horas en el futuro. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Tenga en cuenta que con la zona horaria del destinatario activa, la programación de cadencia no mostrará una zona horaria específica, ya que podría haber varias. Solo muestra la hora.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Establecer cadencia de flujo](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
