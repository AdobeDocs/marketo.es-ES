---
unique-page-id: 1147324
description: Borrar valores de campo - Documentos de Marketo - Documentación del producto
title: Borrar valores de campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Borrar valores de campo {#clear-field-values}

[Cambiar ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) valores de datos es bueno, pero ¿cómo se  __ elimina completamente el valor? ¡Buena pregunta!

1. En el paso de flujo, elija el campo que desea borrar y escriba **NULL** (todos mayúsculas) como **Nuevo valor**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. ¡Boom! ¡Apuesto a que no lo sabías! Una vez finalizado el paso de flujo, se borra el valor del campo elegido.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Dejar el nuevo valor en blanco o simplemente entrar en un SPACE no vaciará realmente el campo. Debe escribir NULL. Además, recuerde que los pasos de flujo no se pueden deshacer después de ejecutarse.
