---
unique-page-id: 14352482
description: Cómo funciona el seguimiento de respuestas - Documentos de marketing - Documentación del producto
title: Funcionamiento del seguimiento de respuestas
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que se encuentra en cada correo electrónico enviado. Cada correo electrónico contiene un ID de mensaje único que nos permite tener uno de los mejores seguimientos de respuesta.

>[!PREREQUISITES]
>
>**Conexión con el servidor de correo electrónico:** Sales Connect debe estar conectado con su bandeja de entrada para que sepamos cuándo ha llegado una nueva respuesta. Necesitará tener su cuenta de Sales Connect [conectada a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-tab-for-gmail-users.md). Si utiliza Outlook, necesitaremos integrarlo con su [servidor de intercambio](https://toutapp.com/next#settings/exchange_settings).

Si Sales Connect no puede realizar el seguimiento de la respuesta del cliente potencial a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas o registrar esa respuesta en Salesforce.  ¿Qué significa que cualquier dirección de correo electrónico puede responder?

Esto significa que si envía un correo electrónico a flynn@flynnsarcade.com y responde con kevinf@flynnsarcade.com, podemos rastrear la respuesta. Además, si envía un correo electrónico a flynn@flynnsarcade.com y a CC alan@encom.com, y Alan le escribe nuevamente, también detectará la respuesta y finalizará la campaña.
