---
unique-page-id: 12982909
description: Programar programas de participación con la zona horaria del destinatario - Documentos de Marketo - Documentación del producto
title: Programar programas de participación con la zona horaria del destinatario
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Programar programas de participación con la zona horaria del destinatario {#schedule-engagement-programs-with-recipient-time-zone}

Cuando se programa un flujo de programa de participación y la zona horaria del destinatario está activa, el lanzamiento del programa comenzará a ejecutarse a medianoche en la primera zona horaria (UTC +14:00). Necesitamos que programes el primer reparto **al menos 25 horas** en el futuro, porque puede haber personas que califiquen para el reparto en cada huso horario en todo el mundo. Comenzar a procesar en este momento en el primer huso horario garantiza que entregaremos el correo electrónico en la fecha y hora programadas para cada destinatario.

1. En el programa de participación, vaya a **Flujos** y haga clic en la programación de cadencia de una emisión para editarla.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Establezca la configuración de cadencia](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) como lo haría normalmente, compruebe la **Zona horaria del destinatario** cuadro. Recuerde que su primer lanzamiento debe ser al menos 25 horas en el futuro. Clic **Guardar**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Tenga en cuenta que con la zona horaria del destinatario activa, la programación de cadencia no mostrará una zona horaria específica, ya que podría haber varias. Solo muestra la hora.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Explicación de la zona horaria del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Definir cadencia de flujo](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
