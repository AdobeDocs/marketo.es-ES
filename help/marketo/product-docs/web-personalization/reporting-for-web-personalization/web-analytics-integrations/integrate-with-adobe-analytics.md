---
unique-page-id: 2949160
description: 'Integración con Adobe Analytics: documentos de marketing: documentación del producto'
title: Integración con Adobe Analytics
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Integración con Adobe Analytics {#integrate-with-adobe-analytics}

## Intro {#intro}

Analice el análisis de Web desde una perspectiva B2B mediante la visualización de datos de campaña de la organización, el sector y la personalización en tiempo real (RTP) de Marketing en su cuenta de Adobe Analytics.

Este documento permite la integración entre la Personalización en tiempo real (RTP) de Marketing y Adobe Analytics de Adobe. Los datos de RTP le permitirán detectar y analizar las tendencias en todos los segmentos y organizaciones del sector que visiten su sitio y medir la eficacia de sus campañas RTP, proporcionando las perspectivas y la análisis para obtener resultados óptimos.

Para lograrlo, observe las métricas, tales como los números de visitantes nuevos frente a los que regresan en cada segmento, analice las tasas de clics en las campañas y descubra qué industrias y segmentos personalizados y campañas en tiempo real generaron los mejores clientes potenciales de conversión. Aproveche esta capacidad para obtener el máximo beneficio de su cuenta RTP.

## Audience Analytics RTP {#rtp-audience-analytics}

Con la integración RTP - AA, tiene una nueva dimensión en la interfaz de análisis web. RTP mejora automáticamente sus paneles de análisis web con:

1. Datos de organización e industria
1. Segmentos RTP personalizados
1. Listas de cuenta con nombre (mercadotecnia basada en cuenta)

Esto mejora los datos B2B y le permite centrarse en visitantes relevantes optimizando:

1. Canales salientes
1. Contenido
1. Retargeting

## Informe canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

El panel RTP le ayuda a comprender el desglose de sus visitantes según los segmentos verticales y RTP. Puede ver el rendimiento del visitante según la industria y las diferentes campañas de marketing (pagas, orgánicas, sociales) relacionadas con esa industria. El panel también proporciona información general de alto nivel sobre las secciones del sitio que ven sus visitantes según el tipo de sector.

## Informe de comportamiento {#behavioral-report}

En Adobe Analytics se pueden crear diferentes informes de comportamiento basados en datos de segmentos de organización, industria y RTP. Estos informes de flujo visualizan los visitantes de ruta que se toman de una página o Evento al siguiente. Este informe puede ayudarle a descubrir qué contenido mantiene a los visitantes comprometidos con el sitio.

## Rendimiento de RTP {#rtp-performance}

Impresiones y conversiones de campaña RTP de vista en Vínculos personalizados en Adobe Analytics.

Este informe de vínculos personalizados mostrará las impresiones y conversiones de campañas con el siguiente formato de nomenclatura:

* ISegmento de impresión: [Nombre del segmento RTP], campaña IC: [Nombre de Campaña RTP]
* ISegmento de conversión: [Nombre del segmento RTP], campaña IC: [Nombre de Campaña RTP]

![](assets/custom-links-report.png)

## Configurar en Adobe Analytics {#set-up-in-adobe-analytics}

La integración utiliza la API de JavaScript que Adobe Analytics oferta. En la integración se utilizan variables de conversión personalizadas (eVar), eventos personalizados (evento) y variables de tráfico. Todos deben habilitarse desde el administrador de AA. Debe configurar las variables de conversión, los eventos personalizados y las variables de tráfico en AA o no podrá ver los datos en el grupo aunque los haya habilitado en RTP.

Complete los siguientes pasos para configurar estas variables en AA:

1. Vaya a **Herramientas de administración** en su cuenta de AA.
1. Seleccione el **grupo de informes** que se utilizará con la integración.
1. En **Editar configuración,** vaya a **Conversión** y seleccione ** [Variables de conversión](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Seleccione el número [Variable de conversión](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) (se recomienda):

   1. 

      1. Evar Nº 20 para conversiones personalizadas de la industria
      1. Evar Nº 21 para conversiones personalizadas de la organización

         >[!NOTE]
         >
         >Si se toman estos #, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP.

      1. Cambiar estado a* Habilitado*

         1. Cambie el nombre a **Industria** y **Organización**. (Así es como aparecerá en el grupo de informes).

         1. Cambiar el campo Caduca después de a **Visita.**

1. En **Editar configuración **vaya a** Conversión **y seleccione ** [Eventos de éxito](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

1. Seleccione el número de Evento de Eventos de éxito personalizados (se recomienda):

   1. evento20 para Campañas RTP
   1. evento21 para segmentos RTP

      >[!NOTE]
      >
      >Si se toman estos #, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP.

   1. Cambie los nombres de los dos eventos a **Campañas RTP** y **Segmentos RTP**. Es el nombre que aparecerá en el grupo de informes.

1. Seleccione el campo *Tipo* para que sea **Contador (sin subrelaciones)**

1. En **Editar configuración** vaya a ** [Tráfico](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable) **y seleccione ** [Variables de tráfico](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Seleccione el número de propiedad de la variable de tráfico (se recomienda):

      1. Propiedad Nº 20 - Nombre: Organización de segmentos RTP
      1. Propiedad Nº 21 - Nombre: Industria de segmentos RTP
      1. Propiedad Nº 25 - Nombre: Organización de campaña
      1. Propiedad Nº 26 - Nombre: Industria de Campaña RTP

         >[!NOTE]
         >
         >Si se toman estos #, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP)

      1. Cambie los nombres de las propiedades 4. Es el nombre que aparecerá en el grupo de informes.
   1. Seleccione el campo Habilitado para **Habilitado**
   1. Seleccione el campo Informes de ruta para **Habilitado**


## Configurar en Personalización en tiempo real (RTP) de Marketing a {#set-up-in-marketo-real-time-personalization-rtp}

1. En la plataforma RTP, vaya a **Configuración de cuenta**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **Configuración de cuenta**, haga clic en **Dominio**.
1. En **Analytics, haga clic en** **Adobe Analytics**.
1. Active **On **la variable de conversión, personalizada y tráfico cambia.
1. Asigne las variables de conversión, Evento y tráfico **números de ranura** para que coincidan con los números de ranura creados en AA
1. Haga clic en **GUARDAR**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nuestra configuración de ranura recomendada es
>
>**Variables de conversión**
>
>* Conversiones personalizadas de la industria - Ranura 20
>* Conversiones personalizadas de la organización - Ranura 21

>
>
**Eventos personalizados**
>
>* Evento personalizado de campaña - Ranura 20
>* Evento personalizado del segmento - Ranura 21

>
>
**Variables de tráfico**
>
>* Variable de tráfico de la organización de segmentos - Ranura 20
>* Variable de tráfico del sector de segmentos - Ranura 21
>* Variable de tráfico de la organización de campaña - Ranura 22
>* Variable de tráfico del sector de campaña - Ranura 23

>
>
**Asegúrese de que estos números de ranura se alinean con los números de variables y eventos creados en AA.**

## Informes {#reports}

Cree informes mejorados de SiteAdobe Analytics en función de los nombres de la organización, las industrias y los segmentos de RTP y los datos de campañas en tiempo real.

Algunos ejemplos de informes y paneles personalizados de AA son:

* Rendimiento por sector o segmento definido (listas con nombre basadas en cuenta)
* Desglose por sector por rendimiento KPI
* Páginas vistas por organización
* Rendimiento del canal de mercadotecnia según la organización, el sector y los segmentos

**Ejemplos de informes**

**Informe de industrias principales**

** ![](assets/top-industries-report.png)

**

**Informe de organizaciones**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Creación del Panel RTP**

Cree un [nuevo panel](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), denominado **Panel RTP**. Este panel le ayudará a comprender el desglose de sus visitantes según los segmentos verticales y RTP.

1. Haga clic en **Panel,** haga clic** Añadir Panel***

1. Asigne un nombre al Panel **Panel RTP**
1. Seleccione el **tamaño de panel** 3 x 2, 2 x 2
1. Cree el [informe breve](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) y agregue contenido [al panel](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)

Añadir el informe breve de industrias al Panel

1. Vaya a **Conversiones personalizadas**, haga clic en **Industria**

1. Configurar gráfico para **gráfico circular**
1. Haga clic en **Panel**, agregue **informe breve**

1. Asigne un nombre al informe **Principales industrias**
1. Colocar en Panel **Panel RTP**
1. Crear **Nuevo**.

Añadir el informe breve Segmentos al Panel

1. Vaya a **Métricas del sitio, **Haga clic en **Eventos personalizados, segmentos**

1. Configurar gráfico en **barra vertical**
1. Haga clic en **Panel**, agregue **informe breve**

1. Asigne un nombre al informe **Segmentos principales**
1. Colocar en Panel **Panel RTP**
1. Crear **Nuevo.**

Los informes breves se mostrarán en el panel.

## Clics e impresiones de vista (conversiones) en Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Haga clic en Vínculos personalizados.

   ![](assets/sitecatalyst1-1.png)

1. Busque impresiones en los nombres de segmentos de vista y Campañas que representen el número de impresiones de la campaña.\
   ![](assets/sitecatalyst1.png)

1. Busque los nombres de segmentos de vista y Campañas que representan el número de clics de la campaña.

   ![](assets/sitecatalyst2.png)

