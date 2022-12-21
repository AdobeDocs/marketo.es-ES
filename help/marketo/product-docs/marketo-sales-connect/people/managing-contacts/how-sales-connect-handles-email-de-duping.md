---
unique-page-id: 14352514
description: Cómo gestiona la conexión de ventas la desduplicación de correos electrónicos - Documentos de Marketo - Documentación del producto
title: Cómo gestiona la conexión de ventas la desduplicación de correos electrónicos
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Cómo gestiona la conexión de ventas la desduplicación de correos electrónicos {#how-sales-connect-handles-email-de-duping}

Cuando [carga de un CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) en Sales Connect, combinamos todos como contactos en el CSV antes de que se realice la importación.

Lo hacemos en función de direcciones de correo electrónico similares. Por lo tanto, si hay dos direcciones de correo electrónico idénticas, las combinamos en un contacto.

Si más adelante intenta agregar o cargar manualmente el mismo contacto, no lo combinaremos.

Si intenta agregar un contacto que ya está en la base de datos, evitaremos que lo agregue.
