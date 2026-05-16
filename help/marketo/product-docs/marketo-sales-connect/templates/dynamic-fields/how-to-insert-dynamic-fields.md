---
unique-page-id: 14352592
description: Aprenda a insertar campos dinámicos en plantillas de Sales Connect. Agregue el nombre, la empresa y otros campos de combinación en el editor de plantillas.
title: Cómo insertar campos dinámicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/WwKaorfXBu5Ah9wD6pXf5U4YzlpP9MoUMg-TtDzXDRo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 4%

---

# Cómo insertar campos dinámicos {#how-to-insert-dynamic-fields}

Le permitimos personalizar sus plantillas de correo electrónico con atributos predefinidos como `{{first_name}}` o `{{company}}`. Estos campos le permiten enviar por correo electrónico varios contactos y autocompletar estos campos sin tener que escribirlos por separado para cada contacto.

>[!TIP]
>
>El campo &quot;first_name&quot; y &quot;company&quot; son los únicos campos que se verán tanto en [!DNL Sales Connect] como en [!DNL Salesforce]. Eso significa que si un contacto no existe en la [aplicación web](https://toutapp.com/login), buscamos en [!DNL Salesforce] para ver si podemos encontrar un registro de contacto/posible cliente con una dirección de correo electrónico que coincida. A continuación, se utiliza la información de ese registro para rellenar el campo.

## Insertar un campo dinámico en una plantilla {#insert-a-dynamic-field-into-a-template}

1. En **[!UICONTROL Plantillas y campañas]**, busque la plantilla que desee editar y haga clic en **[!UICONTROL Editar plantilla]**.

1. Haga clic en **[!UICONTROL Campos dinámicos de salida]**.

   >[!NOTE]
   >
   >Al enviar por correo electrónico contactos que existen en [!DNL Sales Connect], puede utilizar los campos dinámicos básicos. Estos extraerán directamente del contacto.

Si está enviando por correo electrónico a contactos que existen en [!DNL Salesforce], puede aprovechar los campos dinámicos de [!DNL Salesforce]. Todas comienzan con &quot;sfdc&quot;. Siempre que tenga una conexión con [!DNL Salesforce], estos campos llamarán directamente al posible cliente/contacto de [!DNL Salesforce] para rellenar la información en la plantilla.

## Insertar campos dinámicos en una línea de asunto {#insert-dynamic-fields-in-a-subject-line}

Simplemente, cópielos y péguelos manualmente en el campo de asunto de un correo electrónico, teniendo cuidado de garantizar que tenga el formato adecuado.
