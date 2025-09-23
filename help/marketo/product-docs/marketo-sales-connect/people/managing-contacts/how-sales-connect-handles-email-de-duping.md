---
unique-page-id: 14352514
description: 'Cómo gestiona Sales Connect la desduplicación de correo electrónico: Documentos de Marketo: documentación del producto'
title: Cómo gestiona Sales Connect la eliminación de duplicados de correo electrónico
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 6%

---

# Cómo administra [!DNL Sales Connect] la desduplicación de correo electrónico {#how-sales-connect-handles-email-de-duping}

Cuando [está cargando un archivo CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) en [!DNL Sales Connect], combinamos todos como contactos en el CSV antes de que se realice la importación.

Esto se basa en direcciones de correo electrónico similares. Por lo tanto, si hay dos direcciones de correo electrónico idénticas, las combinamos en un contacto.

Si más adelante intenta agregar o cargar manualmente el mismo contacto, no lo combinaremos.

Si intenta agregar un contacto que ya está en la base de datos, evitaremos que lo agregue.
