---
description: Bloqueo de envíos de formularios de correo no deseado - Documentos de Marketo - Documentación del producto
title: Bloqueo de envíos de formularios no deseados
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Bloqueo de envíos de formularios no deseados {#how-to-block-spam-form-submissions}

A menudo, los envíos de formularios con una suma de comprobación no válida o que falta (generalmente de bots) pueden producir estadísticas falsas. Así es como prevenir eso.

>[!CAUTION]
>
>Esta función rechaza los envíos de formularios realizados mediante POST programáticos al extremo leadCapture/save2 . Si su empresa utiliza una integración que envíe formularios a Marketo con ese método, habilitar esta función bloqueará esos envíos. No se admite ni tampoco está permitido usar leadCapture/save2 como API o realizar envíos programáticos de formularios directamente a él. Asegúrese de que su empresa solo envía formularios mediante: Recursos de formulario, código de formularios incrustados, API de Forms2.js o API de envío de REST de formulario.

1. Haga clic en **Admin**.

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. Haga clic en **Treasure Chest**.

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. Junto a **Captura de persona - Rechazar valores de suma de comprobación no válidos**, haga clic en **Editar**.

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. Seleccione la casilla **Enabled** y haga clic en **Save**.

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>Al habilitar esta función, es posible que vea una caída en la actividad del formulario a medida que se filtran los números falsos.
