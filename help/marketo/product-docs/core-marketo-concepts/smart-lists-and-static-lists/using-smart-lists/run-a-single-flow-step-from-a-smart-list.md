---
unique-page-id: 557322
description: 'Ejecutar un solo paso de flujo desde una lista inteligente: Documentos de Marketo: Documentación del producto'
title: Ejecutar un solo paso de flujo desde una lista inteligente
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# Ejecutar un solo paso de flujo desde una lista inteligente {#run-a-single-flow-step-from-a-smart-list}

Si desea ejecutar un paso de flujo único, puede utilizar un solo paso de flujo dentro de una lista inteligente en lugar de crear una campaña inteligente completa.

>[!PREREQUISITES]
>
>[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione una lista o lista inteligente con personas incluidas y vaya a la **People** pestaña .

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Tanto las listas estáticas como las listas inteligentes tienen esta funcionalidad.

1. Haga clic en **Seleccionar todo**. También puede utilizar **Ctrl/Cmd** y haga clic en para seleccionar algunos registros manualmente.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Si los resultados abarcan varias páginas, haga clic en **Seleccionar todo** seleccionará a todas las personas de todas las páginas.

1. En **Persona** **Acciones**, seleccione el paso de flujo que desee. En este ejemplo usaremos [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Busque y seleccione un **Atributo**. En este ejemplo tomaremos todas las personas que tengan el estado &quot;California&quot; y lo cambiaremos a &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Introduzca un nuevo valor. Haga clic en **Ejecutar ahora**.

   ![](assets/runactionnewvalue-hands.png)

1. Si está cambiando los valores de los datos de un gran número de personas, es posible que tenga que confirmar el cambio escribiendo el número. Haga clic en **Vaya a**.

   ![](assets/changedatavalue.jpg)

¡Increíble trabajo! Verá el estado del paso de flujo único en la esquina superior derecha.

![](assets/completesingleflowaction.jpg)

Cuando termine, actualice la lista y verá la información actualizada.
