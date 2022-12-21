---
unique-page-id: 14352482
description: Cómo funciona el seguimiento de respuestas - Documentos de Marketo - Documentación del producto
title: Cómo funciona el seguimiento de respuestas
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que está en cada correo electrónico que envía. Cada correo electrónico contiene un ID de mensaje único que nos permite tener uno de los mejores seguimientos de respuestas.

>[!PREREQUISITES]
>
>**Conexión con el servidor de correo electrónico:** Sales Connect debe estar conectado a su bandeja de entrada para saber cuándo ha llegado una nueva respuesta. Necesitará tener su cuenta de Conexión de Ventas [conectado a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si utiliza Outlook, tendremos que integrarlo con su [servidor de intercambio](https://toutapp.com/next#settings/exchange_settings).

Si Sales Connect no puede rastrear la respuesta del cliente potencial a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas o en el registro de la respuesta a Salesforce.  ¿Qué queremos decir con cualquier dirección de correo electrónico que pueda responder?

Esto significa que si envía un correo electrónico a flynn@flynnsarcade.com y responde con kevinf@flynnsarcade.com, podemos rastrear la respuesta. Además, si envía un correo electrónico a flynn@flynnsarcade.com y a CC alan@encom.com, y Alan le reescribe, también detectará la respuesta y finalizará la campaña.
