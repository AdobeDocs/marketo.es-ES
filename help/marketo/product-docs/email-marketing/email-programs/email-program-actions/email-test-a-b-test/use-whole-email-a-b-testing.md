---
unique-page-id: 2359502
description: Pruebas A/B de "correo electrónico completo" - Documentos de Marketo - Documentación del producto
title: Usar prueba A/B de "correo electrónico completo"
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Usar prueba A/B de &quot;correo electrónico completo&quot; {#use-whole-email-a-b-testing}

Puede probar fácilmente sus correos electrónicos A/B. Una buena prueba es la prueba de **Correo electrónico completo**. A continuación se muestra cómo configurarlo.

>[!PREREQUISITES]
>
>[Agregar una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. En el mosaico Correo electrónico, con el correo electrónico seleccionado, haga clic en **Agregar prueba A/B**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Se abre una nueva ventana. Haga clic en el menú desplegable **Tipo de prueba** y seleccione **Correos electrónicos completos**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Si tiene información de prueba anterior (como una prueba de sujeto), puede hacer clic con seguridad en **Restablecer prueba**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Seleccione su primer correo electrónico.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Haga clic en **Agregar** para aplicar el correo electrónico.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Puede añadir varios correos electrónicos. Sin embargo, si agrega demasiados, puede ralentizar el proceso de prueba hacia abajo.

1. Seleccione su segundo correo electrónico.

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. Haga clic en **Agregar** para aplicar el segundo correo electrónico. Arrastre el control deslizante para elegir el porcentaje de audiencia que desea que reciba la prueba A/B y haga clic en **Siguiente**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Las diferentes variaciones enviarán partes iguales del **Tamaño de muestra de prueba** elegido.

   >[!CAUTION]
   >
   >**Le recomendamos que evite establecer el tamaño de la muestra en 100%**. Si utiliza una lista estática, al establecer el tamaño de la muestra en 100 % se envía el correo electrónico a todos los miembros de la audiencia y el ganador no se lo lleva a nadie. Si usa una lista **inteligente**, al establecer el tamaño de la muestra en 100%, se enviará el correo electrónico a todos los miembros de la audiencia _en ese momento_. Cuando el programa de correo electrónico se vuelva a ejecutar más adelante, cualquier nueva persona que cumpla los requisitos para la lista inteligente también recibirá el correo electrónico, ya que ahora se incluye en la audiencia.

   Bien, ya casi llegamos. Ahora necesitamos [definir los criterios de ganador de la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
