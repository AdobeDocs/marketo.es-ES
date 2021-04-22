---
unique-page-id: 4719312
description: Agregar o eliminar valores de listas de reproducción - Documentos de Marketo - Documentación del producto
title: Agregar o eliminar valores de listas de reproducción
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Agregar o eliminar valores de listas de reproducción {#add-remove-picklist-values}

A continuación se indican algunas cosas que debe tener en cuenta al agregar y eliminar valores de listas de selección en Salesforce.

## Adición de valores de lista de reproducción {#adding-picklist-values}

1. Si se agrega un valor adicional en Salesforce a un tipo de campo de lista de selección, recibirá una [notificación](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) que identifica a qué formularios afectará esto.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Vaya al editor de formularios y [añada el valor adicional](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) a su lista de sugerencias.

## Eliminar valores de lista de reproducción {#remove-picklist-values}

Cuando se elimina un valor de la lista de selección de un campo de Salesforce, deberá eliminar manualmente este valor de todos los formularios que alojen este campo.

>[!NOTE]
>
>Si un campo de posible cliente y un campo de contacto de Salesforce tienen valores diferentes, los valores comunes estarán disponibles para su uso en Marketo.

Si un campo de posible cliente y un campo de contacto de Salesforce tienen valores diferentes:

1. Añadir un valor adicional en SFDC a una lista de selección obtendrá una notificación.
1. La notificación le indicará dónde se utiliza. Ahora puede agregar este nuevo valor como una opción en el formulario si lo desea.

Si una lista de selección de un posible cliente de SFDC tiene valores diferentes a una lista de selección para un contacto de SFDC, los valores comunes se utilizarán como opciones de valor predeterminadas en el formulario.

Si quita un valor de una lista de selección, deberá eliminarlo manualmente como opción de los formularios.
