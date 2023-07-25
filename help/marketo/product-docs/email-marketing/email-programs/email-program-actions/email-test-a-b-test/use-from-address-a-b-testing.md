---
unique-page-id: 2359504
description: Pruebas A/B "Dirección De Origen" - Documentos de Marketo - Documentación del producto
title: Usar la prueba A/B "Dirección de origen"
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Usar la prueba A/B &quot;Dirección de origen&quot; {#use-from-address-a-b-testing}

Puede probar fácilmente sus correos electrónicos A/B. Una prueba interesante es la **Dirección desde** prueba. A continuación se muestra cómo configurarlo.

>[!PREREQUISITES]
>
>[Añadir una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. En el **Correo electrónico** mosaico, con el correo electrónico seleccionado, haga clic en **Añadir prueba A/B**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Se abrirá una nueva ventana, seleccione **Dirección desde** para **Tipo de prueba**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Si tiene información de prueba previa (como una prueba de sujeto), puede hacer clic con seguridad en **Restablecer prueba**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Introduzca el segundo **Dirección desde** información que desea probar.

   >[!NOTE]
   >
   >La opción A se rellenará previamente con la información contenida en el correo electrónico seleccionado.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Puede hacer clic en **+** para agregar todas las direcciones &quot;De&quot; que desee.

1. Utilice el control deslizante para elegir el porcentaje de audiencia que desea en la prueba A/B y haga clic en **Siguiente**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Las diferentes variaciones enviarán partes iguales del tamaño de muestra de prueba elegido.

   >[!CAUTION]
   >
   >**Se recomienda evitar establecer el tamaño de la muestra en 100 %**. Si utiliza una lista estática, al establecer el tamaño de la muestra en 100 % se envía el correo electrónico a todos los miembros de la audiencia y el ganador no se lo lleva a nadie. Si utiliza una variable **inteligente** , al establecer el tamaño de la muestra en 100 %, se envía el correo electrónico a todos los miembros de la audiencia _en ese momento_. Cuando el programa de correo electrónico se vuelva a ejecutar más adelante, cualquier nueva persona que cumpla los requisitos para la lista inteligente también recibirá el correo electrónico, ya que ahora se incluye en la audiencia.

   Bien, ya casi llegamos. Ahora necesitamos... [definir los criterios de ganador de la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
