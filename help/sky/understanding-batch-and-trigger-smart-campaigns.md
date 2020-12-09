---
title: Understanding-batch-and-desencadenador-campañas inteligentes
description: Explicación de las Campañas inteligentes por lotes y activadoras
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Explicación de las Campañas inteligentes por lotes y activadoras

<br> 

Existen dos tipos de campañas inteligentes: Lote y activador.

## Campaña inteligente por lotes

Una campaña por lotes se inicia a una hora específica y afecta a un conjunto específico de personas a la vez. Un ejemplo sería enviar un correo electrónico a todos los usuarios de la base de datos que residan en California.

Las campañas inteligentes por lotes solo tendrán filtros dentro de la sección de listas inteligentes (es decir, sin activadores).

![Imagen uno](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Al hacer clic en la ficha **[!UICONTROL Programar]** se confirmará que la campaña inteligente se ha definido como &quot;Lote&quot;.

![Imagen dos](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campañas inteligentes por lotes**

* Se puede programar para recurrencias como, por ejemplo, diarias, semanales y mensuales. También se pueden ejecutar una sola vez.
* Están visibles en la vista [del](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)calandario del programa.
* No se incluirá en la vista nada después de un paso &quot;Esperar&quot; dentro de la campaña inteligente.

## Activar Campaña inteligente

Una campaña inteligente de desencadenador afecta a una persona a la vez en función de un evento activado. Un ejemplo de activador sería hacer clic en un vínculo de un correo electrónico.

Si una campaña inteligente utiliza al menos un activador dentro de la sección de lista inteligente, el modo se establecerá automáticamente en activado.

![Imagen tres](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Al hacer clic en la ficha **[!UICONTROL Programar]** , se confirmará que la campaña inteligente está configurada en &quot;Activar&quot;.

![Imagen Cuatro](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Activar Campañas inteligentes**

* No se puede programar para recurrencias. Solo se pueden configurar como activas o inactivas.
* Puede configurar más de un activador. Sin embargo, si se activa _cualquier_ activador, se ejecutarán las acciones de campaña.

>[!TIP]
>
>Utilice el registro [de](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) actividades para ver qué ha ocurrido paso a paso dentro de sus campañas inteligentes. Puede encontrar el registro de actividades en la última ficha de la página de detalles de una persona.
