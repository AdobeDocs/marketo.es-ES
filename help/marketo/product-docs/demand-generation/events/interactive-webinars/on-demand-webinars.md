---
description: Seminarios Web Bajo Demanda - Documentos De Marketo - Documentación Del Producto
title: Seminarios web bajo demanda
hide: true
hidefromtoc: true
feature: Interactive Webinars
source-git-commit: 49a75b6aef25787a68554dff3a847279ef8ba12a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Seminarios web bajo demanda {#on-demand-webinars}

Los seminarios web a petición capturan y perfeccionan los posibles clientes que se registraron en el evento y que no asistieron, pero que desean obtener información relacionada con el evento observando la grabación. Información como el nombre, el ID de correo electrónico y la fecha y duración de la observación se pueden recopilar en Marketo Engage y utilizar para dirigirse a estos posibles clientes que no se muestran.

La URL de unión al seminario web que se compartió con los inscritos antes del evento se puede utilizar como vínculo para ver la grabación bajo demanda. Una vez que un solicitante de registro, que no ha asistido al evento en directo (es decir, un posible cliente con el estado de programa como &quot;No presentarse&quot;), hace clic en la URL de unión al seminario web, el estado del programa de dicho posible cliente cambia de &quot;No presentarse&quot; a &quot;Asistido bajo demanda&quot;. Tenga en cuenta que el estado del programa de los posibles clientes que han visto el evento en directo y tienen el estado &quot;Asistido&quot; no se verá afectado aunque visiten la URL de unión y vean la grabación bajo demanda.

Adobe Connect, la tecnología que alimenta los seminarios web interactivos, realiza un seguimiento de la visita y de la duración del seguimiento de los posibles clientes que han visto la grabación, e informa de ello diariamente a Marketo. La grabación está disponible en la URL de unión durante 30 días después del evento y la duración es fija.

Marketo proporciona las estadísticas de inspección para los seminarios web bajo demanda en la pestaña Tablero con la ayuda de los dos widgets siguientes:
1. Resumen a petición: Proporciona un resumen diario del recuento de visitantes (no-espectadores) que han visto la grabación después del evento.
2. Estadísticas a petición: Estos widgets proporcionan información sobre: a. Días en los que el registro a petición está disponible para su visualización. Esto puede ayudar a los especialistas en marketing a realizar acciones como ejecutar campañas de correo electrónico más cerca del final de la duración de disponibilidad del registro de 30 días.
b. Recuento total de visitantes para seminarios web a petición hasta la fecha. Este sería el recuento de todos los inscritos que han visto la grabación bajo demanda hasta la fecha.
c. Duración media de la visualización en minutos para todos los visitantes. Esto daría al experto en marketing una idea de qué proporción de la grabación se visualiza y qué campañas inteligentes se pueden utilizar para dirigirse a posibles clientes por encima de una determinada duración de reloj.

CAPTURA DE PANTALLA

Los filtros y déclencheur de los seminarios web interactivos se han modificado para adaptarlos a los seminarios web bajo demanda. El déclencheur &quot;Asiste al evento&quot; y el filtro &quot;Ha asistido al evento&quot; se añaden con una restricción adicional &quot;Modo de evento&quot; en el que un experto en marketing puede elegir si el objetivo es una audiencia en directo o bajo demanda. Si la restricción &quot;Modo de evento&quot; no está seleccionada, las audiencias En directo y Bajo demanda serán el objetivo. Otras restricciones como &quot;Fecha de observación&quot; y &quot;Duración de la observación&quot; se podrían utilizar con el modo de evento &quot;Bajo demanda&quot;. El filtro de inactividad &quot;No ha asistido a un evento&quot; también se puede utilizar para seminarios web a petición con el modo de evento &quot;Bajo demanda&quot;.
