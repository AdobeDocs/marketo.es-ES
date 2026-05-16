---
unique-page-id: 4719312
description: Obtenga información sobre cómo añadir y eliminar valores de la lista de selección de Salesforce y cómo afectan a Marketo. Agregue nuevos valores a los formularios desde las notificaciones y elimine los valores manualmente cuando sea necesario.
title: Añadir o quitar valores de la lista de selección
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/dKioXsrR-JTWPgJdoLx70Dw4M56G1X6kMLL1HEO5ZTM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 3%

---

# Añadir o quitar valores de la lista de selección {#add-remove-picklist-values}

A continuación se indican algunas cosas que hay que saber acerca de cómo agregar y quitar valores de listas de selección en [!DNL Salesforce].

## Adición de Valores de Lista {#adding-picklist-values}

1. Si se agrega un valor adicional en Salesforce a un tipo de campo de lista desplegable, recibirá una [notificación](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} que indica a qué formularios afectará esto.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Vaya al editor de formularios y [agregue el valor adicional](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} a su lista de sugerencias.

## Eliminar valores de la lista desplegable {#remove-picklist-values}

Cuando se quita un valor de la lista de selección de un campo de [!DNL Salesforce], tendrá que quitar manualmente este valor de todos los formularios que alojen este campo.

>[!NOTE]
>
>Si un campo de posible cliente y un campo de contacto en Salesforce tienen valores diferentes, los valores en común estarán disponibles para usarlos en Marketo Engage.

Si un campo de posible cliente y un campo de contacto de [!DNL Salesforce] tienen valores diferentes:

1. Si se añade un valor adicional en SFDC a una lista de selección, se recibirá una notificación.
1. La notificación le indicará dónde se utiliza. Ahora puede agregar este nuevo valor como opción en el formulario si lo desea.

Si una lista de selección de un posible cliente de SFDC tiene valores diferentes a los de una lista de selección para un contacto de SFDC, los valores comunes se utilizarán como opciones de valor predeterminadas en el formulario.

Si se elimina un valor de una lista de selección, se deberá eliminar manualmente como opción de los formularios.
