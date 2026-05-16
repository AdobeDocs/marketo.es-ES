---
unique-page-id: 10096583
description: Preguntas más frecuentes sobre el despliegue de seguimiento de  [!DNL Munchkin] próxima generación y el cambio de filtro de Is Anonymous.
title: Preguntas frecuentes sobre seguimiento  [!DNL Munchkin] de próxima generación
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
TQID: https://experienceleague.adobe.com/2kPRUe33THDYoIiP-yUDByqcJz5GPHoBnfDzRgwApNk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 705
ht-degree: 0%

---

# Preguntas frecuentes sobre el seguimiento de [!DNL Munchkin] de próxima generación {#next-generation-munchkin-tracking-faq}

Marketo está implementando la tecnología de seguimiento web de próxima generación por fases.

Estas son las cosas más importantes que debe saber:

* Se ha eliminado el filtro de la lista inteligente &quot;Es anónimo&quot;
* El número de eventos web (visitar la página web, hacer clic en el vínculo de una página web) que Marketo puede introducir va en aumento
* Su código de [!DNL Munchkin] no cambiará, por lo que no se requieren actualizaciones en el sitio web

## ¿Cuándo tendrá lugar mi suscripción a Marketo en [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Aún no está disponible una fecha exacta. Consulte esta página para ver las actualizaciones.

## ¿Necesito hacer algún cambio en mi seguimiento de [!DNL Munchkin] en mi sitio web? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

No. El código de seguimiento [!DNL Munchkin] sigue siendo el mismo. No es necesario realizar cambios en el sitio web.

>[!NOTE]
>
>Este cambio no afecta a Web Personalization (Real-Time Personalization). Sigue identificando visitantes web anónimos y conocidos, y personalizando el contenido en tiempo real para estos visitantes.

## ¿Por qué Marketo eliminó el filtro &quot;Es anónimo&quot; de las listas inteligentes? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketo ha cambiado la forma en que las personas anónimas interactúan con las campañas inteligentes. Antes, fluían a través de una campaña inteligente, al igual que la gente conocida. El filtro &quot;Es anónimo&quot; se utilizó para especificar que solo las personas conocidas o anónimas fluyen a través de la campaña.

Con [!DNL Munchkin] V2, Marketo seguirá realizando el seguimiento de todas las actividades anónimas; sin embargo, ya no podrá aplicar filtros a las personas anónimas. En el momento de la conversión (cuando la persona se conoce en Marketo), todas las actividades que se produjeron cuando la persona era anónima se anexan al registro de actividad de la persona y, en este momento, fluyen a través de las campañas para las que cumplen los requisitos.

Si ya está utilizando este filtro en una lista inteligente (por ejemplo, en una campaña inteligente o un informe), no se elimina automáticamente de la lista inteligente. Consulte a continuación para obtener más información.

>[!NOTE]
>
>**Déclencheur**: visita la página web, la página web es una página de precios >**Flujo**: cambiar puntuación +10 y momento interesante >**Web**: página de precios vista
>
>Con [!DNL Munchkin] V2, si una persona anónima visita la página de precios, no ingresa a la campaña inmediatamente. En el momento en que se conoce a la persona anónima, Marketo ejecuta esta campaña en ella. Ellos:
>
>* Obtenga una puntuación de 10
>
>* Establezca la actividad de la página web en la fecha correcta (cuando realizó la visita)
>
>* Tener un momento interesante registrado para ellos (con la fecha en la que realmente visitaron la página, no cuando se dieron a conocer)
>
>* Registre una actividad &quot;Nueva persona&quot;, tal como está hoy

## ¿Qué les sucede a mis listas inteligentes que ya tienen el filtro &quot;Es anónimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Después de la versión de invierno de 16, si tiene campañas inteligentes antiguas con una lista inteligente que contiene el filtro &quot;Es anónimo&quot;, ocurrirá una de estas dos cosas:

1. Si la Smart List tiene el filtro &quot;Is Anonymous = False&quot;, no ocurrirá nada. Se ignora.
1. Si la lista inteligente tiene el filtro &quot;Is Anonymous = True&quot;, esta campaña falla y se envía una notificación.

## He estado usando Marketo durante un tiempo. ¿Cómo sé cuál de mis campañas utiliza el filtro &quot;Es anónimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de este cambio, Marketo enviaba varias notificaciones semanales a su bandeja de entrada de notificaciones con una lista de listas inteligentes, campañas inteligentes e informes que utilizan el filtro &quot;Es anónimo&quot;. Esto puede ayudarle a identificar dónde está utilizando actualmente este filtro.

Revise e identifique dónde tiene &quot;Is Anonymous&quot; establecido en True, ya que estas son las campañas afectadas. La mayoría de las veces, este ajuste se utiliza para algún tipo de puntuación. Consulte el ejemplo anterior para comprender cómo funcionarán ahora estas campañas.

## Me gustaría una documentación más detallada. ¿Dónde puedo encontrarlo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Consulte estos vínculos:

[Resumen de actualizaciones de posibles clientes anónimas](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Actualizaciones anónimas de posibles clientes: cambios en la IU de Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Actualizaciones anónimas de posibles clientes: se necesita la acción del cliente](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Actualizaciones de posibles clientes anónimas: informes de Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Actualizaciones anónimas de posibles clientes: programación de versiones](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Actualizaciones de clientes potenciales anónimas: bajo el capó](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promoción de posible cliente anónima a posible cliente conocido - Comportamiento de  [!DNL Munchkin] V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## ¡Tengo más preguntas! ¿Cómo puedo conseguir que me respondan? {#i-have-more-questions-how-do-i-get-them-answered}

Visite la [Comunidad de Marketo](https://experienceleaguecommunities.adobe.com/?profile.language=es){target="_blank"}. También puede ponerse en contacto con el Soporte de Marketo. Ellos estarán encantados de responder a sus preguntas.
