---
unique-page-id: 14352592
description: 'Inserción de campos dinámicos: documentos de Marketo, documentación del producto'
title: Cómo insertar campos dinámicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Cómo insertar campos dinámicos {#how-to-insert-dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y autocompletar estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>El campo &quot;first_name&quot; y &quot;company&quot; son los únicos campos que se buscarán en Sales Connect y Salesforce. Esto significa que si un contacto no existe en el [aplicación web](https://toutapp.com/login), buscamos en Salesforce para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico coincidente. A continuación, se utiliza la información de ese registro para rellenar el campo.

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. Entrada **Plantillas y campañas**, busque la plantilla que desee editar y haga clic en **Editar plantilla**.

1. Clic **Extraer campos dinámicos**.

   >[!NOTE]
   >
   >Al enviar por correo electrónico a los contactos que existen en Sales Connect, puede utilizar los campos dinámicos básicos. Estos extraerán directamente del contacto.

Si va a enviar por correo electrónico a contactos que existen en Salesforce, puede aprovechar los campos dinámicos de Salesforce. Todas comienzan con &quot;sfdc&quot;. Siempre que tenga una conexión con Salesforce, estos campos llamarán directamente al posible cliente o contacto de Salesforce para rellenar la información en la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente, cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de garantizar que tenga el formato adecuado.
