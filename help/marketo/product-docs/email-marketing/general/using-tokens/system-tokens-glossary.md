---
unique-page-id: 1147344
description: Glosario de tokens del sistema - Documentos de Marketo - Documentación del producto
title: Glosario de tokens del sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Glosario de tokens del sistema {#system-tokens-glossary}

Además de los tokens de persona, puede utilizar algunos tokens de sistema muy interesantes. Aquí están.

>[!NOTE]
>
>La configuración de la zona horaria de la cuenta se ve afectada cuando se ejecutan los tokens de fecha y hora.

## system.date {#system-date}

El `{{system.date}}` El token procesará la fecha actual en tiempo de ejecución de la siguiente manera: **8 de agosto de 2013**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} paso de flujo
* [Momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} paso de flujo
* [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} paso de flujo
* Cuerpo de un correo electrónico o una plantilla

## system.time {#system-time}

El `{{system.time}}` El token procesará la hora actual en tiempo de ejecución de la siguiente manera: **16:34 (GMT -0700)**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} paso de flujo
* [Momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} paso de flujo
* [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} paso de flujo
* Cuerpo de un correo electrónico o una plantilla

## system.dateTime {#system-datetime}

El `{{system.dateTime}}` El token procesará la fecha y la hora actuales en tiempo de ejecución de la siguiente manera: **08-08-2013 16:36:13**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} paso de flujo
* [Momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} paso de flujo
* [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} paso de flujo
* Cuerpo de un correo electrónico o una plantilla

## system.forwardToFriendLink {#system-forwardtofriendlink}

El `{{system.forwardToFriendLink}}` token permite controlar la colocación de la variable [&quot;Reenviar a un vínculo de amigo&quot; en correos electrónicos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Funciona en:**

* [Añadir un token de sistema como vínculo en un correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o plantilla

## system.unsubscribeLink {#system-unsubscribelink}

El `{{system.unsubscribeLink}}` Este token permite controlar la ubicación del vínculo de cancelación de suscripción en un correo electrónico.

**Funciona en:**

* [Añadir un token de sistema como vínculo en un correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o plantilla

## system.viewAsWebpageLink {#system-viewaswebpagelink}

El `{{system.viewAsWebpageLink}}` Este token permite controlar la ubicación del vínculo Ver como página web en un mensaje de correo electrónico.

**Funciona con:**

* [Añadir un token de sistema como vínculo en un correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o plantilla
