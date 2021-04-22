---
unique-page-id: 7512524
description: Prácticas recomendadas para listas inteligentes - Documentos de Marketo - Documentación del producto
title: Prácticas recomendadas para listas inteligentes
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Prácticas recomendadas para listas inteligentes {#best-practices-for-smart-lists}

Las listas inteligentes son la herramienta de consulta más potente del entorno de marketing. Encuentran a la gente que buscas con velocidad mágica y facilidad.

Para facilitar el trabajo y la optimización del rendimiento, hemos creado una lista de prácticas recomendadas. ¡Disfrútelo!

>[!NOTE]
>
>**Cada cliente es diferente.** Cuanto mayor sea la base de datos, más procesamiento se producirá. Cuantas más actividades haya almacenado, más tardará en buscarlas.
>
>Si está experimentando lentitud, pruebe los consejos siguientes. Si el problema persiste, póngase en contacto con el [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. **Limitar historial: los filtros de** historial (también conocidos como filtros de actividad) están entre las operaciones con mayor consumo de recursos y con más tiempo. Si debe utilizarlos, intente limitar el intervalo de fechas a lo más corto posible, lo que reduciría el conjunto de datos que se pueden buscar.
1. **Limitar listas inteligentes anidadas:** al crear una nueva lista inteligente, limite la cantidad de filtros de &quot;Miembro de la lista inteligente&quot; utilizados. Esto se denomina anidación de listas inteligentes, y cada lista inteligente a la que se hace referencia aumentará el tiempo de procesamiento. En su lugar, haga referencia a listas estáticas o utilice [segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Utilice operadores positivos sobre negativos:** aunque los filtros &quot;no&quot; están disponibles, deben buscar en todo el conjunto de datos de su instancia, lo que puede consumir mucho tiempo. Los filtros &quot;is&quot; positivos son capaces de aprovechar algoritmos de búsqueda más efectivos.
1. **Evitar &quot;contiene&quot;:** si solo tiene datos parciales, los calificadores &quot;comienza con&quot; arrojarán resultados mucho más rápidos que &quot;contiene&quot;. &quot;Is&quot; se ejecutará aún más rápido. Evite utilizar &quot;contiene&quot; con varios valores; ambos juntos pueden ralentizar aún más una campaña.
1. **Usar muestra aleatoria por sí solo:** el ejemplo aleatorio es un filtro especial. Úselo por sí solo para colocar a sus personas en listas prediseñadas. A continuación, utilice &quot;Member of List&quot; para hacer que su lista inteligente sea muy rápida. El ejemplo aleatorio **NOT** funcionará con listas inteligentes anidadas. El filtro de ejemplo aleatorio no funcionará si se hace referencia a la lista inteligente para el filtro &quot;Miembro de la lista inteligente&quot;.
1. **Sea versátil con los filtros de inactividad:** los filtros como &quot;Formulario no rellenado&quot; pueden ser muy útiles, pero requieren mucho más poder de procesamiento.
1. **Tenga cuidado al pegar en varios valores:** la selección múltiple está diseñada para pegar en docenas o posiblemente cientos de valores. Sin embargo, pongamos demasiadas cosas y se va a ralentizar.
1. **Tenga cuidado al agregar restricciones:** estos son los pequeños detalles de una regla y los valores relacionados. Cuantas más restricciones agregue, más lento será el tiempo de procesamiento.
1. **Simplifique sus campañas: más de** 100 reglas independientes (¡lo hemos visto!) obviamente van a tomar algún tiempo en procesarse. Manténgalo sencillo y notará las mejoras de velocidad - además será más fácil de entender.
1. **Incluya el símbolo @ antes del nombre de dominio al utilizar el filtro** **Dirección de correo electrónico** : esto hace que utilice una consulta más rápida. Ejemplo: En lugar de utilizar _el correo electrónico contiene &#39;somedomain.com&#39;_, utilice _el correo electrónico contiene &#39;@somedomain.com_&#39;. Si utiliza varias direcciones de correo electrónico con &quot;contiene&quot;, TODAS deben comenzar con &quot;@&quot;.

>[!TIP]
>
>Marketo se puede usar de muchas maneras y ciertas técnicas son mejores para usted y su empresa. Considere los [servicios profesionales de Marketo](https://pages2.marketo.com/72-hour-survival-guide.html) para que su inversión brille.
