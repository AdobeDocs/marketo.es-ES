---
unique-page-id: 2359545
description: Definición de los criterios del ganador de la prueba A/B - Marketo Docs - Documentación del producto
title: Definir los criterios del ganador de la prueba A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
source-git-commit: 67ae4605d541a475b42a5094a5588c469a9d975d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 3%

---

# Definir los criterios del ganador de la prueba A/B {#define-the-a-b-test-winner-criteria}

When [adición de una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;} para su programa de correo electrónico, deberá elegir un tipo de prueba, [programar la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;} y, a continuación, defina los criterios ganadores. Así es como decidir qué correo electrónico gana.

>[!PREREQUISITES]
>
>[Agregar una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}

## Criterios de ganadores {#winner-criteria}

1. El valor predeterminado **Criterios de ganador** se muestran en primer lugar.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>Abre</b></td>
   <td>Una apertura se registra cuando las imágenes se descargan en un correo electrónico. Aunque no incluya una imagen, Marketo inserta de forma predeterminada un solo píxel de seguimiento en todos los correos electrónicos de HTML.</td>
   </tr>
   <tr>
   <td><b>Clics</b></td>
   <td>De forma predeterminada, los vínculos de los correos electrónicos tienen un seguimiento incrustado en ellos que le permite ver quién hizo clic en qué vínculo, cuántos vínculos totales se hicieron clic, etc.</td>
   </tr>
   <tr>
   <td><b>Hace clic para abrir %</b></td>
   <td>Porcentaje de correos electrónicos que se abrieron y en los que se hizo clic en un vínculo del correo electrónico. Esto mide la relevancia y el contexto de un correo electrónico tomando el número de clics únicos dividido por el número de aperturas únicas y luego multiplicándose por 100 para mostrarlo como un porcentaje.</td>
   </tr>
   <tr>
   <td><b>Puntaje de participación</b></td>
   <td>La variable <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">puntuación de participación</a> ayuda a determinar la eficacia del contenido.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Si elige Puntuación de participación, la prueba deberá ejecutarse durante al menos 24 horas. Más información sobre [explicación de la puntuación de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target=&quot;_blank&quot;}.

1. También puede personalizar sus criterios seleccionando Conversión personalizada y haciendo clic en Editar.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >La conversión personalizada permite elegir cualquier evento como conversión mediante déclencheur y filtros.

1. Se abrirá una ventana. Busque el déclencheur que desee y arrástrelo al lienzo.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Defina el déclencheur.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo solo permite déclencheur/filtros para las personas a las que se ha enviado el correo electrónico desde este programa de correo electrónico, por lo que no es necesario añadir el filtro &quot;Correo electrónico enviado&quot;. Además, al utilizar un déclencheur o filtro relacionado con el correo electrónico, asegúrese de utilizar &quot;is any&quot; como operador.

1. Haga clic en **Cerrar**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   ¡Excelente! Ahora es el momento de decidir cómo se determina el ganador.

## Proclamar al ganador {#declare-winner}

1. Elija una de las dos opciones disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Si está haciendo una **Fecha y hora** Prueba A/B, solo puede elegir **Manual**.

   Una vez finalizada la prueba A/B, Marketo puede enviar automáticamente el correo electrónico ganador a la hora programada, o puede revisar los resultados y decidir qué correo electrónico sale cuando.

1. Automático es impresionante y es la opción predeterminada. Haga clic en **Siguiente**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Elección **Manual** enviará la prueba y esperará a que declare un ganador. Recibirá un informe de los resultados.

¡Perfecto! Ahora vamos a [programar la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}.
