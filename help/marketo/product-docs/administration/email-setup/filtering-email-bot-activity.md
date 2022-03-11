---
description: Filtrado de la actividad de bots de correo electrónico - Documentos de Marketo - Documentación del producto
title: Filtrado de la actividad de bots de correo electrónico
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Filtrado de la actividad de bots de correo electrónico {#filtering-email-bot-activity}

A veces, la actividad de bots de correo electrónico puede inflar erróneamente los datos de aperturas y clics del correo electrónico. Así es como arreglarlo.

>[!NOTE]
>
>Al usar la variable [Lista internacional de arañas web y bots de la IAB/ABC](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), toda la actividad de apertura o clic con una IP o un agente de usuario que coincida con cualquier cosa de esa lista se identificará como actividad de bots y no se registrará en Marketo.

1. Haga clic en **Administrador**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Haga clic en el **Actividad de bots** pestaña .

   ![](assets/filtering-email-bot-activity-3.png)

1. Haga clic en el control deslizante para activar **Filtrar actividad de bots**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Puede elegir por separado si desea que se registre o no la actividad de bots. Si decide no hacerlo, es posible que vea una caída en las aperturas de correo electrónico y los clics mientras se filtran los números falsos.

**PASO OPCIONAL**: Para desactivar la función, simplemente anule la selección del control deslizante. Si desactiva, los datos de &quot;Actividad de bots en los últimos 90 días&quot; sí lo hacen **not** restablecer.

>[!TIP]
>
>Aproveche los datos de actividad de bots en las listas inteligentes mediante el booleano &quot;Es actividad de bots&quot; (sí/no) o en las restricciones aplicables de filtro/déclencheur.
