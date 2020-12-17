---
unique-page-id: 14352514
description: Cómo gestiona Sales Connect la eliminación de la copia de seguridad por correo electrónico - Documentos de marketing - Documentación del producto
title: Cómo gestiona Sales Connect la desduplicación de correos electrónicos
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Cómo gestiona Sales Connect la desduplicación de correos electrónicos {#how-sales-connect-handles-email-de-duping}

Cuando [carga un archivo CSV](http://docs.marketo.com/x/VADb) en Sales Connect, combinamos todos como contactos en el CSV antes de que se realice la importación.

Lo hacemos en base a direcciones de correo electrónico similares. Si hay dos direcciones de correo electrónico idénticas, las combinamos en un solo contacto.

Si más adelante intenta agregar o cargar manualmente el mismo contacto, no lo combinaremos.

Si intenta agregar un contacto que ya se encuentra en la base de datos, le impediremos agregarlo.

