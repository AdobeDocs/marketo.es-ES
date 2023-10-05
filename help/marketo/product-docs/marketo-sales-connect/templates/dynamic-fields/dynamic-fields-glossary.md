---
unique-page-id: 14352509
description: 'Glosario de campos dinámicos: documentos de Marketo, documentación del producto'
title: Glosario de campos dinámicos
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 1%

---

# Glosario de campos dinámicos {#dynamic-fields-glossary}

Al crear una plantilla en Sales Connect, siempre se recomienda integrar los campos dinámicos mediante el **Campos dinámicos MSE** botón.

Esta herramienta se utiliza para `auto-personalize your email` y ahorrarte toneladas de tiempo por `pulling information from the People page`.

| Campo dinámico | Ejemplo de lo que aparece en el correo electrónico |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Si ya no desea recibir correos electrónicos de nuestra parte, haga clic aquí |
| `{{friendly_unsubscribe}}` | ¿Cansado de todos los correos electrónicos? Por favor, hágamelo saber aquí |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, escritor técnico sénior - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor técnico sénior |
| `{{work_website}}` | https://www.adobe.com |

**Cosas que debe tener en cuenta**:

* Si la información de un contacto se introduce incorrectamente o no aparece en la página Personas, no se abrirá correctamente en la plantilla.
* La diferencia entre `{{company}}` y `{{company_friendly}}` es eso `{{company_friendly}}` eliminará cualquier título formal, como Inc., LLC., etc., del nombre de la compañía de su contacto.
* Al utilizar `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los datos de contacto. Así es como Sales Connect sabe lo que debe eliminar al extraer el valor.
* Si usa el `{{my_signature}}` , el sistema no adjuntará automáticamente la firma del usuario para evitar duplicados.

>[!TIP]
>
>Puede crear su propio [campo dinámico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para cualquier cosa que desee haber incluido automáticamente en sus correos electrónicos
