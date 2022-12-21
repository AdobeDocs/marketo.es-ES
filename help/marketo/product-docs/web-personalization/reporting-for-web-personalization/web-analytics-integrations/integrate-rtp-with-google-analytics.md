---
unique-page-id: 2949158
description: Integración de RTP con Google Analytics - Marketo Docs - Documentación del producto
title: Integrar RTP con Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Integrar RTP con Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics es ahora el estándar operativo y todas las propiedades de Google se han actualizado a Universal Analytics.
>
>Este artículo muestra cómo usar el antiguo Google Standard Analytics, pero le recomendamos que cambie a Universal Analytics.
>
>Si todavía no utiliza la variable [código de seguimiento de analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google recomienda encarecidamente volver a etiquetar el sitio para utilizarlo. Google está en desuso lo siguiente:
>
>* ga.js
>* urchin.js
>* Fragmentos WAP/del lado del servidor
>* YT/MO
>* Variables personalizadas
>* Variables definidas por el usuario
>
>Consulte cómo integrar [Personalización web con Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introducción {#introduction}

Analice el análisis web desde un nuevo ángulo utilizando el flujo de datos directo desde la personalización en tiempo real de Marketo (RTP) a su cuenta de Google Analytics (GA). Mida sus visitas web en GA según organizaciones, industrias y campañas RTP. Vea métricas como los tipos de industrias o segmentos de RTP en GA y cómo funcionan y generan posibles clientes según diferentes fuentes de tráfico (social, de pago, orgánico), analizando las tasas de clics en las campañas y midiendo el impacto que las campañas de personalización tienen en su sitio web. Aproveche esta capacidad para obtener el máximo beneficio de su cuenta RTP

**Audience Analytics RTP**

Con la integración, tiene una nueva dimensión en su cuenta de GA. RTP mejora automáticamente sus paneles con:

1. Organizaciones e industrias
1. Segmentos personalizados en RTP
1. Listas de Account-Based Marketing

Céntrese en sus perspectivas clave de B2B. Analice los canales según las industrias y los segmentos a los que se dirijan.

## Informe de canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

El panel RTP B2B le ayuda a comprender el desglose de sus visitantes según las verticales y la segmentación RTP. Puede ver el rendimiento del visitante según el sector financiero y según diferentes campañas de marketing (de pago, orgánicas, sociales). El tablero también proporciona información general de alto nivel sobre el rendimiento de los segmentos de RTP y se explora para mostrar las principales organizaciones que visitan el sitio.

## Flujo de comportamiento {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

El informe Flujo de comportamiento (ver imagen) visualiza la ruta que los visitantes recorren de una página o evento al siguiente. El ejemplo de imagen muestra la ruta de todos los visitantes del sector financiero. Este informe puede ayudarle a descubrir qué contenido mantiene a los visitantes involucrados con el sitio.

## Rendimiento de RTP {#rtp-performance}

Mida sus campañas RTP y correlaciónelas con el promedio general del sitio. Conozca cómo afectan estas campañas a las métricas de su sitio web y utilice estos datos para centrar sus esfuerzos de personalización en los objetivos adecuados. Genere informes personalizados para comprender mejor el rendimiento de sus campañas de personalización.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configuración de RTP con Google Analytics {#setting-up-rtp-with-google-analytics}

1. Añada el correo electrónico rtp.ga2@gmail.com como usuario de lectura y análisis a su cuenta de GA. Para obtener más información, consulte [here](https://support.google.com/analytics/answer/2884495?hl=en).

1. En su cuenta RTP. Vaya a **Configuración de la cuenta**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. En **Configuración de la cuenta**, **Dominio** y **Analytics**.

1. Haga clic en **Google Analytics**.

1. Active el **Variables personalizadas** y **Eventos** para anexar estos datos de RTP a los Google Analytics.

1. Introduzca la variable **Ranura** número para enviar datos de variables personalizadas (el valor predeterminado es 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Haga clic en **Guardar**.

>[!NOTE]
>
>Para enviar datos de segmentos a GA, en la sección [Página Editar segmento](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) en la plataforma RTP, seleccione la casilla de verificación **Enviar un evento a los Google Analytics en la coincidencia de segmentos**.

## Configuración de informes de Google Analytics con datos RTP {#setting-up-google-analytics-reports-with-rtp-data}

En los Google Analytics, puede utilizar los paneles, la segmentación GA y los informes para ver sus datos RTP:

* [Tableros](https://support.google.com/analytics/answer/1068216?hl=en) proporciona información general sobre el rendimiento del sitio web.
* Un segmento GA está diseñado para filtrar visitantes en la interfaz de GA y ver el tráfico por segmento. Consulte cómo crear un segmento [here](https://support.google.com/analytics/answer/3124493?hl=en).
* Creación [informes personalizados](https://support.google.com/analytics/answer/1033013?hl=en) para ver o configurar correos electrónicos programados. Consulte en Personalización > Nuevo informe personalizado .
