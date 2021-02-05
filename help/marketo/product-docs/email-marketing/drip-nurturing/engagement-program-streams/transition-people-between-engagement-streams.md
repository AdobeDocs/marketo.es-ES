---
unique-page-id: 2359947
description: Transición de personas entre flujos de participación - Documentos de marketing - Documentación del producto
title: Transición de personas entre flujos de participación
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# Transición de personas entre flujos de participación {#transition-people-between-engagement-streams}

Los programas de participación pueden tener más de un flujo. Si [agrega un flujo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), querrá definir una manera de que las personas se muevan de un flujo a otro. Se llaman **reglas de transición.**

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Seleccione el programa de participación de varios flujos y vaya a **Flujos**.

   ![](assets/multistream.jpg)

1. Haga clic en **Reglas de Transición** para el flujo que desee extraer de otros flujos y, a continuación, haga clic en **Editar reglas de Transición**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >las reglas de transición se arrastran a un flujo; defina siempre las reglas en el flujo en el que desee extraer.

   Una vez que se abra la ventana de la regla de transición, busque y arrastre el déclencheur que desee. En este caso, queremos mover a las personas a la Etapa media cuando se añada a una oportunidad.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Vamos a establecer el operador en **es cualquier** para que las personas se muevan para cualquier oportunidad agregada.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Puede agregar varios déclencheur y filtros a una regla de transición, pero la regla de transición utiliza todos los filtros (la única opción es usar TODOS los filtros). Si necesita utilizar O en una regla de transición, le recomendamos que configure una campaña inteligente externa.

1. Haga clic en **Cerrar**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   ¡bueno! Ahora cualquier persona del programa de participación que se agregue a una oportunidad se moverá al flujo de la fase media.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Los pasos descritos anteriormente *do* se aplican también a las personas que estén [en pausa](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
