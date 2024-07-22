---
unique-page-id: 14352482
description: Funcionamiento del seguimiento de respuestas - Documentos de Marketo - Documentación del producto
title: Funcionamiento del seguimiento de respuestas
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Funcionamiento del seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que aparece en cada correo electrónico que envía. Cada correo electrónico contiene un ID de mensaje único que nos permite tener algunos de los mejores resultados de seguimiento de respuestas.

>[!PREREQUISITES]
>
>**Conexión con el servidor de correo electrónico:** Sales Connect debe estar conectado a su bandeja de entrada para que sepamos cuándo ha llegado una nueva respuesta. Necesitarás tener tu cuenta de Sales Connect [conectada a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si utiliza Outlook, tendremos que integrarlo con su [servidor de Exchange](https://toutapp.com/next#settings/exchange_settings).

Si Sales Connect no puede rastrear la respuesta de su posible cliente a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas ni registrar esa respuesta en Salesforce.  ¿Qué significa que cualquier dirección de correo electrónico puede responder?

Esto significa que si envía un correo electrónico a flynn@flynnsarcade.com y él responde con kevinf@flynnsarcade.com, podemos rastrear la respuesta. Además, si envías un correo electrónico a flynn@flynnsarcade.com y CC alan@encom.com, y Alan te devuelve una respuesta, también detectará la respuesta y finalizará la campaña.
