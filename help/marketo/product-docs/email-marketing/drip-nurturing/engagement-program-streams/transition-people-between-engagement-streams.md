---
unique-page-id: 2359947
description: Aprenda a configurar reglas de transición para mover a las personas entre flujos de participación. Defina las reglas en el flujo al que desee extraer.
title: Transición de personas entre flujos de participación
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/viGLYAkvGqF-9K5bhAHWDSOMYaiBuKRe8F2QginuYps
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 6%

---

# Transición de personas entre flujos de participación {#transition-people-between-engagement-streams}

Los programas de participación pueden tener más de un flujo. Si [agrega una secuencia](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), defina la forma en que las personas puedan pasar de una secuencia a otra. Se denominan **reglas de transición.**

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/ma.png)

1. Seleccione su programa de participación de varias transmisiones y vaya a **[!UICONTROL Transmisiones]**.

   ![](assets/multistream.jpg)

1. Haga clic en **[!UICONTROL Reglas de transición]** para el flujo que quiera extraer de otros flujos y luego haga clic en **[!UICONTROL Editar reglas de transición]**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Las reglas de transición entran en un flujo; defina siempre las reglas del flujo en el que desee entrar.

   Una vez abierta la ventana de la regla de transición, busque y arrastre el déclencheur que desee. En este ejemplo, las personas se moverán a la [!UICONTROL etapa intermedia] cuando se agreguen a una oportunidad.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Establezca el operador en **[!UICONTROL is any]** para que las personas se muevan para cualquier oportunidad agregada.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Puede añadir varios déclencheur y filtros a una regla de transición, pero la regla de transición utiliza todos los filtros (el uso de TODOS los filtros es la única opción). Si necesita utilizar OR en una regla de transición, se recomienda configurar una campaña inteligente externa en su lugar.

1. Haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Ahora, cualquier persona del programa de participación que se agregue a una oportunidad se moverá al flujo de [!UICONTROL Etapa intermedia].

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Los pasos descritos anteriormente *do* se aplican a las personas que están [en pausa](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) también.
