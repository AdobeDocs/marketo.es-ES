---
unique-page-id: 7512524
description: Prácticas recomendadas para Listas inteligentes - Documentos de marketing - Documentación del producto
title: Prácticas recomendadas para Listas inteligentes
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Prácticas recomendadas para Listas inteligentes {#best-practices-for-smart-lists}

Las listas inteligentes son la herramienta de consulta más poderosa del universo de la mercadotecnia. Encuentran a la gente que buscas con velocidad y facilidad mágicas.

Para facilitar el trabajo y la optimización del rendimiento, hemos creado una lista de buenas prácticas. ¡Disfrútelo!

>[!NOTE]
>
>**Cada cliente es diferente.** Cuanto mayor sea la base de datos, mayor será el procesamiento. Cuantas más actividades haya almacenado, más tardará en buscarlas.
>
>Si está experimentando lentitud, pruebe las sugerencias siguientes. Si el problema persiste, póngase en contacto con [Soporte técnico de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. **Limitar historial: filtros** de historia (también conocidos como Filtros de actividad) están entre las operaciones que requieren más recursos y más tiempo. Si debe utilizarlos, intente limitar el intervalo de fechas a la mayor brevedad posible, lo que reduciría el conjunto de datos que se pueden buscar.
1. **Limitar listas inteligentes anidadas:** al crear una nueva lista inteligente, limite la cantidad de filtros &quot;Miembro de Lista inteligente&quot; que se utilicen. Esto se denomina anidar listas inteligentes y cada lista inteligente a la que se hace referencia aumentará el tiempo de procesamiento. En su lugar, haga referencia a listas estáticas o utilice [segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Usar operadores positivos sobre negativos:** aunque los filtros &quot;no&quot; están disponibles, deben buscar todo el conjunto de datos de la instancia, lo que puede llevar mucho tiempo. Los filtros &quot;is&quot; positivos pueden aprovechar algoritmos de búsqueda más eficaces.
1. **Evitar &quot;contiene&quot;:** si solo tiene datos parciales, los calificadores &quot;inicios con&quot; producirán resultados mucho más rápidos que &quot;contiene&quot;. &quot;Is&quot; se ejecutará aún más rápido. Evite utilizar &quot;contiene&quot; con varios valores; los dos juntos pueden ralentizar aún más una campaña.
1. **Usar la muestra aleatoria por sí misma: la muestra** aleatoria es un filtro especial. Úselo por sí mismo para poner a su gente en listas prefabricadas. Entonces, sólo usa &quot;Miembro de Lista&quot; para hacer su lista inteligente súper rápido. La muestra aleatoria **NO** funcionará con Listas inteligentes anidadas. El filtro Ejemplo aleatorio no funcionará si se hace referencia a la Lista inteligente para el filtro &quot;Miembro de Lista inteligente&quot;.
1. **Sea próspero con filtros de inactividad -** Filtros como &quot;No rellenado el formulario&quot; pueden ser realmente útiles, pero requieren mucho más poder de procesamiento.
1. **Sea muy útil al pegar en varios valores: la selección** múltiple está diseñada para pegarse en docenas o posiblemente cientos de valores. Sin embargo, pongamos demasiados y se reducirá.
1. **Sea más ahorrador al agregar restricciones:** Estos son los pequeños detalles de una regla y los valores relacionados. Cuantas más restricciones agregue, más lento será el tiempo de procesamiento.
1. **Simplifique sus campañas: más de** 100 reglas independientes (¡lo hemos visto!) obviamente van a tomar algún tiempo en procesarse. Manténgalo sencillo y notará los aumentos de velocidad - además será más fácil de entender.
1. **Incluya el símbolo @ antes del nombre de dominio cuando utilice el filtro** **Dirección de correo electrónico (** esto hace que utilice una consulta más rápida). Ejemplo: En lugar de usar _el correo electrónico contiene &#39;somedomain.com&#39;_, utilice _el correo electrónico contiene &#39;@somedomain.com_&#39;. Si está utilizando varias direcciones de correo electrónico con &quot;contains&quot; (contiene), TODAS deben estar en inicio con &quot;@&quot;.

>[!TIP]
>
>El marketing se puede usar de muchas maneras y ciertas técnicas son mejores para usted y su negocio. Considere [Servicios profesionales de marketing](https://pages2.marketo.com/72-hour-survival-guide.html) para hacer que su inversión brille.
