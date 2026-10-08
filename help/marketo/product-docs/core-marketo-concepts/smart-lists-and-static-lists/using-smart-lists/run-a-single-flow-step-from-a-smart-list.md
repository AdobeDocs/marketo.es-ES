---
unique-page-id: 557322
description: Obtenga información sobre cómo ejecutar un solo paso de flujo desde una lista inteligente. Ejecutar una acción de flujo para las personas seleccionadas de la lista.
title: Ejecutar un solo paso de flujo desde una lista inteligente
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/GdWQiObUSnllii3M8x1bTuHRByAtg-UF03V-3sOuI9I'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 9%
---
# Ejecutar un solo paso de flujo desde una lista inteligente {#run-a-single-flow-step-from-a-smart-list}

Si desea ejecutar un paso de flujo de solo una vez, puede utilizar un solo paso de flujo dentro de una Smart List en lugar de crear una campaña inteligente completa.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-1.png)

1. Seleccione una lista o lista inteligente con personas y, a continuación, vaya a la ficha **[!UICONTROL Personas]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-2.png)

   >[!TIP]
   >
   >Tanto las listas estáticas como las listas inteligentes tienen esta funcionalidad.

1. Haga clic en **[!UICONTROL Seleccionar todo]**. También puede usar **Ctrl/Cmd** y hacer clic para seleccionar algunos registros manualmente.

   ![](assets/run-a-single-flow-step-from-a-smart-list-3.png)

   >[!NOTE]
   >
   >Si los resultados abarcan varias páginas, al hacer clic en **[!UICONTROL Seleccionar todo]** se seleccionarán todas las personas en todas las páginas.

1. En **[!UICONTROL Acciones de persona]**, seleccione el paso de flujo que desee. Este ejemplo usa [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}.

   ![](assets/run-a-single-flow-step-from-a-smart-list-4.png)

1. Busque y seleccione un **[!UICONTROL atributo]**. En este ejemplo, tomaremos todas las personas que tengan el estado &quot;California&quot; y lo cambiaremos a &quot;CA&quot;.

   ![](assets/run-a-single-flow-step-from-a-smart-list-5.png)

1. Introduzca un nuevo valor. Haga clic en **[!UICONTROL Ejecutar ahora]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-6.png)

1. Si está cambiando los valores de los datos de un gran número de personas, es posible que tenga que confirmar el cambio escribiendo el número. Haga Clic En **[!UICONTROL Ir A Por Él]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-7.png)

El estado del paso de un solo flujo aparecerá en la esquina superior derecha.

![](assets/run-a-single-flow-step-from-a-smart-list-8.png)

Cuando termine, actualice la lista y verá la información actualizada.
