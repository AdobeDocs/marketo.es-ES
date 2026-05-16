---
unique-page-id: 1147324
description: Aprenda a borrar valores de campo en un paso del flujo de Smart Campaign. Elimine valores de los campos de persona o empresa.
title: Borrar valores de campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/57QZb7T-y2JVdNeP4nhTl9PDjIX1S9GcQmRAMJ-53E0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 106
ht-degree: 5%

---

# Borrar valores de campo {#clear-field-values}

[Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) es genial, pero ¿cómo _quitas_ el valor por completo? ¡Buena pregunta!

1. En el paso de flujo, elija el campo que desea borrar y escriba **[!UICONTROL NULL]** (mayúsculas) como **[!UICONTROL Nuevo valor]**.

   ![](assets/clear-field-values-1.png)

1. Una vez finalizado el paso de flujo, se borra el valor del campo seleccionado.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Si deja el nuevo valor en blanco o introduce un ESPACIO, el campo no se vaciará. Tiene que escribir NULL. Además, recuerde, los pasos de flujo no se pueden deshacer después de ejecutar.
