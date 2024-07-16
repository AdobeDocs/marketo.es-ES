---
unique-page-id: 1147324
description: Borrar valores de campo - Documentos de Marketo - Documentación del producto
title: Borrar valores de campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 7dd2e21969b71a50bfd4643ab15459150ca07c92
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Borrar valores de campo {#clear-field-values}

[Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) es genial, pero ¿cómo _quitas_ el valor por completo? ¡Buena pregunta!

1. En el paso de flujo, elija el campo que desea borrar y escriba **NULL** (mayúsculas) como **Nuevo valor**.

   ![](assets/clear-field-values-1.png)

1. ¡Boom! ¡Apuesto a que no lo sabías! Una vez finalizado el paso de flujo, se borra el valor del campo seleccionado.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Si deja el nuevo valor en blanco o simplemente introduce un ESPACIO, el campo no se vaciará. Tiene que escribir NULL. Además, recuerde, los pasos de flujo no se pueden deshacer después de ejecutar.
