---
unique-page-id: 7512524
description: Prácticas recomendadas para Listas inteligentes - Documentos de marketing - Documentación del producto
title: Prácticas recomendadas para Listas inteligentes
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---


# Prácticas recomendadas para Listas inteligentes {#best-practices-for-smart-lists}

Las listas inteligentes son la herramienta de consulta más poderosa del universo de la mercadotecnia. Encuentran a la gente que buscas con velocidad y facilidad mágicas.

Para facilitar el trabajo y la optimización del rendimiento, hemos creado una lista de buenas prácticas. ¡Disfrútelo!

>[!NOTE]
>
>**Cada cliente es diferente.** Cuanto mayor sea la base de datos, mayor será el procesamiento. Cuantas más actividades haya almacenado, más tardará en buscarlas.
>
>Si está experimentando lentitud, pruebe las sugerencias siguientes. Si el problema persiste, póngase en contacto con la [asistencia](http://support.marketo.com)de marketing.

1. **Limitar historia - **filtros históricos (también conocidos como Filtros de actividad) están entre las operaciones que requieren más recursos y más tiempo. Si debe utilizarlos, intente limitar el intervalo de fechas a la mayor brevedad posible, lo que reduciría el conjunto de datos que se pueden buscar.
1. **Limitar las listas inteligentes anidadas - **Al crear una nueva lista inteligente, limite la cantidad de filtros de &quot;Miembro de Lista inteligente&quot; utilizados. Esto se denomina anidar listas inteligentes y cada lista inteligente a la que se hace referencia aumentará el tiempo de procesamiento. En su lugar, haga referencia a listas estáticas o utilice [la segmentación](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Use operadores positivos sobre negativos - **Aunque los filtros &quot;no&quot; están disponibles, tienen que buscar todo el conjunto de datos en su instancia, lo que puede llevar mucho tiempo. Los filtros &quot;is&quot; positivos pueden aprovechar algoritmos de búsqueda más eficaces.
1. **Evite &quot;contiene&quot; -** Si solo tiene datos parciales, los calificadores &quot;inicios con&quot; producirán resultados mucho más rápidos que &quot;contiene&quot;. &quot;Is&quot; se ejecutará aún más rápido. Evite utilizar &quot;contiene&quot; con varios valores; los dos juntos pueden ralentizar aún más una campaña.
1. **Usar la muestra aleatoria por sí misma - **La muestra aleatoria es un filtro especial. Úselo por sí mismo para poner a su gente en listas prefabricadas. Entonces, sólo usa &quot;Miembro de Lista&quot; para hacer su lista inteligente súper rápido. La muestra aleatoria **NO funcionará** con Listas inteligentes anidadas. El filtro Ejemplo aleatorio no funcionará si se hace referencia a la Lista inteligente para el filtro &quot;Miembro de Lista inteligente&quot;.
1. **Sea próspero con filtros de inactividad - **Filtros como &quot;No rellenado el formulario&quot; pueden ser realmente útiles, pero requieren mucho más poder de procesamiento.
1. **Pega mucho con pegar en varios valores - **La selección múltiple está diseñada para pegar en docenas o posiblemente cientos de valores. Sin embargo, pongamos demasiados y se reducirá.
1. **Sea ahorrador al agregar restricciones - **Estos son los pequeños detalles de una regla y los valores relacionados. Cuantas más restricciones agregue, más lento será el tiempo de procesamiento.
1. **Simplifique sus campañas - **100 reglas más independientes (¡lo hemos visto!) obviamente van a tomar algún tiempo en procesarse. Manténgalo sencillo y notará los aumentos de velocidad - además será más fácil de entender.
1. **Incluya el símbolo @ antes del nombre de dominio cuando utilice el filtro** Dirección de correo electrónico **-** Esto hace que utilice una consulta más rápida. Ejemplo: En lugar de usar el *correo electrónico contiene &#39;somedomain.com*&#39;, utilice *email contains &#39;@somedomain.com*&#39;. Si está utilizando varias direcciones de correo electrónico con &quot;contains&quot; (contiene), TODAS deben estar en inicio con &quot;@&quot;.

>[!TIP]
>
>El marketing se puede usar de muchas maneras y ciertas técnicas son mejores para usted y su negocio. Considere [los servicios](http://pages2.marketo.com/72-hour-survival-guide.html) profesionales de Marketing para hacer que su inversión brille.

