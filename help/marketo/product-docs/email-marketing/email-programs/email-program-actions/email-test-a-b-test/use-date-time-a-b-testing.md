---
unique-page-id: 2359520
description: Usar la prueba A/B "Fecha/hora" - Documentos de Marketo - Documentación del producto
title: Usar prueba A/B "Fecha/Hora"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Usar prueba A/B &quot;Fecha/Hora&quot; {#use-date-time-a-b-testing}

Puede probar fácilmente sus correos electrónicos A/B. Una prueba es la **Fecha/hora** prueba. Esto prueba a qué hora del día o del día de la semana es mejor enviar correos electrónicos. A continuación se muestra cómo configurarlo.

>[!PREREQUISITES]
>
>[Añadir una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. En el **Correo electrónico** mosaico, haga clic en **Añadir prueba A/B**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Se abre una nueva ventana. Seleccionar **Fecha/hora** para **Tipo de prueba**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Si tiene información de prueba previa (como una prueba de sujeto), puede hacer clic con seguridad en **Restablecer prueba**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Seleccione la fecha de la primera fecha/hora.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Seleccione la hora de la primera fecha/hora.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Haga lo mismo con la segunda fecha y hora.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Utilice el control deslizante para elegir el porcentaje de audiencia que desea en la prueba A/B y haga clic en **Siguiente**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Las diferentes variaciones se aplicarán a partes iguales del tamaño de muestra de prueba elegido.

   >[!CAUTION]
   >
   >**Se recomienda evitar establecer el tamaño de la muestra en 100 %**. Si utiliza una lista estática, al establecer el tamaño de la muestra en 100 % se envía el correo electrónico a todos los miembros de la audiencia y el ganador no se lo lleva a nadie. Si utiliza una variable **inteligente** , al establecer el tamaño de la muestra en 100 %, se envía el correo electrónico a todos los miembros de la audiencia _en ese momento_. Cuando el programa de correo electrónico se vuelva a ejecutar más adelante, cualquier nueva persona que cumpla los requisitos para la lista inteligente también recibirá el correo electrónico, ya que ahora se incluye en la audiencia.

   Bueno, estamos un paso más cerca. Ahora necesitamos... [definir los criterios de ganador de la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
