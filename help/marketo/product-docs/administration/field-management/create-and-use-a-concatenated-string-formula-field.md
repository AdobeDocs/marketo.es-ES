---
unique-page-id: 2360337
description: Crear y utilizar un campo de cadena concatenada (fórmula) - Marketo Docs - Documentación del producto
title: Crear y utilizar un campo de cadena concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Crear y utilizar un campo de cadena concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Puede combinar valores de varios campos o crear un valor condicional mediante un campo de fórmula de Marketo.

1. Vaya a **Administrador** y haga clic en **Gestión de las actividades sobre el terreno**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Haga clic en **Nuevo campo personalizado**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Select **Fórmula** para el **Tipo**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Escriba un **Nombre** para el campo , haga clic en **Crear**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Busque y seleccione el campo de fórmula y haga clic en **Editar reglas**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Añada dos opciones y defina como la captura de pantalla siguiente.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Más información sobre [tokens para pasos de flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ahora puede añadir el campo de fórmula como token en un correo electrónico.

   ![](assets/seven.png)

>[!NOTE]
>
>Los campos de fórmula se pueden utilizar en páginas de aterrizaje, correos electrónicos y columnas de lista inteligente (no se exportan). Los correos electrónicos con campos de fórmula pueden **not** se envían mediante una campaña por lotes. Utilice un [token de script de correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) en este escenario.

¡Buen trabajo! Ahora tiene un campo inteligente que sabe qué saludo incluir en función del género. Diviértete con esto y sé creativo.
