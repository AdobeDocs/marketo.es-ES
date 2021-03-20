---
unique-page-id: 14352482
description: Cómo funciona el seguimiento de respuestas - Documentos de Marketo - Documentación del producto
title: Cómo funciona el seguimiento de respuestas
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que está en cada correo electrónico que envía. Cada correo electrónico contiene un ID de mensaje único que nos permite tener uno de los mejores seguimientos de respuestas.

>[!PREREQUISITES]
>
>**Conexión con el servidor de correo electrónico:** La conexión de ventas debe estar conectada con la bandeja de entrada para que sepamos cuándo llega una nueva respuesta. Tendrá que tener su cuenta de Conexión de ventas [conectada a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si utiliza Outlook, tendremos que integrarlo con su [servidor de intercambio](https://toutapp.com/next#settings/exchange_settings).

Si Sales Connect no puede rastrear la respuesta del cliente potencial a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas o en el registro de la respuesta a Salesforce.  ¿Qué queremos decir con cualquier dirección de correo electrónico que pueda responder?

Esto significa que si envía un correo electrónico a flynn@flynnsarcade.com y responde con kevinf@flynnsarcade.com, podemos rastrear la respuesta. Además, si envía un correo electrónico a flynn@flynnsarcade.com y a CC alan@encom.com, y Alan le reescribe, también detectará la respuesta y finalizará la campaña.
