---
unique-page-id: 2359545
description: Definición de los criterios de ganador de la prueba A/B - Documentos de Marketo - Documentación del producto
title: Definir los criterios de ganador de la prueba A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# Definir los criterios de ganador de la prueba A/B {#define-the-a-b-test-winner-criteria}

Cuando [agregue una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"} a su programa de correo electrónico, deberá elegir un tipo de prueba, [programar la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"} y luego definir los criterios de ganador. Así se decide qué correo electrónico gana.

>[!PREREQUISITES]
>
>[Agregar una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Criterios de ganadores {#winner-criteria}

1. Las opciones predeterminadas **[!UICONTROL Criterios de ganador]** se muestran primero.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>[!UICONTROL Abre]</b></td>
   <td>Una apertura registra cuándo se descargan las imágenes en un correo electrónico. Incluso si no incluye una imagen, Marketo inserta de forma predeterminada un solo píxel de seguimiento en todos los correos electrónicos de HTML.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Clics]</b></td>
   <td>De forma predeterminada, los vínculos de los correos electrónicos tienen un seguimiento incrustado que le permite ver quién hizo clic en qué vínculo, en cuántos vínculos se hizo clic, etc.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Haga clic para abrir] %</b></td>
   <td>Porcentaje de correos electrónicos que se abrieron y en los que se hizo clic en un vínculo. Esto mide la relevancia y el contexto de un correo electrónico tomando el número de clics únicos dividido por el número de aperturas únicas y luego multiplicándolo por 100 para mostrarlo como un porcentaje.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Puntuación de participación]</b></td>
   <td>La <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html?lang=es" target="_blank">puntuación de participación</a> le ayuda a determinar la eficacia de su contenido.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Si elige Puntuación de participación, la prueba deberá ejecutarse durante al menos 24 horas. Más información acerca de [cómo entender la puntuación de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. También puedes personalizar tus criterios seleccionando **[!UICONTROL Conversión personalizada]** y haciendo clic en **[!UICONTROL Editar]**.

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
   >Marketo solo permite déclencheur para las personas que han recibido el correo electrónico desde este programa de correo electrónico, por lo que no es necesario añadir el filtro &quot;Se envió el correo electrónico&quot;. Además, cuando utilice un déclencheur relacionado con el correo electrónico, asegúrese de utilizar &quot;is any&quot; como operador.

1. Haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   ¡Excelente! Ahora es el momento de decidir cómo se determina el ganador.

## Proclamar al ganador {#declare-winner}

1. Elija una de las dos opciones disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Si estás haciendo una prueba A/B de **Fecha/Hora**, solo puedes elegir **[!UICONTROL Manual]**.

   Una vez finalizada la prueba A/B, Marketo puede enviar automáticamente el correo electrónico ganador a la hora programada o puede revisar los resultados y decidir qué correo electrónico se envía cuando.

1. Automático es impresionante y es la opción predeterminada. Simplemente haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Si eliges **[!UICONTROL Manual]**, se enviará la prueba y esperarás a que declares un ganador. Recibirá un informe de los resultados.

¡Perfecto! Ahora vamos a [programar la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
