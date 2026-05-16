---
unique-page-id: 2359504
description: Obtenga información sobre cómo ejecutar pruebas A/B desde direcciones remotas. Pruebe distintas direcciones de remitente y elija un ganador según el rendimiento.
title: Usar prueba A/B “Dirección de origen”
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
TQID: https://experienceleague.adobe.com/rerG-Wyn1X53QQBDXFwyg74uEOznGcYcBis9EwX4vQU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 2%

---

# Usar Prueba A/B &quot;[!UICONTROL Dirección De Origen]&quot; {#use-from-address-a-b-testing}

Puede probar fácilmente sus correos electrónicos A/B. Una prueba interesante es la prueba **[!UICONTROL Dirección de origen]**. A continuación se muestra cómo configurarlo.

>[!PREREQUISITES]
>
>[Agregar una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. En el mosaico **[!UICONTROL Correo electrónico]**, con el correo electrónico seleccionado, haga clic en **[!UICONTROL Agregar prueba A/B]**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Se abre una nueva ventana, seleccione **[!UICONTROL Dirección desde]** para **[!UICONTROL Tipo de prueba]**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Si tiene información de prueba anterior (como una prueba de sujeto), puede hacer clic con seguridad en **[!UICONTROL Restablecer prueba]**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Escriba la segunda información **[!UICONTROL de la dirección]** que desee probar.

   >[!NOTE]
   >
   >La opción A se rellenará previamente con la información contenida en el correo electrónico seleccionado.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Puede hacer clic en **+** para agregar todas las direcciones remitente que desee.

1. Utilice el control deslizante para elegir el porcentaje de audiencia que desea en la prueba A/B y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Las diferentes variaciones enviarán partes iguales del tamaño de muestra de prueba elegido.

   >[!CAUTION]
   >
   >**Le recomendamos que evite establecer el tamaño de la muestra en 100%**. Si utiliza una lista estática, al establecer el tamaño de la muestra en 100 % se envía el correo electrónico a todos los miembros de la audiencia y el ganador se lo lleva a nadie. Si usa una lista **inteligente**, al establecer el tamaño de la muestra en 100% se enviará el correo electrónico a todos los miembros de la audiencia _en ese momento_. Cuando el programa de correo electrónico se vuelva a ejecutar más adelante, cualquier nueva persona que cumpla los requisitos para la lista inteligente también recibirá el correo electrónico, ya que ahora se incluye en la audiencia.

   Bien, ya casi llegamos. Ahora necesitamos [definir los criterios de ganador de la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
