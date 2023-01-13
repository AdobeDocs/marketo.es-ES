---
unique-page-id: 2360337
description: Crear y utilizar un campo de cadena concatenada (fórmula) - Marketo Docs - Documentación del producto
title: Crear y utilizar un campo de cadena concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: b13360b009aea869bbd96a9cd0888bb121afdcd2
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Crear y utilizar un campo de cadena concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Puede combinar valores de varios campos o crear un valor condicional mediante un campo de fórmula de Marketo.

1. Vaya a la **Administrador** .

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Haga clic en **Gestión de las actividades sobre el terreno**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Haga clic en **Nuevo campo personalizado**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Select **Fórmula** para el **Tipo**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Escriba un **Nombre** para el campo , haga clic en **Crear**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Busque y seleccione el campo de fórmula y haga clic en **Editar reglas**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Añada dos opciones y defina como la captura de pantalla siguiente.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Más información sobre [tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ahora puede añadir el campo de fórmula como token en un correo electrónico.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Los campos de fórmula se pueden utilizar en páginas de aterrizaje, correos electrónicos y columnas de lista inteligente (no se exportan). Los correos electrónicos con campos de fórmula pueden **not** se envían mediante una campaña por lotes. Utilice un [token de script de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) en este escenario.

¡Buen trabajo! Ahora tiene un campo inteligente que sabe qué saludo incluir en función del género. Diviértete con esto y sé creativo.
