---
unique-page-id: 2359947
description: 'Transición de personas entre flujos de participación: documentos de Marketo: documentación del producto'
title: Transición de personas entre flujos de participación
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Transición de personas entre flujos de participación {#transition-people-between-engagement-streams}

Los programas de participación pueden tener más de un flujo. Si [añadir una secuencia](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), tendrá que definir la forma en que las personas podrán moverse de un flujo a otro. Estos se llaman **reglas de transición.**

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione su programa de participación multiflujo y vaya a **Transmisiones**.

   ![](assets/multistream.jpg)

1. Haga clic en **Reglas de transición** para el flujo al que desee extraer de otros flujos, haga clic en **Editar reglas de transición**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Las reglas de transición se arrastran a un flujo; defina siempre las reglas del flujo que desee extraer.

   Una vez que se abra la ventana de la regla de transición, busque y arrastre el déclencheur que desee. En este caso, queremos mover personas a la fase intermedia cuando se añada a una oportunidad.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Vamos a establecer el operador en **es cualquiera** para que la gente pase por cualquier oportunidad añadida.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Puede agregar varios déclencheur y filtros a una regla de transición, pero esta utiliza todos los filtros (la única opción es usar TODOS los filtros). Si necesita utilizar O en una regla de transición, le recomendamos que configure una campaña inteligente externa en su lugar.

1. Haga clic en **Cerrar**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   ¡Excelente! Ahora, cualquier persona del programa de participación que se agregue a una oportunidad se moverá al flujo de Etapa media.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Los pasos descritos anteriormente *do* se aplican a las personas que [al pausar](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) también.
