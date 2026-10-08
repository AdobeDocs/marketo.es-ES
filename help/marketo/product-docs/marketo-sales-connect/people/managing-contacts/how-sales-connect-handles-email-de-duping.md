---
unique-page-id: 14352514
description: Descubra cómo Sales Connect gestiona la desduplicación de correo electrónico. Obtenga información sobre cómo se combinan o administran los contactos duplicados al sincronizar.
title: Cómo gestiona Sales Connect la eliminación de duplicados de correo electrónico
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
TQID: 'https://experienceleague.adobe.com/gO6I2rCotAEDOGQNdRleeJbqMIix1wQizZe84JZSLPs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: ab9cc269-26ac-5c58-b645-e0736aefe9f3
    internal-label: Marketo Sales Connect
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 6%
---
# Cómo administra [!DNL Sales Connect] la desduplicación de correo electrónico {#how-sales-connect-handles-email-de-duping}

Cuando [está cargando un archivo CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) en [!DNL Sales Connect], combinamos todos como contactos en el CSV antes de que se realice la importación.

Esto se basa en direcciones de correo electrónico similares. Por lo tanto, si hay dos direcciones de correo electrónico idénticas, las combinamos en un contacto.

Si más adelante intenta agregar o cargar manualmente el mismo contacto, no lo combinaremos.

Si intenta agregar un contacto que ya está en la base de datos, evitaremos que lo agregue.
