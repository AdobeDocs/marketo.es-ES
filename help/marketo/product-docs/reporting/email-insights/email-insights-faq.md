---
unique-page-id: 10100257
description: Preguntas frecuentes sobre las perspectivas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre Email Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Preguntas frecuentes sobre Email Insights {#email-insights-faq}

## ¿Hay alguna diferencia entre las métricas de proporción con Email Insights y otros informes de correo electrónico de Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sí. Perspectivas de correo electrónico correlaciona las métricas de participación con sus métricas de entrega correspondientes para el mismo correo electrónico enviado al calcular las proporciones de métricas de participación (Tasa de apertura, Tasa de clics hasta la apertura, Tasa de cancelación de suscripción). Por ejemplo, en las Perspectivas de correo electrónico, cuando se mira un gráfico de series temporales de la semana pasada con desgloses diarios de tasa de clics a apertura, ahora mostramos la proporción real correlacionada de eventos de apertura/clic/cancelación de suscripción en función de las métricas de entrega correspondientes. Esto contrasta con el comportamiento en el Explorador de ingresos, que simplemente resume todo. Perspectivas de correo electrónico presenta una vista más precisa de las proporciones de participación.

## ¿Por qué Email Insights solo admite 10 Dimension personalizados? {#why-does-email-insights-only-support-custom-dimensions}

En muchos casos de uso, ampliar las dimensiones predeterminadas del sistema con 10 dimensiones personalizadas adicionales será más que adecuado, e incluye dimensiones personalizadas basadas en segmentaciones o etiquetas de programa. En el futuro, planeamos permitir que los clientes aumenten el número de Dimension personalizados permitidos.

## ¿Por qué no puedo reutilizar las ranuras de Dimension personalizados después de haberlas asignado? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una vez que se ha asignado una ranura de Dimension personalizado determinada, la reasignación haría que los datos anteriores produjeran un error cuando se combinaran con un nuevo significado. Debido a esto, es posible que las ranuras para Dimension personalizados no se puedan reutilizar. Este comportamiento es coherente con el de otras herramientas de análisis de métricas, como los Google Analytics.

## ¿Las perspectivas de correo electrónico admiten los correos electrónicos de perspectivas de ventas de Marketo? {#does-email-insights-support-marketo-sales-insight-emails}

Sí. Todos los correos electrónicos enviados a través de Información de ventas de Marketo se incluyen en Información de correo electrónico.

## ¿Email Insights admite los correos electrónicos operativos? {#does-email-insights-support-operational-emails}

Sí. De forma predeterminada, los correos electrónicos operativos están ocultos para su visualización y consulta. Sin embargo, puede cambiar esta configuración en el panel Configuración personal.

## ¿Insights de correo electrónico captura los pasos recurrentes del flujo de correo electrónico de Smart Campaign programados o ejecutados de nuevo? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sí y No. Con la versión inicial de las Perspectivas de correo electrónico, todos los eventos de correo electrónico se capturan y son accesibles para cualquier campaña inteligente recurrente programada o que se vuelva a ejecutar. Pero no podrá diferenciar entre diferentes ejecuciones de esa campaña inteligente. En la próxima versión añadiremos la compatibilidad para capturar la información de ejecución de la campaña inteligente para los eventos Open, Click y Unsubscribe con el fin de diferenciar.

## ¿Por qué muchas métricas muestran cero cuando filtro por tipo de dispositivo o sistema operativo del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Con la excepción de Clic para abrir tasa, Aperturas, Clics y Cancelaciones de suscripción, todas las demás métricas admitidas son eventos de entrega o proporciones derivadas de eventos de entrega. Dado que Tipo de dispositivo y Sistema operativo del dispositivo solo se aplican a las métricas de participación, simplemente no tenemos la información que mostrar. Por ejemplo, si se filtra por Tipo de dispositivo = móvil, se trata de una consulta sin definir para solicitar la Tasa de entrega, ya que Marketo no habría recibido ninguna métrica de participación para los eventos de entrega y envío subyacentes. Estamos explorando maneras de aplicar el tipo de dispositivo y el sistema operativo del dispositivo desde las métricas de participación para relaciones compuestas por métricas de participación y entrega.

## ¿Qué hace Insights de correo electrónico cuando ciertos clientes de correo electrónico bloquean imágenes? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema común del sector es el creciente número de clientes de correo electrónico que desactivan las imágenes de forma predeterminada. La carga de imágenes es la base de cómo se graban las aperturas. Es totalmente posible que un usuario reciba un correo electrónico con imágenes bloqueadas, pero con el texto y los vínculos totalmente legibles. Si un usuario experimentara esto y hiciera clic en un vínculo de ese correo electrónico, terminaría con el escenario de un evento de clic, pero no el evento de apertura correspondiente para ese correo electrónico. Marketo Email Insights generará automáticamente cualquier evento que falte. La lógica es idéntica a cómo lo hace Marketo para el informe de rendimiento de correo electrónico, así como para el área de análisis de correo electrónico del Explorador de ingresos.
