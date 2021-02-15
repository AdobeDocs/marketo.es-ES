---
unique-page-id: 14352509
description: Glosario de campos dinámicos - Documentos de marketing - Documentación del producto
title: Glosario de campos dinámicos
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Glosario de campos dinámicos {#dynamic-fields-glossary}

Al crear una plantilla en Sales Connect, siempre se recomienda integrar campos dinámicos mediante el botón **Campos dinámicos MSE**.

Esta herramienta se utiliza para `auto-personalize your email` y ahorrarle toneladas de tiempo por `pulling information from the People page`.

| Campo dinámico | Ejemplo de lo que aparece en el correo electrónico |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Si no quieres volver a escuchar de mí, por favor avísenme aquí |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Redactor técnico principal |
| `{{work_website}}` | https://www.marketo.com |

**Cosas a tener en cuenta**:

* Si la información de un contacto se introduce incorrectamente o falta en la página Personas, no se extraerá correctamente en la plantilla.
* La diferencia entre `{{company}}` y `{{company_friendly}}` es que `{{company_friendly}}` eliminará cualquier título formal, como Inc., LLC., etc., del nombre de la compañía de su contacto.
* Al utilizar `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los detalles de contacto. De este modo, Sales Connect sabe qué eliminar al extraer el valor.

>[!TIP]
>
>Puede crear su propio [campo dinámico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para todo aquello que desee que se incluya automáticamente en los correos electrónicos
