---
description: Filtrado de la actividad de bots de correo electrónico - Documentos de Marketo - Documentación del producto
title: Filtrado de la actividad de bots de correo electrónico
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a746fc2350ba2441ecd2157708b88d2480237c49
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Filtrado de la actividad de bots de correo electrónico {#filtering-email-bot-activity}

A veces, la actividad de bots de correo electrónico puede inflar erróneamente los datos de aperturas y clics del correo electrónico. Siga los pasos que se indican a continuación para solucionar el problema.

Utilizamos tres métodos diferentes para confirmar la actividad de bots:

* Coincidir con [Lista de bots de Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;}: Las actividades que coincidan con cualquier elemento de la lista IAB UA/IP (agente de usuario/dirección IP) se marcarán como bots.
* Coincidencia con patrón de proximidad: Cuando se producen más de dos actividades al mismo tiempo (en menos de un segundo), se identifican como bots.

Con respecto a los clics en vínculos de correo electrónico y a la actividad de apertura de correos electrónicos, los nuevos atributos se rellenarán con los valores siguientes:

* Las actividades identificadas como bots tendrán &quot;Actividad de bots&quot; como &quot;Verdadero&quot; y &quot;Patrón de actividad de bots&quot; como patrón/método identificado
* Las actividades identificadas como no bots tendrán &quot;Actividad de bots&quot; como &quot;Falso&quot; y &quot;Patrón de actividad de bots&quot; como &quot;N/D&quot;
* Las actividades que se produjeron antes de que introdujéramos estos atributos tendrán &quot;Actividad de bots&quot; como &quot; (vacío) y &quot;Patrón de actividad de bots&quot; como &quot;&quot; (vacío)

1. Haga clic en **Administrador**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Haga clic en el **Actividad de bots** pestaña .

   ![](assets/filtering-email-bot-activity-3.png)

1. Elija **Coincidir con la lista IAB**, **Coincidencia con patrón de proximidad**, o ambas. Elija si desea registrar la actividad de bots _o_ filtrar la actividad de bots.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Si elige Filtrar la actividad de bots, es posible que vea una caída en las aperturas de correo electrónico y los clics a medida que se eliminan las actividades falsas.

**PASO OPCIONAL**: Para desactivar esta función, simplemente anule la selección del control deslizante. Si deshabilita, los datos no se restablecerán.

>[!TIP]
>
>Aproveche los datos de actividad de bots en las listas inteligentes mediante los déclencheur booleano &quot;Es actividad de bots&quot; (sí/no) y &quot;Patrón de actividad de bots&quot; de &quot;Vínculo en el correo electrónico&quot; y &quot;Abrir correo electrónico&quot;, y &quot;Vínculo de clics en el correo electrónico&quot; y &quot;Abre el correo electrónico&quot;.
