---
unique-page-id: 14352509
description: Glosario de campos dinámicos - Documentos de marketing - Documentación del producto
title: Glosario de campos dinámicos
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[protegido por correo electrónico]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | Redactor técnico principal |
| `{{work_website}}` | https://www.marketo.com |

**Cosas a tener en cuenta**:

* Si un contacto `information is entered incorrectly` o falta en la página Personas, `will not pull over correctly` se incluirá en la plantilla.

* La diferencia entre `{{company}}` y `{{company_friendly}}` es que `{{company_friendly}}` `remove any formal title`, como Inc., LLC., etc., se obtendrá a partir del nombre de la compañía de su contacto.
* Al utilizar `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los detalles de contacto. De este modo, Sales Connect sabe qué eliminar al extraer el valor.

>[!TIP]
>
>Puede crear su propio [campo dinámico personalizado](http://docs.marketo.com/x/fADb) para todo aquello que desee que se incluya automáticamente en los correos electrónicos

