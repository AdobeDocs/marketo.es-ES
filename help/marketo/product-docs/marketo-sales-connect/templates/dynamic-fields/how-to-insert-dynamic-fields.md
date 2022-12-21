---
unique-page-id: 14352592
description: Inserción de campos dinámicos - Documentos de Marketo - Documentación del producto
title: Inserción de campos dinámicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Inserción de campos dinámicos {#how-to-insert-dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y completar automáticamente estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>El campo &quot;first_name&quot; y &quot;company&quot; son los únicos campos que se utilizarán en Conexión de ventas y en Salesforce. Esto significa que si un contacto no existe en la variable [aplicación web](https://toutapp.com/login), buscamos en Salesforce para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico coincidente. A continuación, utilizamos la información de ese registro para rellenar el campo .

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. En **Plantillas y campañas**, busque la plantilla que desea editar y haga clic en **Editar plantilla**.

1. Haga clic en **Tejer campos dinámicos**.

   >[!NOTE]
   >
   >Al enviar por correo electrónico a los contactos que existen en Conexión de ventas, puede utilizar los campos dinámicos básicos. Se extraerán directamente del contacto.

Si está enviando por correo electrónico contactos que existen en Salesforce, puede aprovechar los campos dinámicos de Salesforce. Todos ellos comienzan con &quot;sfdc&quot;. Siempre y cuando tenga una conexión con Salesforce, estos campos llamarán directamente al posible cliente o contacto de Salesforce para rellenar la información en la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente, cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de asegurarse de que tiene el formato adecuado.
