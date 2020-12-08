---
unique-page-id: 10096583
description: Preguntas más frecuentes sobre el seguimiento de Munchkin de próxima generación - Documentos de marketing - Documentación del producto
title: Preguntas más frecuentes sobre el seguimiento de Munchkin de próxima generación
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Preguntas más frecuentes sobre el seguimiento de Munchkin de próxima generación {#next-generation-munchkin-tracking-faq}

Estamos emocionados de anunciar que pronto comenzaremos un lanzamiento gradual de nuestra tecnología de seguimiento web de próxima generación.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Aquí están las cosas más importantes que hay que saber:

* Eliminamos el filtro de Lista inteligente &quot;Es anónimo&quot; con nuestra versión del primer trimestre (ya está listo)
* Aumentamos el número de eventos Web (visita a la página Web, clic en vínculo en la página Web) que podemos ingerir
* El código de Munchkin no cambiará, por lo que no se requieren actualizaciones en su sitio web

## ¿Cuándo estará mi suscripción de Marketing en Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Todavía no tenemos una fecha exacta, pero por favor, vuelva aquí para ver las actualizaciones.

## ¿Tendré que hacer algún cambio en mi seguimiento de Munchkin en mi sitio web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. El código de seguimiento Munchkin sigue siendo el mismo. No es necesario realizar cambios en el sitio web.

>[!NOTE]
>
>Este cambio no afecta a la Personalización web (Personalización en tiempo real). Sigue identificando visitantes web anónimos y conocidos y personalizando contenido en tiempo real para estos visitantes.

## ¿Por qué Marketo eliminó el filtro &quot;Es anónimo&quot; de las Listas inteligentes? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Hemos cambiado la forma en que las personas anónimas interactúan con Campañas inteligentes. Antes, fluían a través de una campaña inteligente, como la gente conocida. El filtro &quot;Es anónimo&quot; se utilizó para especificar que solo las personas conocidas o anónimas fluyen a través de la campaña.

Con Munchkin V2 seguiremos haciendo un seguimiento de todas las actividades anónimas; sin embargo, ya no se pueden aplicar filtros a personas anónimas. En el momento de la conversión (cuando la persona es conocida en el Marketing), todas las actividades que se produjeron cuando la persona fue anónima se anexan al registro de actividades de la persona y en este momento fluyen a través de las campañas para las que cumple los requisitos.

Si ya está utilizando este filtro en una Lista inteligente (por ejemplo, en una Campaña inteligente o un informe), no se elimina automáticamente de la Lista inteligente. Consulte a continuación para obtener más detalles.

>[!NOTE]
>
>**Ejemplo**
>
>**Activador**: Página Web Visitas, Página Web Precios\
>**Flujo**: Cambiar puntuación +10 y momento interesante, **Web**: Página Precios visualizados
>
>Con Munchkin V2, si una persona anónima visita la página de precios, no entra en la campaña inmediatamente. En el momento en que la persona anónima sea conocida, le haremos esta campaña. Ella:
>
>* Obtener una puntuación de 10
   >
   >
* Tener la actividad de página Web establecida en la fecha correcta (cuando realmente visitó)
   >
   >
* Tener un momento interesante registrado para ella (con la fecha en que realmente visitó la página, no cuando se dio a conocer)
   >
   >
* Se ha registrado una actividad &quot;Persona nueva&quot;, como sucede hoy

>



## ¿Qué pasa con mis Listas inteligentes que ya tienen el filtro &quot;Es anónimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Después de nuestra versión 16 de invierno, si tiene Campañas inteligentes antiguas con una Lista inteligente que tiene el filtro &quot;Es anónimo&quot;, sucederá una de las dos cosas:

1. Si la Lista inteligente tiene el filtro &quot;Is Anonymous = False&quot;, entonces no sucederá nada. Lo ignoraremos.
1. Si la Lista inteligente tiene el filtro &quot;Is Anonymous = True&quot;, esta campaña fallará y se le enviará una notificación.

## Llevo un tiempo usando Marketo. ¿Cómo sé cuál de mis campañas usa el filtro &quot;Es anónimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de realizar este cambio, enviamos varias notificaciones semanales a la bandeja de entrada de notificaciones con una lista de Listas inteligentes, Campañas inteligentes e informes que utilizan el filtro &quot;Es anónimo&quot;. Esto puede ayudarle a identificar dónde está utilizando este filtro.

Por favor, remítalos e identifíquense dónde tiene &quot;Is Anonymous&quot; establecido en True, ya que estas son las campañas que se ven afectadas. La mayoría de las veces, los clientes utilizan esta configuración para obtener algún tipo de puntuación. Consulte el ejemplo anterior para comprender cómo funcionarán estas campañas ahora.

## Quisiera documentación más detallada. ¿Dónde puedo encontrarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consulte estos vínculos:

[Información general sobre las actualizaciones de posibles clientes anónimas](https://nation.marketo.com/docs/DOC-2937)

[Actualizaciones de posibles clientes anónimas: cambios dentro de la interfaz de usuario de Marketing](https://nation.marketo.com/docs/DOC-2938)

[Actualizaciones de posibles clientes anónimas: se requiere la acción del cliente](https://nation.marketo.com/docs/DOC-2939)

[Actualizaciones de posibles clientes anónimas: informes de Analytics](https://nation.marketo.com/docs/DOC-2940)

[Actualizaciones de posibles clientes anónimas: programación de la versión](https://nation.marketo.com/docs/DOC-2961)

[Actualizaciones de posibles clientes anónimas - Bajo el capó](https://nation.marketo.com/docs/DOC-2962)

[Promoción de posibles clientes anónimos a posible cliente conocido - Comportamiento de Munchkin V2](https://nation.marketo.com/docs/DOC-2963)

## ¡Tengo más preguntas! ¿Cómo obtengo respuestas? {#i-have-more-questions-how-do-i-get-them-answered}

Por favor, contacte con la [comunidad](https://nation.marketo.com/welcome). También puede enviar un correo electrónico a [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#4c3f393c3c233e380c212d3e27293823622f232162) Ellos estarán encantados de responder sus preguntas.
