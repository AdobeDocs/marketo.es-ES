---
unique-page-id: 10096583
description: ' [!DNL Munchkin] Preguntas frecuentes sobre el seguimiento de próxima generación - Documentos de Marketo - Documentación del producto'
title: Preguntas frecuentes sobre seguimiento  [!DNL Munchkin] de próxima generación
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Preguntas frecuentes sobre el seguimiento de [!DNL Munchkin] de próxima generación {#next-generation-munchkin-tracking-faq}

Estamos encantados de anunciar que pronto comenzaremos un despliegue gradual de nuestra tecnología de seguimiento web de próxima generación.

Estas son las cosas más importantes que debe saber:

* Eliminamos el filtro de lista inteligente &quot;Is Anonymous&quot; con nuestra versión del primer trimestre (ya completada)
* Estamos aumentando el número de eventos web (Visite la página web, Haga clic en el enlace en la página web) que podemos ingerir
* Su código de [!DNL Munchkin] no cambiará, por lo que no se requieren actualizaciones en el sitio web

## ¿Cuándo tendrá lugar mi suscripción a Marketo en [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Aún no tenemos una fecha exacta, pero vuelva a consultar esta página para ver las últimas novedades.

## ¿Necesito hacer algún cambio en mi seguimiento de [!DNL Munchkin] en mi sitio web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. El código de seguimiento [!DNL Munchkin] sigue siendo el mismo. No es necesario realizar cambios en el sitio web.

>[!NOTE]
>
>Este cambio no afecta a Web Personalization (Real-Time Personalization). Sigue identificando visitantes web anónimos y conocidos, y personalizando el contenido en tiempo real para estos visitantes.

## ¿Por qué Marketo eliminó el filtro &quot;Es anónimo&quot; de las listas inteligentes? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Hemos cambiado la forma en que las personas anónimas interactúan con las campañas inteligentes. Antes, fluían a través de una campaña inteligente, al igual que la gente conocida. El filtro &quot;Es anónimo&quot; se utilizó para especificar que solo las personas conocidas o anónimas fluyen a través de la campaña.

Con [!DNL Munchkin] V2, seguiremos realizando el seguimiento de todas las actividades anónimas; sin embargo, ya no podrá aplicar filtros a las personas anónimas. En el momento de la conversión (cuando la persona se conoce en Marketo), todas las actividades que se produjeron cuando la persona era anónima se anexan al registro de actividad de la persona y, en este momento, fluyen a través de las campañas para las que cumplen los requisitos.

Si ya está utilizando este filtro en una lista inteligente (por ejemplo, en una campaña inteligente o un informe), no se elimina automáticamente de la lista inteligente. Consulte a continuación para obtener más información.

>[!NOTE]
>
>**Déclencheur**: visita la página web, la página web es una página de precios
>>**Flujo**: cambiar puntuación +10 y momento interesante
>>**Web**: página de precios vista
>
>Con [!DNL Munchkin] V2, si una persona anónima visita la página de precios, no ingresa a la campaña inmediatamente. En el momento en que la persona anónima sea conocida, haremos esta campaña con ella. Lo hará:
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

[Información general sobre actualizaciones anónimas de posibles clientes](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Actualizaciones anónimas de posibles clientes - Cambios dentro de la interfaz de usuario de Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Actualizaciones anónimas de clientes potenciales: se necesita la acción del cliente](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Actualizaciones anónimas de posibles clientes - Informes de Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Actualizaciones anónimas de posibles clientes - Programación de versiones](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Actualizaciones De Posibles Clientes Anónimas - Bajo El Capó](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promoción de posible cliente anónima a posible cliente conocido - [!DNL Munchkin] Comportamiento de la versión 2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## ¡Tengo más preguntas! ¿Cómo puedo conseguir que me respondan? {#i-have-more-questions-how-do-i-get-them-answered}

Póngase en contacto con la [comunidad](https://nation.marketo.com/){target="_blank"}. También puede ponerse en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. Estarán encantados de responder a sus preguntas.
