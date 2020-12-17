---
unique-page-id: 14352482
description: Cómo funciona el seguimiento de respuestas - Documentos de marketing - Documentación del producto
title: Funcionamiento del seguimiento de respuestas
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Cómo funciona el seguimiento de respuestas {#how-reply-tracking-works}

El seguimiento de respuestas se realiza mirando un ID de mensaje que se encuentra en cada correo electrónico enviado. Cada correo electrónico contiene un ID de mensaje único que nos permite tener uno de los mejores seguimientos de respuesta.

>[!PREREQUISITES]
>
>**Conexión con el servidor de correo electrónico:** Sales Connect debe estar conectado con su bandeja de entrada para que sepamos cuándo ha llegado una nueva respuesta. Necesitará tener su cuenta de Sales Connect [conectada a Gmail](http://docs.marketo.com/x/kYMOAQ). Si utiliza Outlook, necesitaremos integrarlo con su [servidor de intercambio](http://toutapp.com/next#settings/exchange_settings).

Si Sales Connect no puede realizar el seguimiento de la respuesta del cliente potencial a su correo electrónico, no podrá detener una campaña basada en la detección de respuestas o registrar esa respuesta en Salesforce.  ¿Qué significa que cualquier dirección de correo electrónico puede responder?

Esto significa que si envía un mensaje de correo electrónico [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) y responde con [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad), podemos rastrear la respuesta. Además, si envía un mensaje de correo electrónico [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) y CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153) y Alan lo vuelve a escribir, también detectará la respuesta y finalizará la campaña.
