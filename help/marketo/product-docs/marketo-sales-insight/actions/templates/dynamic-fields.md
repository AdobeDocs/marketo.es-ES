---
description: 'Campos dinámicos: documentos de Marketo: documentación del producto'
title: Campos dinámicos
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: 466df1fbd561860152f9fea02edb6eab5670c90a
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Campos dinámicos {#dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y autocompletar estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>El campo &quot;first_name&quot; y &quot;company&quot; son los únicos campos que buscarán tanto Sales Insight Actions como Salesforce. Esto significa que si un contacto no existe en el [aplicación web](https://toutapp.com/login), buscamos en Salesforce para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico coincidente. A continuación, se utiliza la información de ese registro para rellenar el campo.

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. Entrada **Plantillas y campañas**, busque la plantilla que desee editar y haga clic en **Editar plantilla**.

1. Clic **Insertar campo dinámico**.

   >[!NOTE]
   >
   >Al enviar por correo electrónico a los contactos que existen en las acciones de información de ventas, puede utilizar los campos dinámicos básicos. Estos extraerán directamente del contacto.

Si va a enviar por correo electrónico a contactos que existen en Salesforce, puede aprovechar los campos dinámicos de Salesforce. Todas comienzan con &quot;sfdc&quot;. Siempre que tenga una conexión con Salesforce, estos campos llamarán directamente al posible cliente o contacto de Salesforce para rellenar la información en la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente, cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de garantizar que tenga el formato adecuado.

## Valores predeterminados de campo dinámico {#dynamic-field-default-values}

Al añadir campos dinámicos a las plantillas de correo electrónico, puede añadir un valor predeterminado que el campo dinámico resolverá si no hay otro valor disponible.

Para ello, añada &quot;|&quot; después de la etiqueta de campo dinámico y, a continuación, añada &quot;default:&quot;. A continuación, agregue el valor al que desee que se resuelva el campo si no se encuentra ningún otro valor.

**Ejemplo:**

`{{first name | default: loyal customer}}`

`{{sfdc_contact_account_name | default: your company}}`

## Glosario de campos dinámicos {#dynamic-fields-glossary}

Al crear una plantilla en las acciones de información de ventas, siempre se recomienda integrar los campos dinámicos utilizando **Insertar campo dinámico** botón.

Esta herramienta se utiliza para `auto-personalize your email` y ahorrarte toneladas de tiempo por `pulling information from the People page`.

| Campo dinámico | Ejemplo de lo que aparece en el correo electrónico |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Si no quieres volver a saber de mí, por favor házmelo saber aquí |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor técnico sénior |
| `{{work_website}}` | https://www.marketo.com |

**Cosas que debe tener en cuenta**:

* Si la información de un contacto se introduce incorrectamente o no aparece en la página Personas, no se abrirá correctamente en la plantilla.
* La diferencia entre `{{company}}` y `{{company_friendly}}` es eso `{{company_friendly}}` eliminará cualquier título formal, como Inc., LLC., etc., del nombre de la compañía de su contacto.
* Al utilizar `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los datos de contacto. Así es como las acciones de perspectiva de ventas saben qué eliminar al extraer el valor.
* Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{my_name}}` o `{{my_title}}`. Estos campos le permiten hacer referencia rápidamente a sí mismo en sus plantillas de correo electrónico.

>[!TIP]
>
>Si los campos dinámicos no se rellenan, consulte [este artículo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
