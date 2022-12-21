---
unique-page-id: 10100257
description: Preguntas frecuentes sobre Email Insights - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre Email Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Preguntas frecuentes sobre Email Insights {#email-insights-faq}

## ¿Hay alguna diferencia entre las métricas de proporción con las Perspectivas de correo electrónico y otros informes de correo electrónico de Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sí. Las perspectivas de correo electrónico correlacionan las métricas de participación con las métricas de envío correspondientes para el mismo correo electrónico enviado al calcular las proporciones de métricas de participación (Tasa de apertura, Tasa de clics hasta el inicio, Tasa de cancelación de suscripciones). Por ejemplo, en Perspectivas de correo electrónico, al consultar un gráfico de series temporales de la semana pasada con desgloses diarios de la tasa de clics hasta el público, ahora se muestra la verdadera proporción correlacionada de eventos abiertos, de clics o de cancelación de suscripciones en función de las métricas de envío correspondientes. Esto contrasta con el comportamiento en el Explorador de ingresos, que simplemente resume todo. Perspectivas de correo electrónico presenta una vista más precisa de las tasas de participación.

## ¿Por qué Perspectivas de correo electrónico solo admite 10 Dimension personalizados? {#why-does-email-insights-only-support-custom-dimensions}

En muchos casos de uso, ampliar las dimensiones predeterminadas del sistema con 10 dimensiones personalizadas adicionales será más que suficiente e incluirá dimensiones personalizadas basadas en Segmentos o Etiquetas de programa. En el futuro, planificamos permitir a los clientes aumentar el número de Dimension personalizados permitidos.

## ¿Por qué no puedo reutilizar las ranuras de Dimension personalizados después de haberlas asignado? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Una vez que se ha asignado una ranura de Dimension personalizado determinada, volver a asignarla causaría que los datos anteriores produjeran un error al combinarse con un nuevo significado. Debido a ello, es posible que las ranuras de Dimension personalizadas no se vuelvan a utilizar. Este comportamiento es coherente con el de otras herramientas de análisis de métricas, como los Google Analytics.

## ¿Las perspectivas de correo electrónico admiten los correos electrónicos de Insight de ventas de Marketo? {#does-email-insights-support-marketo-sales-insight-emails}

Sí. Todos los correos electrónicos enviados a través de Marketo Sales Insights se incluyen en Email Insights.

## ¿Admite las perspectivas de correo electrónico los correos electrónicos operativos? {#does-email-insights-support-operational-emails}

Sí. De forma predeterminada, los correos electrónicos operativos están ocultos de la vista y las consultas. Sin embargo, puede cambiar esta configuración en el panel Configuración personal .

## ¿Las perspectivas de correo electrónico capturan los pasos recurrentes programados o ejecutados de nuevo por el flujo de correo electrónico de la campaña inteligente? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sí y No. Con la versión inicial de Perspectivas de correo electrónico, todos los eventos de correo electrónico se capturan y se puede acceder a ellos desde cualquier campaña inteligente programada o que se vuelva a ejecutar de forma recurrente. Pero no podrá diferenciar entre las diferentes ejecuciones de esa campaña inteligente. En nuestra próxima versión vamos a añadir asistencia para capturar la información de ejecución de Smart Campaign para los eventos Open, Click y Unsubscribe con el fin de diferenciar.

## ¿Por qué muchas métricas muestran cero cuando filtro por tipo de dispositivo o sistema operativo del dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Con la excepción de Clic para tasa de apertura, aperturas, clics y cancelaciones de suscripción, todas las demás métricas admitidas son eventos de envío o proporciones derivadas de eventos de envío. Dado que Tipo de dispositivo y SO de dispositivo solo se aplican a las métricas de participación, simplemente no tenemos la información que mostrar. Por ejemplo, es una consulta indefinida pedir la tasa de entrega cuando se filtra por tipo de dispositivo = móvil, ya que Marketo no habría recibido ninguna métrica de participación para los eventos de envío y envío subyacentes. Estamos explorando maneras de aplicar el tipo de dispositivo y el sistema operativo del dispositivo a partir de las métricas de participación para las relaciones que comprenden tanto las métricas de participación como las de envío.

## ¿Qué hace Perspectivas de correo electrónico cuando determinados clientes de correo electrónico bloquean imágenes? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problema común del sector es que un número creciente de clientes de correo electrónico desactivan las imágenes de forma predeterminada. La carga de imágenes es la base de cómo se graban las aperturas. Es totalmente posible que un usuario reciba un correo electrónico con imágenes bloqueadas, pero con el texto y los vínculos totalmente legibles. Si un usuario lo experimenta y hace clic en un vínculo de ese correo electrónico, se produce un escenario de un evento de clic, pero no un evento de apertura correspondiente para dicho correo electrónico. Las perspectivas de correo electrónico de Marketo generarán automáticamente cualquier evento que faltara. La lógica es idéntica a la de Marketo para el informe Rendimiento del correo electrónico , así como para el área Análisis del correo electrónico en el Explorador de ingresos.
