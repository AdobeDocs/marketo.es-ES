---
unique-page-id: 7512524
description: 'Prácticas recomendadas para listas inteligentes: Documentos de Marketo, documentación del producto'
title: Prácticas recomendadas para listas inteligentes
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Prácticas recomendadas para listas inteligentes {#best-practices-for-smart-lists}

Las listas inteligentes son la herramienta de consulta más potente del entorno de marketing. Encuentra a las personas que buscas con una velocidad y facilidad mágicas.

Para que sean fáciles de usar y optimizar el rendimiento, hemos creado una lista de prácticas recomendadas. ¡Disfrútelo!

>[!NOTE]
>
>**Cada usuario de Marketo Engage es diferente.** Cuanto mayor sea la base de datos, más se procesará. Cuantas más actividades haya almacenado, más tardará en buscarlas.
>
>Si está experimentando lentitud, pruebe las sugerencias a continuación. Si el problema continúa, comuníquese con [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Limitar historial -** Los filtros de historial (también conocidos como filtros de actividad) se encuentran entre las operaciones que consumen más tiempo y recursos. Si debe utilizarlos, intente limitar el intervalo de fechas al más corto posible, lo que reduciría el conjunto de datos en el que se pueden buscar. Además, los intervalos de fechas no sustituyen a los períodos de retención. Ejemplo: Si la actividad que está consultando tiene un período de retención de 90 días y elige &quot;últimos 100 días&quot;, solo se devolverán los resultados de los últimos 90 días. Los períodos de retención de actividades [se pueden encontrar aquí](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limitar listas inteligentes anidadas -** Al crear una nueva lista inteligente, limite la cantidad de filtros de &quot;Miembro de lista inteligente&quot; utilizados. Esto se denomina anidar listas inteligentes y cada lista inteligente a la que se haga referencia aumentará el tiempo de procesamiento. En su lugar, haga referencia a listas estáticas o utilice [segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Use operadores positivos sobre negativos -** Aunque los filtros &quot;no&quot; están disponibles, tienen que buscar en todo el conjunto de datos de su instancia, lo que puede consumir mucho tiempo. Los filtros &quot;es&quot; positivos pueden aprovechar algoritmos de búsqueda más eficaces.
1. **Evite el uso de &quot;contiene&quot; -** Si solo dispone de datos parciales, los calificadores &quot;comienza con&quot; producirán resultados mucho más rápidos que &quot;contiene&quot;. &quot;Is&quot; se ejecutará aún más rápido. Evite utilizar &quot;contiene&quot; con varios valores; ambos juntos pueden ralentizar aún más una campaña.
1. **Usar muestra aleatoria por sí sola:** la muestra aleatoria es un filtro especial. Úsalo solo para poner a tu gente en listas prefabricadas. A continuación, solo tiene que usar &quot;Miembro de lista&quot; para que su lista inteligente sea muy rápida. La muestra aleatoria **NO** funcionará con listas inteligentes anidadas. El filtro de muestra aleatoria no funcionará si se hace referencia a la lista inteligente para el filtro &quot;Miembro de lista inteligente&quot;.
1. **Ahorre con los filtros de inactividad -** Los filtros como &quot;Formulario no rellenado&quot; pueden ser muy útiles, pero requieren mucha más potencia de procesamiento.
1. **Ahorre con el pegado de varios valores:** La selección múltiple está diseñada para pegar docenas o posiblemente cientos de valores. Pon demasiados, sin embargo, y se desacelerará mucho.
1. **Ahorre tiempo al agregar restricciones -** Estos son los pequeños detalles de una regla y los valores relacionados. Cuantas más restricciones agregue, más lento será el tiempo de procesamiento.
1. **Simplifique sus campañas:** más de 100 reglas independientes (¡ya las hemos visto!) obviamente tardarán algún tiempo en procesarse. Sea sencillo y notará las mejoras de velocidad, además de que le resultará más fácil de entender.
1. **Incluya el símbolo @ antes del nombre de dominio al usar el filtro de dirección de correo electrónico** **-**. Esto hace que utilice una consulta más rápida. Ejemplo: en lugar de usar _email contiene &#39;somedomain.com&#39;_, use _email contiene &#39;@somedomain.com_&#39;. Si utiliza varias direcciones de correo electrónico con &quot;contiene&quot;, TODOS deben comenzar por &quot;@&quot;.

>[!TIP]
>
>Marketo Engage se puede utilizar de muchas maneras y ciertas técnicas son mejores para usted y su empresa. Póngase en contacto con su representante de ventas de Adobe Professional Services si desea obtener ayuda para sacar el máximo partido a su inversión.
