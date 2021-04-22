---
unique-page-id: 2360337
description: 'Crear y utilizar un campo de cadena concatenada (fórmula): Marketo Docs: documentación del producto'
title: Crear y utilizar un campo de cadena concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Crear y usar un campo de cadena concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Puede combinar valores de varios campos o crear un valor condicional mediante un campo de fórmula de Marketo.

1. Vaya a **Admin** y haga clic en **Administración de campos**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Haga clic en **Nuevo campo personalizado**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Seleccione **Formula** para **Type**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Introduzca un **Name** para el campo y haga clic en **Create**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Busque y seleccione el campo de fórmula y haga clic en **Editar reglas**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Añada dos opciones y defina como la captura de pantalla siguiente.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Obtenga más información sobre [tokens para los pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ahora puede añadir el campo de fórmula como token en un correo electrónico.

   ![](assets/seven.png)

>[!NOTE]
>
>Los campos de fórmula se pueden utilizar en páginas de aterrizaje, correos electrónicos y columnas de lista inteligente (no se exportan). Los correos electrónicos con campos de fórmula **not** se pueden enviar mediante una campaña por lotes. Utilice un [token de script de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) en esta situación.

¡Buen trabajo! Ahora tiene un campo inteligente que sabe qué saludo incluir en función del género. Diviértete con esto y sé creativo.
