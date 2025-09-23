---
description: 'Campos dinámicos: documentos de Marketo: documentación del producto'
title: Campos dinámicos
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 2%

---

# Campos dinámicos {#dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y autocompletar estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>El campo &quot;first_name&quot; y &quot;company&quot; son los únicos campos que se verán tanto en [!DNL Sales Insight Actions] como en [!DNL Salesforce]. Eso significa que si un contacto no existe en la [aplicación web](https://toutapp.com/login), buscamos en [!DNL Salesforce] para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico que coincida. A continuación, se utiliza la información de ese registro para rellenar el campo.

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. En **[!UICONTROL Plantillas y campañas]**, busque la plantilla que desee editar y haga clic en **[!UICONTROL Editar plantilla]**.

1. Haga clic en **[!UICONTROL Insertar campo dinámico]**.

   >[!NOTE]
   >
   >Al enviar por correo electrónico contactos que existen en [!DNL Sales Insight Actions], puede utilizar los campos dinámicos básicos. Estos extraerán directamente del contacto.

Si va a enviar por correo electrónico contactos que existen en [!DNL Salesforce], puede aprovechar los campos dinámicos de [!DNL Salesforce]. Todas comienzan con &quot;sfdc&quot;. Siempre que tenga una conexión con [!DNL Salesforce], estos campos llamarán directamente al posible cliente/contacto de [!DNL Salesforce] para rellenar la información en la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente, cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de garantizar que tenga el formato adecuado.

## Valores predeterminados de campo dinámico {#dynamic-field-default-values}

Al añadir campos dinámicos a las plantillas de correo electrónico, puede añadir un valor predeterminado que el campo dinámico resolverá si no hay otro valor disponible.

Para ello, añada &quot;|&quot; después de la etiqueta del campo dinámico y, a continuación, añada &quot;default:&quot; (ambos sin comillas). A continuación, agregue el valor al que desea que se resuelva el campo (entre comillas) si no se encuentra ningún otro valor.

**Ejemplo:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glosario de campos dinámicos {#dynamic-fields-glossary}

Al crear una plantilla en [!DNL Sales Insight Actions], siempre se recomienda integrar campos dinámicos con el botón **[!UICONTROL Insertar campo dinámico]**.

Esta herramienta se ha usado para `auto-personalize your email` y le ahorrará mucho tiempo a `pulling information from the People page`.

| Campo dinámico | Ejemplo de lo que aparece en el correo electrónico |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Si ya no desea recibir correos electrónicos de nuestra parte, haga clic aquí |
| `{{friendly_unsubscribe}}` | ¿Cansado de todos los correos electrónicos? Por favor, hágamelo saber aquí |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, redactor técnico sénior - Adobe |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | Escritor técnico sénior |
| `{{work_website}}` | <https://www.adobe.com> |

**Aspectos a tener en cuenta**:

* Si la información de un contacto se introduce incorrectamente o no aparece en la página Personas, no se abrirá correctamente en la plantilla.
* La diferencia entre `{{company}}` y `{{company_friendly}}` es que `{{company_friendly}}` eliminará cualquier título formal, como Inc., LLC., etc., del nombre de la compañía del contacto.
* Cuando use `{{company_friendly}}`, asegúrese de separar Inc. o Co. con una coma en los detalles de contacto. Así es como [!DNL Sales Insight Actions] sabe qué quitar al extraer el valor.
* Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{my_name}}` o `{{my_title}}`. Estos campos le permiten hacer referencia rápidamente a sí mismo en sus plantillas de correo electrónico.
* El sistema anexa automáticamente la firma del usuario a cada correo electrónico enviado. Si el usuario está usando una plantilla con el campo dinámico `{{my_signature}}`, el sistema rellenará la firma donde se ha colocado el campo dinámico `{{my_signature}}`. Solo se añade allí para evitar duplicaciones. El sistema administrará `{{team_unsubscribe}}` del mismo modo cuando la configuración global de cancelación de suscripción de datos anexados esté habilitada.

>[!TIP]
>
>Si los campos dinámicos no se rellenan, consulte [este artículo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
