---
unique-page-id: 2953132
description: Explicación de las Campañas inteligentes por lotes y Déclencheur - Documentos de marketing - Documentación del producto
title: Explicación de las Campañas inteligentes por lotes y Déclencheur
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Explicación de las Campañas inteligentes por lotes y Déclencheur {#understanding-batch-and-trigger-smart-campaigns}

Existen dos tipos de campañas inteligentes: Lote y Déclencheur.

## Campaña inteligente por lotes {#batch-smart-campaign}

>[!NOTE]
>
>**Definición**
>
>Una campaña por lotes se inicia a una hora específica y afecta a un conjunto específico de personas a la vez. Un ejemplo sería enviar un correo electrónico a todas las personas de California.

Las campañas inteligentes por lotes solo tendrán filtros dentro de la sección de listas inteligentes (es decir, sin déclencheur).

![](assets/batch-filter.png)

Al hacer clic en la ficha **Programar** se confirmará que la campaña inteligente se ha definido como &quot;Lote&quot;.

![](assets/batch-c4.png)

**Campañas inteligentes por lotes**

* Se puede programar para recurrencias como, por ejemplo, diarias, semanales y mensuales. También se pueden ejecutar una sola vez.
* Están visibles en la vista [calandario del programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). No se incluirá en la vista nada después de un paso &quot;Esperar&quot; dentro de la campaña inteligente.

<br> 

## Campaña inteligente de déclencheur {#trigger-smart-campaign}

>[!NOTE]
>
>**Definición**
>
>Una campaña inteligente de déclencheur afecta a una persona a la vez en función de un evento activado. Un ejemplo de déclencheur sería hacer clic en un vínculo de un correo electrónico.

Si una campaña inteligente utiliza al menos un déclencheur dentro de la sección de lista inteligente, el modo se establecerá automáticamente en activado.

![](assets/trigger.png)

Al hacer clic en la ficha **Programar** se confirmará que la campaña inteligente se ha definido como &quot;Activada&quot;.

![](assets/trigger2.png)

**Campañas inteligentes de déclencheur**

* No se puede programar para recurrencias. Solo se pueden configurar como activas o inactivas.
* Puede configurar más de un déclencheur. Sin embargo, si se activa algún déclencheur, se ejecutarán las acciones de campaña.

>[!TIP]
>
>Utilice el [registro de actividades](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) para ver qué ha ocurrido paso a paso dentro de sus campañas inteligentes. Puede encontrar el registro de actividades en la última ficha de la página de detalles de una persona.
