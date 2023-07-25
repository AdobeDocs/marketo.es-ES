---
unique-page-id: 557322
description: 'Ejecución de un solo paso de flujo desde una lista inteligente: documentos de Marketo, documentación del producto'
title: Ejecutar un solo paso de flujo desde una lista inteligente
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# Ejecutar un solo paso de flujo desde una lista inteligente {#run-a-single-flow-step-from-a-smart-list}

Si desea ejecutar un paso de flujo de solo una vez, puede utilizar un solo paso de flujo dentro de una lista inteligente en lugar de crear una campaña inteligente completa.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Ir a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione una lista o lista inteligente con personas y, a continuación, vaya a **People** pestaña.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Tanto las listas estáticas como las listas inteligentes tienen esta funcionalidad.

1. Clic **Seleccionar todo**. También puede utilizar **Ctrl/Cmd** y haga clic en para seleccionar algunos registros manualmente.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Si los resultados se extienden por varias páginas, haga clic en **Seleccionar todo** seleccionará todas las personas en todas las páginas.

1. En **Persona** **Acciones**, seleccione el paso de flujo que desee. En este ejemplo utilizaremos [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Busque y seleccione un **Atributo**. En este ejemplo, tomaremos todas las personas que tengan el estado &quot;California&quot; y lo cambiaremos a &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Introduzca un nuevo valor. Clic **Ejecutar ahora**.

   ![](assets/runactionnewvalue-hands.png)

1. Si va a cambiar los valores de los datos de un gran número de personas, es posible que tenga que confirmar el cambio escribiendo el número. Clic **Ir a por él**.

   ![](assets/changedatavalue.jpg)

¡Increíble trabajo! Verá el estado del paso de un solo flujo en la esquina superior derecha.

![](assets/completesingleflowaction.jpg)

Cuando haya terminado, actualice la lista y verá la información actualizada.
