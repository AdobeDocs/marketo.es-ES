---
unique-page-id: 1147344
description: Glosario de tokens del sistema - Documentos de Marketo - Documentación del producto
title: Glosario de tókenes del sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: bf420edcc79aa551e286302fa002df9162371873
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 2%

---

# Glosario de tókenes del sistema {#system-tokens-glossary}

Además de los tokens de persona, puede utilizar algunos tokens de sistema muy interesantes. Aquí están.

>[!NOTE]
>
>La configuración de la zona horaria de la cuenta se ve afectada cuando se ejecutan los tokens de fecha y hora.

## system.date {#system-date}

El token `{{system.date}}` procesará la fecha actual en tiempo de ejecución de la siguiente manera: **8 de agosto de 2013**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} paso de flujo
* Paso de flujo de [momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Paso de flujo [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Cuerpo de un correo electrónico o una plantilla

## system.time {#system-time}

El token `{{system.time}}` procesará la hora actual en tiempo de ejecución como: **04:34 PM (GMT -0700)**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} paso de flujo
* Paso de flujo de [momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Paso de flujo [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Cuerpo de un correo electrónico o una plantilla

## system.dateTime {#system-datetime}

El token `{{system.dateTime}}` procesará la fecha y hora actuales en tiempo de ejecución de la siguiente manera: **2013-08-08 16:36:13**

**Funciona en:**

* [Cambiar valor de datos](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} paso de flujo
* Paso de flujo de [momento interesante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Paso de flujo [Crear tarea](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Cuerpo de un correo electrónico o una plantilla

## system.unsubscribeLink {#system-unsubscribelink}

El token `{{system.unsubscribeLink}}` le permite controlar la ubicación del vínculo de cancelación de suscripción en un mensaje de correo electrónico.

**Funciona en:**

* [Agregar un token de sistema como un vínculo en un mensaje de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o plantilla

## system.viewAsWebpageLink {#system-viewaswebpagelink}

El token `{{system.viewAsWebpageLink}}` le permite controlar la ubicación del vínculo Ver como página web en un mensaje de correo electrónico.

**Funciona con:**

* [Agregar un token de sistema como un vínculo en un mensaje de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o plantilla
