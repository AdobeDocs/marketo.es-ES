---
unique-page-id: 14352482
description: Descubra cómo funciona el seguimiento de respuestas en Sales Connect. Obtenga información sobre cómo se detectan y registran las respuestas en Salesforce o Marketo.
title: Cómo funciona el seguimiento de respuestas
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 4%

---

# Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que aparece en cada correo electrónico que envía. Cada correo electrónico contiene un ID de mensaje único que nos permite tener algunos de los mejores resultados de seguimiento de respuestas.

>[!PREREQUISITES]
>
>**La conexión con el servidor de correo electrónico:** [!DNL Sales Connect] debe estar conectada con su bandeja de entrada para que sepamos cuándo ha llegado una nueva respuesta. Necesitarás tener tu cuenta de [!DNL Sales Connect] [conectada a Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si usas [!DNL Outlook], necesitaremos integrarlo con tu [servidor de Exchange](https://toutapp.com/next#settings/exchange_settings).

Si [!DNL Sales Connect] no puede rastrear la respuesta de su posible cliente a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas ni registrar esa respuesta a [!DNL Salesforce].  ¿Qué significa que cualquier dirección de correo electrónico puede responder?

Esto significa que si envía un correo electrónico a <flynn@flynnsarcade.com> y él responde con <kevinf@flynnsarcade.com>, podremos realizar un seguimiento de la respuesta. Además, si envía un correo electrónico a <flynn@flynnsarcade.com> y CC <alan@encom.com>, y Alan le devuelve una respuesta, también detectará la respuesta y finalizará la campaña.
