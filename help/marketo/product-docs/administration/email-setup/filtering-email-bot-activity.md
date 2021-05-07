---
description: Filtrado de la actividad de bots de correo electrónico - Documentos de Marketo - Documentación del producto
title: Filtrado de la actividad de bots de correo electrónico
translation-type: tm+mt
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---

# Filtrado de la actividad de bots de correo electrónico {#filtering-email-bot-activity}

A veces, la actividad de bots de correo electrónico puede inflar erróneamente los datos de aperturas y clics del correo electrónico. Así es como arreglarlo.

>[!NOTE]
>
>Esta función se habilitará para todas las instancias de Marketo la tarde del martes 11 de mayo.

>[!NOTE]
>
>Mediante la [Lista internacional de bots y arañas de la IAB/ABC](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), toda actividad de apertura o de clic con una IP o un agente de usuario que coincida con cualquier elemento de la lista se identificará como actividad de bots y no se iniciará sesión en Marketo.

1. Haga clic en **Admin**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Haga clic en **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Haga clic en la pestaña **Actividad de bots**.

   ![](assets/filtering-email-bot-activity-3.png)

1. Seleccione la casilla **Enable Filtering of Email Bot Activity**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Al habilitar esta función, es posible que vea una caída en las aperturas de correo electrónico y en los clics a medida que se filtran los números falsos.

**PASO** OPCIONAL: Para desactivar la función, simplemente anule la selección de la casilla de verificación. Si deshabilita, los datos &quot;Actividad de bots en los últimos 90 días&quot; **no** se restablecen.
