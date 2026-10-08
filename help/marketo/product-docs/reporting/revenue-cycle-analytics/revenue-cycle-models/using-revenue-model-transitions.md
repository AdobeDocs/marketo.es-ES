---
unique-page-id: 4718672
description: Aprenda a utilizar las transiciones del modelo de ingresos en Marketo Engage mediante las transiciones del modelo de ingresos. Utilice esta guía para completar el siguiente paso.
title: Uso de transiciones del modelo de ingresos
exl-id: c658b631-b849-438a-b412-63ffd41e4c85
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 3%
---
# Uso de transiciones del modelo de ingresos {#using-revenue-model-transitions}

>[!PREREQUISITES]
>
>[Crear un nuevo modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-new-revenue-model.md)

Al crear el modelo y seleccionar y organizar las etapas del inventario, es hora de establecer las transiciones.

![](assets/one-2.png)

1. Haga clic con el botón derecho (también puede hacer doble clic) en una de las flechas para comenzar y seleccione **[!UICONTROL Editar transición]**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >No se pueden editar las reglas de transición &#39;[!UICONTROL Anonymous] ⇒ [!UICONTROL Known]&#39;.

1. Se abrirá una nueva pestaña para la transición seleccionada.

   ![](assets/three-1.png)

1. Las transiciones controlan cómo se mueven los posibles clientes entre etapas. Arrastre el déclencheur (o filtro) que desee desde la derecha y suéltelo en cualquier lugar del lienzo. En este ejemplo, seleccionaremos el déclencheur **[!UICONTROL Rellena formulario]**.

   >[!TIP]
   >
   >Dado que el modelador de ingresos le está configurando para la creación de informes, se recomienda que las transiciones siempre incluyan déclencheur. De este modo, los informes reflejarán la velocidad real del flujo de modelo/fase. Se pueden añadir filtros con los déclencheur para restricciones adicionales.

   ![](assets/four-2.png)

1. Elija los parámetros del déclencheur o filtro seleccionado.

   ![](assets/five-2.png)

1. Para volver al modelo, haz clic en **[!UICONTROL Modeler]**.

   ![](assets/six.png)

1. En la parte inferior de la pantalla, ahora verá las reglas de transición.

   ![](assets/seven.png)

1. Una vez que haya configurado las reglas para todas las transiciones, haga clic en **[!UICONTROL Validar]** para verificarlas.

   ![](assets/eight.png)

1. Si se realiza correctamente, verá el siguiente mensaje.

   ![](assets/nine.png)

¡Bien hecho! Ha modificado correctamente las transiciones del modelo.

>[!MORELIKETHIS]
>
>[Aprobar o desaprobar un modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)
