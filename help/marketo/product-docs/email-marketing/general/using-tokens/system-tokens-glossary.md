---
unique-page-id: 1147344
description: Glosario de tokens del sistema - Documentos de Marketo - Documentación del producto
title: Glosario de tokens del sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
source-git-commit: 93032a016a67fe0edf7a8093633d6b06ec25c18d
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Glosario de tokens del sistema {#system-tokens-glossary}

Además de los tokens de persona, puede utilizar algunos tokens de sistema realmente geniales. Aquí están.

>[!NOTE]
>
>La configuración del huso horario de la cuenta afecta al momento en que se ejecutan los tokens de fecha y hora.

## system.date {#system-date}

La variable `{{system.date}}` El token mostrará la fecha actual en tiempo de ejecución de la siguiente manera: **8 de agosto de 2013**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} paso de flujo
* [Momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} paso de flujo
* [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} paso de flujo
* El cuerpo de un correo electrónico o una plantilla

## system.time {#system-time}

La variable `{{system.time}}` representará así la hora actual en tiempo de ejecución: **04:34 PM (GMT -0700)**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} paso de flujo
* [Momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} paso de flujo
* [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} paso de flujo
* El cuerpo de un correo electrónico o una plantilla

## system.dateTime {#system-datetime}

La variable `{{system.dateTime}}` representará la fecha y la hora actuales en tiempo de ejecución de la siguiente manera: **2013-08-08 18:36:13**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} paso de flujo
* [Momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} paso de flujo
* [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} paso de flujo
* El cuerpo de un correo electrónico o una plantilla

## system.forwardToFriendLink {#system-forwardtofriendlink}

La variable `{{system.forwardToFriendLink}}` permite controlar la colocación de la variable [&quot;Reenviar a un vínculo de amigo&quot; en correos electrónicos](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target=&quot;_blank&quot;}.

**Funciona en:**

* [Añadir un token del sistema como vínculo en un correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} o plantilla

## system.unsubscribeLink {#system-unsubscribelink}

La variable `{{system.unsubscribeLink}}` token le permite controlar la ubicación del vínculo de cancelación de suscripción en un correo electrónico.

**Funciona en:**

* [Añadir un token del sistema como vínculo en un correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} o plantilla

## system.viewAsWebpageLink {#system-viewaswebpagelink}

La variable `{{system.viewAsWebpageLink}}` permite controlar la colocación del vínculo Ver como página web en un correo electrónico.

**Funciona con:**

* [Añadir un token del sistema como vínculo en un correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} o plantilla
