---
unique-page-id: 1147324
description: Aprenda a borrar valores de campo en un paso del flujo de Smart Campaign. Elimine valores de los campos de persona o empresa.
title: Borrar valores de campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '107'
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
   >Si deja el nuevo valor en blanco o simplemente introduce un ESPACIO, el campo no se vaciará. Tiene que escribir NULL. Además, recuerde, los pasos de flujo no se pueden deshacer después de ejecutar.
