---
unique-page-id: 14352592
description: Cómo insertar campos dinámicos - Documentos de marketing - Documentación del producto
title: Cómo insertar campos dinámicos
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Cómo insertar campos dinámicos {#how-to-insert-dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y completar automáticamente estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>Los campos &quot;first_name&quot; y &quot;compañía&quot; son los `only fields that will look to both Sales Connect and Salesforce.` que significan que si un contacto no existe en la aplicación [](http://toutapp.com/login)web, buscamos en Salesforce para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico coincidente. Luego usamos la información de ese registro para rellenar el campo.

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. En **Plantillas y Campañas**, busque la plantilla que desee editar y haga clic en **Editar plantilla**.
1. Haga clic en **Extraer campos** dinámicos.

   >[!NOTE]
   >
   >Al enviar por correo electrónico contactos que existen en Sales Connect, puede utilizar los campos dinámicos básicos. Éstos se extraerán directamente del contacto.

Si está enviando por correo electrónico contactos que existen en Salesforce, puede aprovechar los campos dinámicos de Salesforce. Todo comienza con &quot;sfdc&quot;. Siempre que tenga una conexión con Salesforce, estos campos llamarán directamente al contacto/posible cliente de Salesforce para rellenar la información de la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de asegurarse de que tiene el formato adecuado.
