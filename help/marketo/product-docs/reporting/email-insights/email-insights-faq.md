---
unique-page-id: 10100257
description: Preguntas más frecuentes sobre las perspectivas de correo electrónico - Documentos de marketing - Documentación del producto
title: Preguntas más frecuentes sobre las perspectivas de correo electrónico
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Preguntas más frecuentes sobre las perspectivas de correo electrónico {#email-insights-faq}

## ¿Existen diferencias entre las métricas de proporción con las perspectivas de correo electrónico y otros sistemas de informes de marketing y correo electrónico? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sí. Las perspectivas de correo electrónico correlacionan las métricas de participación con las métricas de envío correspondientes para el mismo correo electrónico enviado al calcular las tasas de métricas de participación (Tasa abierta, Tasa de clics hasta abrir, Tasa de cancelación de suscripciones). Por ejemplo: en Perspectivas de correo electrónico, al observar un gráfico de series temporales de la semana pasada con desgloses diarios de la tasa de clics hasta abrir, ahora mostramos la verdadera proporción correlacionada de eventos de apertura, clic y cancelación de suscripciones en base a las métricas de envíos correspondientes. Esto contrasta con el comportamiento del Explorador de ingresos, que simplemente resume todo. Email Insights presenta una vista más precisa de los índices de participación.

## ¿Por qué las perspectivas de correo electrónico solo admiten 10 Dimension personalizados? {#why-does-email-insights-only-support-custom-dimensions}

En muchos casos de uso, ampliar las dimensiones predeterminadas del sistema con 10 dimensiones personalizadas adicionales será más que suficiente e incluye dimensiones personalizadas basadas en segmentos o etiquetas de Programa. En el futuro, planeamos permitir que los clientes aumenten el número de Dimension personalizados permitidos.

## ¿Por qué no puedo reutilizar las ranuras de Dimension personalizados después de haberlas asignado? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una vez asignada una ranura de Dimension personalizado determinada, la reasignación de la misma provocaría que los datos anteriores produjeran un error al combinarse con un nuevo significado. Debido a esto, es posible que las ranuras de Dimension personalizadas no se vuelvan a utilizar. Este comportamiento es coherente con el de otras herramientas de análisis de métricas, como Google Analytics.

## ¿Las perspectivas de correo electrónico son compatibles con los correos electrónicos de perspectiva de ventas de marketing? {#does-email-insights-support-marketo-sales-insight-emails}

Sí. Todos los mensajes de correo electrónico enviados a través de Marketo Sales Insights se incluyen en Email Insights.

## ¿Las perspectivas de correo electrónico son compatibles con los correos electrónicos operativos? {#does-email-insights-support-operational-emails}

Sí. De forma predeterminada, los mensajes de correo electrónico operativos están ocultos en la vista y las consultas. Sin embargo, puede cambiar esta configuración en el panel Ajustes personales.

## ¿Las perspectivas de correo electrónico capturan los pasos recurrentes del flujo de correo electrónico de Campaña inteligente programados o reejecutados? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sí y No. Con la versión inicial de Perspectivas de correo electrónico, todos los eventos de correo electrónico se capturan y se puede acceder a ellos para cualquier Campaña inteligente recurrente programada o que se vuelva a ejecutar. Pero no se podrá diferenciar entre las distintas ejecuciones de esa Campaña inteligente. En nuestra próxima versión agregaremos asistencia para capturar la información de ejecución de Campaña inteligente para los eventos Abrir, Clic y Cancelar suscripción, a fin de diferenciar.

## ¿Por qué muchas métricas muestran cero cuando filtro por tipo de dispositivo o sistema operativo del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Con la excepción de Clics hasta la tasa de apertura, Aperturas, Clics y Cancelaciones de suscripción, todas las demás métricas admitidas son eventos de envío o tasas derivadas de eventos de envío. Dado que el tipo de dispositivo y el sistema operativo del dispositivo solo se aplican a las métricas de compromiso, simplemente no tenemos la información que mostrar. Por ejemplo, es una consulta no definida solicitar la tasa de Envío cuando se filtra por tipo de dispositivo = móvil, ya que Marketing no habría recibido ninguna métrica de compromiso para los eventos de Envío y envío subyacentes. Estamos explorando formas de aplicar el tipo de dispositivo y el sistema operativo del dispositivo a partir de las métricas de compromiso para las relaciones que comprenden las métricas de compromiso y Envío.

## ¿Qué hace Email Insights cuando ciertos clientes de correo electrónico bloquean imágenes? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema común del sector es que un número creciente de clientes de correo electrónico desactivan las imágenes de forma predeterminada. La carga de imágenes es la base de cómo se graban las aperturas. Es totalmente posible que un usuario reciba un correo electrónico con imágenes bloqueadas, pero con el texto y los vínculos totalmente legibles. Si un usuario lo experimentara y hacía clic en un vínculo de ese correo electrónico, acabaría con un escenario de un evento de clics, pero sin el correspondiente evento de apertura para dicho correo electrónico. Las perspectivas de correo electrónico de marketing generarán automáticamente los eventos que faltaban. La lógica es idéntica a la de Marketo para el informe Rendimiento del correo electrónico, así como para el área Análisis del correo electrónico en el Explorador de ingresos.
