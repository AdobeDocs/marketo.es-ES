---
title: define-a-smart-list-for-a-batch-campaign
description: Definir una lista inteligente para una campaña por lotes
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Definir una lista inteligente para una campaña por lotes

<br> 

Las listas inteligentes son el mecanismo de Marketo para definir &quot;quién&quot; (qué personas) incluir, ya sea un informe, una lista o una campaña inteligente. A continuación se muestra cómo definir una lista inteligente para una campaña por lotes.

1. Elija una campaña inteligente y haga clic en **[!UICONTROL Smart List]**.

   ![Imagen uno](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Escriba para buscar un filtro y luego arrástrelo y suéltelo en el lienzo. Repita el proceso para varios filtros.

   ![Imagen dos](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >Una campaña inteligente con solo filtros se ejecuta en modo Lote. Encuentra personas en la base de datos que califican según los filtros y los ejecuta a través del flujo a la vez.

   >[!IMPORTANT]
   >
   >Puede hacer que una campaña inteligente se ejecute en una persona a la vez según los eventos en directo añadiendo déclencheur, lo que pone la campaña inteligente en modo de Déclencheur.

1. Haga clic en la lista desplegable y seleccione un operador de filtro (p. ej. **[!UICONTROL es]**, **[!UICONTROL no es]**, etc.) para el filtro que ha elegido.

   ![Imagen tres](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >Las líneas rojas indican errores o falta información. Si no se corrige, la campaña no será válida y no se ejecutará.

1. Introduzca el valor del filtro.

   ![Imagen Cuatro](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>De forma predeterminada, las personas que satisfacen TODAS las reglas de listas inteligentes son
>cualificado. Esto se puede modificar para adaptarlo a sus necesidades de campaña. Consulte [Reglas de lista inteligente para lógica compleja](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic) para obtener más información.
>
>Para realizar déclencheur en eventos en directo de una persona a la vez, aprenda a [Definir lista inteligente para campañas inteligentes | Déclencheur](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
