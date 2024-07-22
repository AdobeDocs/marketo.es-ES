---
description: '¿Cómo Gestionan Las Acciones De Perspectiva De Ventas La Desduplicación De Correo Electrónico? Documentos De Marketo: Documentación Del Producto'
title: ¿Cómo Gestionan Las Acciones De Perspectiva De Ventas La Desduplicación De Correo Electrónico?
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# ¿Cómo Gestionan Las Acciones De Perspectiva De Ventas La Desduplicación De Correo Electrónico? {#how-does-sales-insight-actions-handle-email-de-duping}

Cuando [está cargando un archivo CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) en acciones de información de ventas, combinamos todos los contactos similares en el CSV antes de que se realice la importación.

Esto se basa en direcciones de correo electrónico similares. Por lo tanto, si hay dos direcciones de correo electrónico idénticas, las combinamos en un contacto.

Si más adelante intenta agregar o cargar manualmente el mismo contacto, no lo combinaremos.

Si intenta agregar un contacto que ya está en la base de datos, evitaremos que lo agregue.
