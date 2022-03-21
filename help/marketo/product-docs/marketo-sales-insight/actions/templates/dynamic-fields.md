---
description: Campos dinámicos - Documentos de Marketo - Documentación del producto
title: Campos dinámicos
hide: true
hidefromtoc: true
source-git-commit: a0b10255513c13b7100b667513e3e61fc3788a15
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Campos dinámicos {#dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y completar automáticamente estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>Los campos &quot;first_name&quot; y &quot;company&quot; son los únicos campos que se utilizarán tanto para las acciones de perspectiva de ventas como para Salesforce. Esto significa que si un contacto no existe en la variable [aplicación web](https://toutapp.com/login), buscamos en Salesforce para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico coincidente. A continuación, utilizamos la información de ese registro para rellenar el campo .

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. En **Plantillas y campañas**, busque la plantilla que desea editar y haga clic en **Editar plantilla**.

1. Haga clic en **Insertar campo dinámico**.

   >[!NOTE]
   >
   >Al enviar por correo electrónico a los contactos que existen en las acciones de perspectiva de ventas, puede utilizar los campos dinámicos básicos. Se extraerán directamente del contacto.

Si está enviando por correo electrónico contactos que existen en Salesforce, puede aprovechar los campos dinámicos de Salesforce. Todos ellos comienzan con &quot;sfdc&quot;. Siempre y cuando tenga una conexión con Salesforce, estos campos llamarán directamente al posible cliente o contacto de Salesforce para rellenar la información en la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente, cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de asegurarse de que tiene el formato adecuado.

## Glosario de campos dinámicos {#dynamic-fields-glossary}

Al crear una plantilla en acciones de perspectiva de ventas, siempre se recomienda integrar campos dinámicos, utilizando la variable **Insertar campo dinámico** botón.

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
* Al usar `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los detalles de contacto. Así es como las acciones de perspectiva de ventas saben qué eliminar al extraer el valor.
* Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{my_name}}` o `{{my_title}}`. Estos campos le permiten hacerse referencia rápidamente a sí mismo en las plantillas de correo electrónico.

>[!TIP]
>
>Si los campos dinámicos no se rellenan, desproteja [este artículo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
