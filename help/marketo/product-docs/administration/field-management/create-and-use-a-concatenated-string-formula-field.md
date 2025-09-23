---
unique-page-id: 2360337
description: 'Creación y uso de un campo de cadena concatenada (fórmula): documentos de Marketo, documentación del producto'
title: Crear y utilizar un campo de cadena concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 9%

---

# Crear y utilizar un campo de cadena concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Puede combinar valores de varios campos o crear un valor condicional mediante un campo de fórmula de Marketo Engage.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Haga clic en **[!UICONTROL Administración de campos]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Haga clic en **[!UICONTROL Nuevo campo personalizado]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Seleccione **[!UICONTROL Fórmula]** para **[!UICONTROL Tipo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Escriba un **[!UICONTROL Nombre]** para el campo y haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Busque y seleccione el campo de fórmula y haga clic en **[!UICONTROL Editar reglas]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Añada dos opciones y configúrelas como en la captura de pantalla siguiente.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Obtenga más información acerca de [tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ahora puede agregar el campo de fórmula como un token en un correo electrónico.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Los campos de fórmula se pueden utilizar en páginas de destino, correos electrónicos y columnas de listas inteligentes. Los correos electrónicos con campos de fórmula _no_ se pueden enviar usando una campaña por lotes. Use un [token de script de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) en este escenario.

¡Buen trabajo! Ahora tiene un campo inteligente que sabe qué saludos incluir en función del género. Diviértete con esto y ponte creativo.
