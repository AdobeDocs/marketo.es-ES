---
unique-page-id: 7512524
description: Obtenga ayuda sobre las prácticas recomendadas para listas inteligentes. Cree listas más rápidas y precisas con estas sugerencias.
title: Prácticas recomendadas para listas inteligentes
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
TQID: https://experienceleague.adobe.com/Z1k--jj24QHIEThtPbj29i9FBhcEp0Hf9hBeZEgSP3w
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 592
ht-degree: 2%

---

# Prácticas recomendadas para listas inteligentes {#best-practices-for-smart-lists}

Las listas inteligentes son la herramienta de consulta más potente del entorno de marketing. Encuentra a las personas que buscas con una velocidad y facilidad mágicas.

Para que sea más fácil trabajar con ellos y optimizar el rendimiento, se proporcionan las siguientes prácticas recomendadas.

>[!NOTE]
>
>**Cada usuario de Marketo Engage es diferente.** Cuanto mayor sea la base de datos, más se procesa. Cuantas más actividades haya almacenado, más tardará en buscarlas.
>
>Si está experimentando lentitud, pruebe las sugerencias a continuación. Si el problema continúa, comuníquese con [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Limitar historial -** Los filtros de historial (también conocidos como filtros de actividad) se encuentran entre las operaciones que consumen más tiempo y recursos. Si debe utilizarlos, intente limitar el intervalo de fechas al más corto posible, lo que reduciría el conjunto de datos en el que se pueden buscar. Además, los intervalos de fechas no sustituyen a los períodos de retención. Ejemplo: Si la actividad que está consultando tiene un período de retención de 90 días y elige &quot;últimos 100 días&quot;, solo se devolverán los resultados de los últimos 90 días. Los períodos de retención de actividades [se pueden encontrar aquí](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limitar listas inteligentes anidadas -** Al crear una nueva lista inteligente, limite la cantidad de filtros de &quot;Miembro de lista inteligente&quot; utilizados. Esto se denomina anidar listas inteligentes y cada lista inteligente a la que se haga referencia aumentará el tiempo de procesamiento. En su lugar, haga referencia a listas estáticas o utilice [segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Use operadores positivos sobre negativos -** Aunque los filtros &quot;no&quot; están disponibles, tienen que buscar en todo el conjunto de datos de su instancia, lo que puede consumir mucho tiempo. Los filtros &quot;es&quot; positivos pueden aprovechar algoritmos de búsqueda más eficaces.
1. **Evite el uso de &quot;contiene&quot; -** Si solo dispone de datos parciales, los calificadores &quot;comienza con&quot; producirán resultados mucho más rápidos que &quot;contiene&quot;. &quot;Is&quot; se ejecutará aún más rápido. Evite utilizar &quot;contiene&quot; con varios valores; ambos juntos pueden ralentizar aún más una campaña.
1. **Usar muestra aleatoria por sí sola:** la muestra aleatoria es un filtro especial. Úsalo solo para poner a tu gente en listas prefabricadas. A continuación, utilice &quot;Miembro de lista&quot; para que su lista inteligente sea muy rápida. La muestra aleatoria **NO** funcionará con listas inteligentes anidadas. El filtro de muestra aleatoria no funcionará si se hace referencia a la lista inteligente para el filtro &quot;Miembro de lista inteligente&quot;.
1. **Ahorre con los filtros de inactividad -** Los filtros como &quot;Formulario no rellenado&quot; pueden ser muy útiles, pero requieren mucha más potencia de procesamiento.
1. **Ahorre con el pegado de varios valores:** La selección múltiple está diseñada para pegar docenas o posiblemente cientos de valores. Pon demasiados, sin embargo, y se desacelerará mucho.
1. **Ahorre tiempo al agregar restricciones -** Estos son los pequeños detalles de una regla y los valores relacionados. Cuantas más restricciones agregue, más lento será el tiempo de procesamiento.
1. **Simplifique sus campañas:** más de 100 reglas independientes obviamente tardarán algún tiempo en procesarse. Sea sencillo y notará las mejoras de velocidad, además de que le resultará más fácil de entender.
1. **Incluya el símbolo @ antes del nombre de dominio al usar el filtro de dirección de correo electrónico** **-**. Esto hace que utilice una consulta más rápida. Ejemplo: en lugar de usar _email contiene &#39;somedomain.com&#39;_, use _email contiene &#39;@somedomain.com_&#39;. Si utiliza varias direcciones de correo electrónico con &quot;contiene&quot;, TODOS deben comenzar por &quot;@&quot;.

>[!TIP]
>
>Marketo Engage se puede utilizar de muchas maneras y ciertas técnicas son mejores para usted y su empresa. Póngase en contacto con su representante de ventas de Adobe Professional Services si desea obtener ayuda para sacar el máximo partido a su inversión.
