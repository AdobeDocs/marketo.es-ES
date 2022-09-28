---
unique-page-id: 10096583
description: 'Preguntas frecuentes sobre el seguimiento de Munchkin de próxima generación: Documentos de Marketo: Documentación del producto'
title: Preguntas frecuentes sobre el seguimiento de Munchkin de próxima generación
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Preguntas frecuentes sobre el seguimiento de Munchkin de próxima generación {#next-generation-munchkin-tracking-faq}

Estamos encantados de anunciar que pronto comenzaremos un despliegue gradual de nuestra tecnología de seguimiento web de próxima generación.

Estas son las cosas más importantes que hay que saber:

* Eliminamos el filtro de lista inteligente &quot;Es anónimo&quot; con nuestra versión del primer trimestre (ya hecho)
* Aumentamos el número de eventos web (Visita a la página web, Vínculo en la página web en el que se hizo clic) que podemos ingerir
* Su código de Munchkin no cambiará, por lo que no se requieren actualizaciones en su sitio web.

## ¿Cuándo estará mi suscripción a Marketo en Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Todavía no tenemos una fecha exacta, pero por favor, vuelva aquí para ver las actualizaciones.

## ¿Tendré que hacer algún cambio en mi seguimiento de Munchkin en mi sitio web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. El código de seguimiento de Munchkin sigue siendo el mismo. No es necesario realizar ningún cambio en el sitio web.

>[!NOTE]
>
>Este cambio no afecta a la personalización web (personalización en tiempo real). Sigue identificando visitantes web anónimos y conocidos y personalizando el contenido en tiempo real para estos visitantes.

## ¿Por qué Marketo ha eliminado el filtro &quot;Es anónimo&quot; de las listas inteligentes? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Hemos cambiado la forma en que las personas anónimas interactúan con las campañas inteligentes. Antes, pasaron por una campaña inteligente, igual que la gente conocida. El filtro &quot;Es anónimo&quot; se utilizó para especificar que solo las personas conocidas o anónimas fluyen a través de la campaña.

Con Munchkin V2, seguiremos haciendo un seguimiento de todas las actividades anónimas; sin embargo, ya no puede aplicar filtros a personas anónimas. En el momento de la conversión (cuando la persona se conoce en Marketo), todas las actividades que se produjeron cuando la persona era anónima se anexan al registro de actividades de la persona y en ese momento fluyen por las campañas para las que cumple los requisitos.

Si ya está utilizando este filtro en una lista inteligente (por ejemplo, en una campaña inteligente o un informe), no se elimina automáticamente de la lista inteligente. Consulte a continuación para obtener más información.

>[!NOTE]
>
>**Déclencheur**: Visita Página Web, Página Web es Página de Precios\
>**Flujo**: Cambio de puntuación +10 y momento interesante
>**Web**: Página Precios visualizados
>
>Con Munchkin V2, si una persona anónima visita la página de precios, no entra inmediatamente en la campaña. En el momento en que la persona anónima sea conocida, le ejecutaremos esta campaña. Ella:
>
>* Obtener una puntuación de 10
>
>* Tener la actividad Página web configurada en la fecha correcta (cuando realmente visitó)
>
>* Tener un momento interesante registrado para ella (con la fecha en que realmente visitó la página, no cuando se dio a conocer)
>
>* Tener una actividad &quot;Nueva persona&quot; registrada, tal como es hoy


## ¿Qué sucede con mis listas inteligentes que ya tienen el filtro &quot;Es anónimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Después de nuestra versión de invierno 16, si tiene campañas inteligentes antiguas con una lista inteligente que tiene el filtro &quot;Es anónimo&quot;, sucederá una de dos cosas:

1. Si la lista inteligente tiene el filtro &quot;Is Anonymous = False&quot;, no ocurrirá nada. Lo ignoraremos.
1. Si la lista inteligente tiene el filtro &quot;Is Anonymous = True&quot;, esta campaña fallará y se le enviará una notificación.

## Llevo un tiempo usando Marketo. ¿Cómo sé cuál de mis campañas usa el filtro &quot;Es anónimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de realizar este cambio, enviamos varias notificaciones semanales a la bandeja de entrada de notificaciones con una lista de listas inteligentes, campañas inteligentes e informes que utilizan el filtro &quot;Es anónimo&quot;. Esto puede ayudarle a identificar dónde está utilizando este filtro.

Revise las campañas e identifique dónde tiene &quot;Is Anonymous&quot; establecido en True, ya que estas son las campañas que se ven afectadas. La mayoría de las veces, los clientes utilizan esta configuración para obtener algún tipo de puntuación. Consulte el ejemplo anterior para comprender cómo funcionarán ahora estas campañas.

## Quisiera documentación más detallada. ¿Dónde puedo encontrarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consulte estos vínculos:

[Información general sobre las actualizaciones de posibles clientes anónimas](https://nation.marketo.com/docs/DOC-2937){target=&quot;_blank&quot;}

[Actualizaciones de posibles clientes anónimas: cambios dentro de la interfaz de usuario de Marketo](https://nation.marketo.com/docs/DOC-2938){target=&quot;_blank&quot;}

[Actualizaciones de posibles clientes anónimas: se necesita la acción del cliente](https://nation.marketo.com/docs/DOC-2939){target=&quot;_blank&quot;}

[Actualizaciones de posibles clientes anónimas: informes de Analytics](https://nation.marketo.com/docs/DOC-2940){target=&quot;_blank&quot;}

[Actualizaciones anónimas de posibles clientes: programación de versiones](https://nation.marketo.com/docs/DOC-2961){target=&quot;_blank&quot;}

[Actualizaciones anónimas de posibles clientes: en el capó](https://nation.marketo.com/docs/DOC-2962){target=&quot;_blank&quot;}

[Promoción de posibles clientes anónimos a posible cliente conocido: Comportamiento de Munchkin V2](https://nation.marketo.com/docs/DOC-2963){target=&quot;_blank&quot;}

## ¡Tengo más preguntas! ¿Cómo obtengo respuestas? {#i-have-more-questions-how-do-i-get-them-answered}

Póngase en contacto con el [comunidad](https://nation.marketo.com/){target=&quot;_blank&quot;}. También puede ponerse en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}. Estarán felices de responder a sus preguntas.
