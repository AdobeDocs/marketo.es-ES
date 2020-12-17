---
unique-page-id: 4719312
description: Añadir/eliminar valores de listas de reproducción - Documentos de marketing - Documentación del producto
title: Añadir/Eliminar valores de lista de selección
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Añadir/Eliminar valores de lista de reproducción {#add-remove-picklist-values}

A continuación se indican algunas cosas que debe saber sobre la adición y eliminación de valores de listas de selección en Salesforce.

## Añadir valores de lista de reproducción {#adding-picklist-values}

1. Si se agrega un valor adicional en Salesforce a un tipo de campo de lista de selección, recibirá una [notificación](../../../product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) que identifica los formularios que esto afectará.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Vaya al editor de formularios y [agregue el valor adicional](../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) a la lista de sugerencias.

## Eliminar valores de lista de reproducción {#remove-picklist-values}

Cuando se elimina un valor de lista de selección de un campo de Salesforce, deberá quitar manualmente este valor de todos los formularios que tengan este campo.

>[!NOTE]
>
>Si un campo de posible cliente y un campo de contacto de Salesforce tienen valores diferentes, los valores en común estarán disponibles para su uso en Marketing.

Si un campo de posible cliente y un campo de contacto de Salesforce tienen valores diferentes:

1. Añadir un valor adicional en SFDC a una lista de selección obtendrá una notificación.
1. La notificación le indicará dónde se utiliza. Ahora puede agregar este nuevo valor como opción en el formulario si lo desea.

Si una lista de selección de un lead SFDC tiene valores diferentes a una lista de selección para un contacto SFDC, los valores comunes se utilizarán como opciones de valor predeterminadas en el formulario.

Si elimina un valor de una lista de selección, deberá eliminarlo manualmente como opción de los formularios.
