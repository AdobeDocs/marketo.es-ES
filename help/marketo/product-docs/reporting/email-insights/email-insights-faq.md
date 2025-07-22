---
unique-page-id: 10100257
description: Preguntas frecuentes sobre las perspectivas de correo electrónico - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre Email Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Preguntas frecuentes sobre Email Insights {#email-insights-faq}

## ¿Hay alguna diferencia entre las métricas de proporción con [!UICONTROL Perspectivas de correo electrónico] y otros informes de correo electrónico de Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sí. [!UICONTROL Perspectivas de correo electrónico] correlaciona las métricas de participación con sus métricas de entrega correspondientes para el mismo correo electrónico enviado al calcular las proporciones de métricas de participación (Tasa de apertura, Tasa de clics a apertura, Tasa de cancelación de suscripción). Por ejemplo, en [!UICONTROL Email Insights], al mirar un gráfico de series temporales de la semana pasada con desgloses diarios de Click-to-Open-Rate, ahora mostramos la relación verdadera correlacionada de los eventos de apertura/clic/cancelación de suscripción en función de las métricas de entrega correspondientes. Esto contrasta con el comportamiento en el Explorador de ingresos, que simplemente resume todo. [!UICONTROL Perspectivas de correo electrónico] presenta una vista más precisa de las proporciones de participación.

## ¿Por qué [!UICONTROL Email Insights] solo admite 10 dimensiones personalizadas? {#why-does-email-insights-only-support-custom-dimensions}

En muchos casos de uso, ampliar las dimensiones predeterminadas del sistema con 10 dimensiones personalizadas adicionales será más que adecuado, e incluye dimensiones personalizadas basadas en segmentaciones o etiquetas de programa. En el futuro, planeamos permitir que los clientes aumenten el número de dimensiones personalizadas permitidas.

## ¿Por qué no puedo reutilizar las ranuras de dimensiones personalizadas después de haberlas asignado? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una vez que se ha asignado una ranura de Dimension personalizada determinada, la reasignación haría que los datos anteriores produjeran un error cuando se combinaran con un nuevo significado. Debido a esto, es posible que las ranuras de Dimension personalizadas no se reutilicen. Este comportamiento es coherente con el de otras herramientas de análisis de métricas, como Google Analytics.

## ¿[!UICONTROL Email Insights] admite correos electrónicos de Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sí. Todos los mensajes de correo electrónico enviados a través de Marketo Sales Insights se incluyen en [!UICONTROL Email Insights].

## ¿[!UICONTROL Email Insights] admite correos electrónicos operativos? {#does-email-insights-support-operational-emails}

Sí. De forma predeterminada, los correos electrónicos operativos están ocultos para su visualización y consulta. Sin embargo, puede cambiar esta configuración en el panel Configuración personal.

## ¿[!UICONTROL Perspectivas de correo electrónico] captura los pasos recurrentes del flujo de correo electrónico de Smart Campaign programados o ejecutados de nuevo? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sí y No. Con la publicación inicial de [!UICONTROL Email Insights], todos los eventos de correo electrónico se capturan y se puede acceder a ellos desde cualquier campaña inteligente recurrente programada o que se vuelva a ejecutar. Pero no podrá diferenciar entre diferentes ejecuciones de esa campaña inteligente. En la próxima versión añadiremos compatibilidad para capturar la información de ejecución de campañas inteligentes para los eventos Open, Click y Unsubscribe con el fin de diferenciar.

## ¿Por qué muchas métricas muestran cero cuando filtro por tipo de dispositivo o sistema operativo del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Con la excepción de Clic para abrir tasa, Aperturas, Clics y Cancelaciones de suscripción, todas las demás métricas admitidas son eventos de entrega o proporciones derivadas de eventos de entrega. Dado que Tipo de dispositivo y Sistema operativo del dispositivo solo se aplican a las métricas de participación, simplemente no tenemos la información que mostrar. Por ejemplo, si se filtra por Tipo de dispositivo = móvil, se trata de una consulta sin definir para solicitar la Tasa de entrega, ya que Marketo no habría recibido ninguna métrica de participación para los eventos de entrega y envío subyacentes. Estamos explorando maneras de aplicar el tipo de dispositivo y el sistema operativo del dispositivo desde las métricas de participación para relaciones compuestas por métricas de participación y entrega.

## ¿Qué hace [!UICONTROL Email Insights] cuando ciertos clientes de correo electrónico bloquean imágenes? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema común del sector es el creciente número de clientes de correo electrónico que desactivan las imágenes de forma predeterminada. La carga de imágenes es la base de cómo se graban las aperturas. Es totalmente posible que un usuario reciba un correo electrónico con imágenes bloqueadas, pero con el texto y los vínculos totalmente legibles. Si un usuario experimentara esto y hiciera clic en un vínculo de ese correo electrónico, terminaría con el escenario de un evento de clic, pero no el evento de apertura correspondiente para ese correo electrónico. Marketo Email Insights generará automáticamente cualquier evento que falte. La lógica es idéntica a cómo lo hace Marketo para el informe de rendimiento de correo electrónico, así como para el área de análisis de correo electrónico del Explorador de ingresos.
