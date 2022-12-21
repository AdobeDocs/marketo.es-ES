---
unique-page-id: 14352509
description: Glosario de campos dinámicos - Documentos de Marketo - Documentación del producto
title: Glosario de campos dinámicos
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Glosario de campos dinámicos {#dynamic-fields-glossary}

Al crear una plantilla en Sales Connect, siempre se recomienda integrar campos dinámicos, utilizando la variable **Campos dinámicos de MSE** botón.

Esta herramienta se utiliza para `auto-personalize your email` y ahorre toneladas de tiempo `pulling information from the People page`.

| Campo dinámico | Ejemplo de lo que aparece en el correo electrónico |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Si no quieres saber de mí otra vez, por favor háganme saber aquí |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor técnico superior |
| `{{work_website}}` | https://www.marketo.com |

**Cosas que hay que tener en cuenta**:

* Si la información de un contacto se introduce incorrectamente o no aparece en la página Personas, no se introduce correctamente en la plantilla.
* La diferencia entre `{{company}}` y `{{company_friendly}}` es que `{{company_friendly}}` quitará cualquier título formal, como Inc., LLC., etc., del nombre de la empresa de su contacto.
* Al usar `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los detalles de contacto. Así es como Sales Connect sabe lo que debe eliminar al extraer el valor.

>[!TIP]
>
>Puede crear su propio [campo dinámico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para cualquier cosa que desee que haya introducido automáticamente en sus correos electrónicos
