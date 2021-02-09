---
unique-page-id: 2359545
description: Definir los criterios del ganador de la prueba A/B - Documentos de marketing - Documentación del producto
title: Definir los criterios del ganador de la prueba A/B
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Definir los criterios del ganador de la prueba A/B {#define-the-a-b-test-winner-criteria}

Cuando [agregue una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md) a su programa de correo electrónico, deberá elegir un tipo de prueba, [programe la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md) y luego definir los criterios ganadores. Así es como decidir qué correo electrónico gana.

>[!PREREQUISITES]
>
>[Añadir una prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

## Criterios del ganador {#winner-criteria}

1. Las opciones predeterminadas **Criterios del ganador** se enumeran en primer lugar.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Abre** | Un archivo abierto se registra cuando las imágenes se descargan en un mensaje de correo electrónico. Aunque no incluya una imagen, de forma predeterminada Marketo inserta un solo píxel de seguimiento en todos los correos electrónicos HTML. |
   |---|---|
   | **Clics** | De forma predeterminada, los vínculos de los mensajes de correo electrónico tienen un seguimiento incrustado que permite ver quién hizo clic en qué vínculo, cuántos vínculos totales se pulsaron, etc. |
   | **Haga clic para abrir %** | Porcentaje de correos electrónicos que se abrieron y en los que se hizo clic en un vínculo en el correo electrónico. Esto mide la relevancia y el contexto de un mensaje de correo electrónico al tomar el número de clics únicos dividido por el número de aperturas únicas y multiplicarse por 100 para mostrarlo como porcentaje. |
   | **Puntuación de participación** | La [puntuación de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md) le ayuda a determinar la eficacia del contenido. |

   >[!TIP]
   >
   >Si elige Puntuación de participación, la prueba tendrá que ejecutarse durante al menos 24 horas. Obtenga más información sobre [cómo comprender la puntuación de participación](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md).

1. También puede personalizar sus criterios seleccionando Conversión personalizada y haciendo clic en Editar.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >La conversión personalizada permite elegir cualquier evento como conversión mediante déclencheur y filtros.

1. Se abrirá una ventana. Busque el déclencheur que desee y arrástrelo al lienzo.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Defina el déclencheur.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo solo permitirá déclencheur para las personas que hayan recibido el correo electrónico desde este programa de correo electrónico. No es necesario agregar el filtro &quot;Se envió correo electrónico&quot;.

1. Haga clic en **Cerrar**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   ¡bueno! Ahora es el momento de decidir cómo se determina al ganador.

## Declarar ganador {#declare-winner}

1. Elija una de las dos opciones disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Si está realizando una **prueba A/B de fecha y hora**, sólo puede elegir **Manual**.

   Una vez finalizada la prueba A/B, Marketo puede enviar automáticamente el correo electrónico ganador a la hora programada, o puede revisar los resultados y decidir qué correo electrónico se envía.

1. Automático es impresionante y es la opción predeterminada. Haga clic en **Siguiente**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Si elige **Manual** se enviará la prueba y esperará a que declare un ganador. Recibirá un informe de los resultados.

¡Perfecto! Ahora vamos a [programar la prueba A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md).
