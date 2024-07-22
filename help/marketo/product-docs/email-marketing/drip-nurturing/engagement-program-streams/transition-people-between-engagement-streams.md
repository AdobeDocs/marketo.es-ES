---
unique-page-id: 2359947
description: Transición de personas entre flujos de participación - Documentos de Marketo - Documentación del producto
title: Transición de personas entre flujos de participación
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Transición de personas entre flujos de participación {#transition-people-between-engagement-streams}

Los programas de participación pueden tener más de un flujo. Si [agrega una secuencia](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), querrá definir una forma para que las personas se muevan de una secuencia a otra. Se denominan **reglas de transición.**

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione su programa de participación de varias transmisiones y vaya a **Transmisiones**.

   ![](assets/multistream.jpg)

1. Haga clic en **Reglas de transición** para el flujo que quiera extraer de otros flujos y luego haga clic en **Editar reglas de transición**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Las reglas de transición entran en un flujo; defina siempre las reglas del flujo en el que desee entrar.

   Una vez abierta la ventana de la regla de transición, busque y arrastre el déclencheur que desee. En este caso, queremos mover a las personas a la fase intermedia cuando se añada a una oportunidad.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Establezcamos el operador en **is any** para que las personas se trasladen para cualquier oportunidad agregada.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Puede añadir varios déclencheur y filtros a una regla de transición, pero la regla de transición utiliza todos los filtros (el uso de TODOS los filtros es la única opción). Si necesita utilizar OR en una regla de transición, le recomendamos que configure una campaña inteligente externa en su lugar.

1. Haga clic en **Cerrar**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   ¡Excelente! Ahora, cualquier persona del programa de participación que se añada a una oportunidad se moverá al flujo de fase intermedia.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Los pasos descritos anteriormente *do* se aplican a las personas que están [en pausa](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) también.
