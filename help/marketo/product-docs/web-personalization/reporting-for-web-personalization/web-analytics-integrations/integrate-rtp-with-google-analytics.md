---
unique-page-id: 2949158
description: 'Integración de RTP con Google Analytics: documentos de marketing: documentación del producto'
title: Integrar RTP con Google Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---


# Integrar RTP con Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics es ahora el estándar operativo y todas las propiedades de Google se han actualizado a Universal Analytics.
>
>En este artículo se muestra cómo usar el antiguo Google Standard Analytics, pero se recomienda cambiar a Universal Analytics.
>
>Si todavía no utiliza el código de seguimiento [analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google recomienda enfáticamente que vuelva a etiquetar el sitio para utilizarlo. Google está dejando de utilizar lo siguiente:
>
>* ga.js
>* urchin.js
>* Fragmentos WAP/del lado del servidor
>* YT / MO
>* Variables personalizadas
>* Variables definidas por el usuario

>
>
Consulte cómo integrar la [Personalización web con Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introducción {#introduction}

Analice el análisis de Web desde un nuevo ángulo utilizando el flujo de datos directo desde la personalización en tiempo real (RTP) de Marketing a su cuenta de Google Analytics (GA). Mida sus visitas web en GA según organizaciones, industrias y campañas RTP. Métricas de vista como los tipos de industrias o segmentos de RTP en GA y cómo funcionan y generan posibles clientes según las distintas fuentes de tráfico (social, pagada, orgánica), analizando las tasas de pulsaciones en las campañas y midiendo el impacto que las campañas de personalización tienen en el sitio web. Aproveche esta capacidad para obtener el máximo beneficio de su cuenta RTP

**Audience Analytics RTP**

Con la integración, tiene una nueva dimensión en su cuenta de GA. RTP mejora automáticamente sus paneles con:

1. Organizaciones e industrias
1. Segmentos personalizados en RTP
1. Listas de mercadotecnia basadas en cuentas

Céntrese en sus clientes potenciales B2B clave. Analizar canales según sectores y segmentos específicos.

## Informe canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

El Panel RTP B2B le ayuda a comprender el desglose de sus visitantes según la segmentación vertical y RTP. Puede ver el rendimiento del visitante según el sector financiero y según las distintas campañas de marketing (pago, orgánico, social). El panel también proporciona información general de alto nivel sobre el rendimiento de los segmentos de RTP y se explora para mostrar las organizaciones principales que visitan el sitio.

## Flujo de comportamiento {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

El informe Flujo de comportamiento (ver imagen) visualiza los visitantes de ruta que se desplazan de una página o Evento al siguiente. El ejemplo de imagen muestra la ruta de todos los visitantes del sector financiero. Este informe puede ayudarle a descubrir qué contenido mantiene a los visitantes comprometidos con el sitio.

## Rendimiento de RTP {#rtp-performance}

Mida sus campañas RTP y correlaciónelas con el promedio general del sitio. Conozca cómo estas campañas afectan las métricas del sitio web y utilice estos datos para centrar sus esfuerzos de personalización en los destinatarios correctos. Genere informes personalizados para comprender mejor el rendimiento de sus campañas de personalización.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configuración de RTP con Google Analytics {#setting-up-rtp-with-google-analytics}

1. Añada el correo electrónico rtp.ga2@gmail.com como usuario de lectura y análisis a su cuenta de GA. Para obtener más información, consulte [aquí](https://support.google.com/analytics/answer/2884495?hl=en).

1. En su cuenta RTP. Vaya a **Configuración de la cuenta**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. En **Configuración de cuenta**, **Dominio** y **Análisis**.

1. Haga clic en **Google Analytics**.

1. Active las **variables personalizadas** y **Eventos** relevantes para anexar estos datos de RTP a Google Analytics.

1. Introduzca el número **Ranura** para enviar datos de variables personalizadas (el valor predeterminado es 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Haga clic en **Guardar**.

>[!NOTE]
>
>Para enviar datos de segmentos a GA, en la [página Editar segmento](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) de la plataforma RTP, seleccione la casilla **Enviar Evento a Google Analytics en coincidencia de segmento**.

## Configuración de informes de Google Analytics con datos RTP {#setting-up-google-analytics-reports-with-rtp-data}

En Google Analytics puede utilizar paneles, segmentación de GA y sistemas de informes para vista de los datos de RTP:

* [Los ](https://support.google.com/analytics/answer/1068216?hl=en) tableros proporcionan información general sobre el rendimiento del sitio web.
* Un segmento GA está diseñado para filtrar visitantes en la interfaz GA y para vista del tráfico por segmento. Vea cómo generar un segmento [aquí](https://support.google.com/analytics/answer/3124493?hl=en).
* Creación de [informes personalizados](https://support.google.com/analytics/answer/1033013?hl=en) para la vista y/o configuración de correos electrónicos programados. Consulte en Personalización > Nuevo informe personalizado.
