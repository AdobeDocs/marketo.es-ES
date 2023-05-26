---
unique-page-id: 2360337
description: 'Creación y uso de un campo de cadena concatenada (fórmula): documentos de Marketo, documentación del producto'
title: Crear y utilizar un campo de cadena concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Crear y utilizar un campo de cadena concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Puede combinar valores de varios campos o crear un valor condicional mediante un campo de Fórmula de Marketo.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Clic **[!UICONTROL Administración de campos]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Clic **[!UICONTROL Nuevo campo personalizado]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Seleccionar **[!UICONTROL Fórmula]** para el **[!UICONTROL Tipo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Introduzca una **[!UICONTROL Nombre]** para el campo, haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Busque y seleccione el campo de fórmula y haga clic en **[!UICONTROL Editar reglas]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Añada dos opciones y configúrelas como en la captura de pantalla siguiente.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Más información sobre [tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ahora puede agregar el campo de fórmula como un token en un correo electrónico.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Los campos de fórmula se pueden utilizar en páginas de aterrizaje, correos electrónicos y columnas de listas inteligentes (no se exportan). Los correos electrónicos con campos de fórmula pueden _no_ se enviarán mediante una campaña por lotes. Utilice una [token de script de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) en este escenario.

¡Buen trabajo! Ahora tiene un campo inteligente que sabe qué saludos incluir en función del género. Diviértete con esto y ponte creativo.
