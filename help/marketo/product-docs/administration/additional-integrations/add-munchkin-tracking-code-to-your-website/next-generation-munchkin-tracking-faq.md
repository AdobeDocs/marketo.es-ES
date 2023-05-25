---
unique-page-id: 10096583
description: "Nueva generación [!DNL Munchkin] Preguntas frecuentes sobre el seguimiento - Documentos de Marketo - Documentación del producto"
title: "Nueva generación [!DNL Munchkin] Preguntas frecuentes sobre seguimiento"
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Próxima generación [!DNL Munchkin] Preguntas frecuentes sobre seguimiento {#next-generation-munchkin-tracking-faq}

Estamos encantados de anunciar que pronto comenzaremos un despliegue gradual de nuestra tecnología de seguimiento web de próxima generación.

Estas son las cosas más importantes que debe saber:

* Eliminamos el filtro de lista inteligente &quot;Is Anonymous&quot; con nuestra versión del primer trimestre (ya completada)
* Estamos aumentando el número de eventos web (Visite la página web, Haga clic en el enlace en la página web) que podemos ingerir
* Su [!DNL Munchkin] El código de no cambiará, por lo que no se requieren actualizaciones en el sitio web

## ¿Cuándo estará activada mi suscripción a Marketo? [!DNL Munchkin] ¿V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Aún no tenemos una fecha exacta, pero vuelva a consultar esta página para ver las últimas novedades.

## ¿Debo realizar algún cambio en mi [!DNL Munchkin] seguimiento en mi sitio web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. El [!DNL Munchkin] el código de seguimiento sigue siendo el mismo. No es necesario realizar cambios en el sitio web.

>[!NOTE]
>
>Este cambio no afecta a la personalización web (personalización en tiempo real). Sigue identificando visitantes web anónimos y conocidos, y personalizando el contenido en tiempo real para estos visitantes.

## ¿Por qué Marketo eliminó el filtro &quot;Es anónimo&quot; de las listas inteligentes? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Hemos cambiado la forma en que las personas anónimas interactúan con las campañas inteligentes. Antes, fluían a través de una campaña inteligente, al igual que la gente conocida. El filtro &quot;Es anónimo&quot; se utilizó para especificar que solo las personas conocidas o anónimas fluyen a través de la campaña.

Con [!DNL Munchkin] V2, seguiremos realizando el seguimiento de todas las actividades anónimas; sin embargo, ya no podrá aplicar filtros a personas anónimas. En el momento de la conversión (cuando la persona se conoce en Marketo), todas las actividades que se produjeron cuando la persona era anónima se anexan al registro de actividad de la persona y, en este momento, fluyen a través de las campañas para las que cumplen los requisitos.

Si ya está utilizando este filtro en una lista inteligente (por ejemplo, en una campaña inteligente o un informe), no se elimina automáticamente de la lista inteligente. Consulte a continuación para obtener más información.

>[!NOTE]
>
>**Déclencheur**: Visita la página web, la página web es una página de precios\
>**Flujo**: Cambiar puntuación +10 y momento interesante
>**Web**: Página de precios vista
>
>Con [!DNL Munchkin] V2, si una persona anónima visita la página de precios, no entra en la campaña inmediatamente. En el momento en que la persona anónima sea conocida, haremos esta campaña con ella. Lo hará:
>
>* Obtenga una puntuación de 10
>
>* Establezca la actividad de la página web en la fecha correcta (cuando realizó la visita)
>
>* Tener un momento interesante registrado para ella (con la fecha en la que realmente visitó la página, no cuando se dio a conocer)
>
>* Registre una actividad &quot;Nueva persona&quot;, tal como está hoy


## ¿Qué les sucede a mis listas inteligentes que ya tienen el filtro &quot;Es anónimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Después de la versión de invierno de 2016, si tiene campañas inteligentes antiguas con una lista inteligente que contiene el filtro &quot;Es anónimo&quot;, ocurrirá una de estas dos cosas:

1. Si la Smart List tiene el filtro &quot;Is Anonymous = False&quot;, no ocurrirá nada. Lo vamos a ignorar.
1. Si la lista inteligente tiene el filtro &quot;Is Anonymous = True&quot;, esta campaña fallará y se le enviará una notificación.

## He estado usando Marketo por un tiempo. ¿Cómo sé cuál de mis campañas utiliza el filtro &quot;Es anónimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de realizar este cambio, enviamos varias notificaciones semanales a su bandeja de entrada de notificaciones con una lista de listas inteligentes, campañas inteligentes e informes que utilizan el filtro &quot;Es anónimo&quot;. Esto puede ayudarle a identificar dónde está utilizando actualmente este filtro.

Revíselas e identifique dónde tiene &quot;Is Anonymous&quot; establecido en True, ya que estas son las campañas afectadas. La mayoría de las veces, los clientes utilizan esta configuración para algún tipo de puntuación. Consulte el ejemplo anterior para comprender cómo funcionarán ahora estas campañas.

## Me gustaría una documentación más detallada. ¿Dónde puedo encontrarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consulte estos vínculos:

[Resumen de actualizaciones de posibles clientes anónimas](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Actualizaciones anónimas de posibles clientes: cambios en la IU de Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Actualizaciones anónimas de posibles clientes: se necesita la acción del cliente](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Actualizaciones de posibles clientes anónimas: informes de Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Actualizaciones anónimas de posibles clientes: programación de versiones](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Actualizaciones de clientes potenciales anónimas: bajo el capó](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promoción de cliente potencial anónimo a cliente potencial conocido - [!DNL Munchkin] Comportamiento de V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## ¡Tengo más preguntas! ¿Cómo puedo conseguir que me respondan? {#i-have-more-questions-how-do-i-get-them-answered}

Póngase en contacto con el [comunidad](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. Estarán encantados de responder a sus preguntas.
