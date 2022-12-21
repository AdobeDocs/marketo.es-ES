---
unique-page-id: 2949160
description: 'Integración con Adobe Analytics: Marketo Docs: Documentación del producto'
title: Integración con Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Integración con Adobe Analytics {#integrate-with-adobe-analytics}

## Introducción {#intro}

Analice el análisis web desde una perspectiva B2B mediante la visualización de datos de campaña de personalización en tiempo real (RTP) de la organización, el sector y Marketo en su cuenta de Adobe Analytics.

Este documento permite la integración entre Marketo Real-Time Personalization (RTP) y Adobe Adobe Analytics. Los datos de RTP le permitirán detectar y analizar las tendencias en todos los segmentos y organizaciones del sector que visiten su sitio y medir la eficacia de sus campañas de RTP, proporcionando perspectivas y análisis para obtener resultados óptimos.

Para lograrlo, fíjese en métricas como el número de visitantes nuevos frente a los que regresan en cada segmento, analice las tasas de clics en las campañas y descubra qué industrias, segmentos personalizados y campañas en tiempo real generaron los mejores posibles clientes de conversión. Aproveche esta capacidad para obtener el máximo beneficio de su cuenta RTP.

## Audience Analytics RTP {#rtp-audience-analytics}

Con la integración RTP - AA, tiene una nueva dimensión dentro de la interfaz de análisis web. RTP mejora automáticamente sus paneles de análisis web con:

1. Datos de organización e industria
1. Segmentos RTP personalizados
1. Listas de cuentas con nombre (Account-Based Marketing)

Esto mejora los datos B2B y le permite centrarse en los visitantes relevantes optimizando:

1. Canales de salida
1. Contenido
1. Redireccionamiento

## Informe de canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

El tablero RTP le ayuda a comprender el desglose de sus visitantes según los segmentos verticales y RTP. Puede ver el rendimiento del visitante según el sector y las diferentes campañas de marketing (de pago, orgánicas y sociales) relacionadas con ese sector. El tablero también proporciona información general de alto nivel sobre las secciones del sitio que ven los visitantes según el tipo de sector.

## Informe de comportamiento {#behavioral-report}

En Adobe Analytics se pueden crear distintos informes de comportamiento basados en datos de segmentos de organización, industria y RTP. Estos informes de flujo visualizan la ruta que los visitantes siguen de una página o evento a otra. Este informe puede ayudarle a descubrir qué contenido mantiene a los visitantes involucrados con el sitio.

## Rendimiento de RTP {#rtp-performance}

Vea impresiones y conversiones de campaña RTP en Vínculos personalizados en Adobe Analytics.

Este informe Vínculo personalizado mostrará impresiones y conversiones de campañas con el siguiente formato de asignación de nombres:

* ISegment de impresión: [Nombre de segmento RTP], ICampaign: [Nombre de campaña de RTP]
* ISegment de conversión: [Nombre de segmento RTP], ICampaign: [Nombre de campaña de RTP]

![](assets/custom-links-report.png)

## Configuración en Adobe Analytics {#set-up-in-adobe-analytics}

La integración utiliza la API de JavaScript que ofrece Adobe Analytics. En la integración se usan variables de conversión personalizadas (eVar), eventos personalizados (evento) y variables de tráfico. Todos deben habilitarse desde un administrador AA. Debe configurar las variables de conversión, los eventos personalizados y las variables de tráfico en AA o no podrá ver los datos en el grupo aunque los haya activado en RTP.

Complete los siguientes pasos para configurar estas variables en AA:

1. Vaya a **Herramientas de administración** en su cuenta AA.
1. Seleccione el **Grupo de informes** para usar con la integración.
1. En **Editar configuración**, vaya a **Conversión** y seleccione **[Variables de conversión](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Seleccione el [Variable de conversión](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) número (se recomienda):

   1. Evar # 20 para conversiones personalizadas del sector
   1. Evar n.º 21 para conversiones personalizadas de organización

   >[!NOTE]
   >
   >Si estos # se toman, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP.

   1. Cambiar estado a _Habilitado_.

      1. Cambiar nombre a **Industria** y **Organización**. (Así es como aparecerá en el grupo de informes).

      1. Cambiar el campo Caduca después de a **Visita**.


1. En **Editar configuración** vaya a **Conversión** y seleccione **[Eventos de éxito](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Seleccione el número de Evento de éxito personalizado (se recomienda):

      1. event20 para campañas RTP
      1. event21 para segmentos RTP

      >[!NOTE]
      >
      >Si estos # se toman, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP.

      1. Cambie los nombres de los dos eventos a **Campañas RTP** y **Segmentos RTP**. Este es el nombre que aparecerá en el grupo de informes.
   1. Seleccione el campo Type que desea **Contador (sin subrelaciones)**



1. En **Editar configuración** vaya a **[Tráfico](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** y seleccione **[Variables de tráfico](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Seleccione el número de propiedad de la variable de tráfico (se recomienda):

      1. Propiedad # 20 - Nombre: Organización de segmentos RTP
      1. Propiedad nº 21 - Nombre: Industria de segmentos RTP
      1. Propiedad nº 25 - Nombre: Organización de campañas
      1. Propiedad nº 26 - Nombre: Industria de campaña RTP

      >[!NOTE]
      >
      >Si estos # se toman, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP)

      1. Cambie los 4 nombres de propiedad. Este es el nombre que aparecerá en el grupo de informes.
   1. Seleccione Enabled field para **Habilitado**.

   1. Seleccione el campo Informes de ruta para **Habilitado**.



## Configuración en Marketo Real-Time Personalization (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. En la plataforma RTP, vaya a **Configuración de la cuenta**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **Configuración de la cuenta**, haga clic en **Dominio**.
1. En **Analytics, haga clic en** **Adobe Analytics**.
1. Turn **Activado** las variables Conversión, Personalizado y Tráfico alternan.
1. Asignar las variables de conversión, evento y tráfico **números de ranura** para coincidir con los números de ranura creados en AA
1. Haga clic en **Guardar**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nuestra configuración de ranura recomendada es
>
>**Variables de conversión**
>
>* Conversiones personalizadas del sector: ranura 20
>* Conversiones personalizadas de organización - Ranura 21
>
>**Eventos personalizados**
>
>* Evento personalizado de campaña - Ranura 20
>* Evento personalizado de segmento - Ranura 21
>
>**Variables de tráfico**
>
>* Variable de tráfico de la organización de segmentos - Ranura 20
>* Variable de tráfico del sector de segmentos: ranura 21
>* Variable de tráfico de la organización de la campaña - Ranura 22
>* Variable de tráfico del sector de la campaña - Ranura 23
>
>**Asegúrese de que estos números de ranura coinciden con los números de variables y eventos creados en AA.**

## Informes {#reports}

Cree informes mejorados de SiteAdobe Analytics según los nombres de organización, industrias y segmentos RTP, así como datos de campañas en tiempo real.

Algunos ejemplos de informes y tableros personalizados de AA son:

* Rendimiento por sector o segmento definido (listas con nombres basados en cuentas)
* Desglose por sector por rendimiento de KPI
* Páginas vistas por organización
* Rendimiento del canal de marketing según organización, sector, segmentos

**-Ejemplos de informes-**

**Informe de principales sectores**

![](assets/top-industries-report.png)

**Informe de organizaciones**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Creación del panel RTP**

Cree un [nuevo panel](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), llamado **Tablero RTP**. Este tablero le ayudará a comprender el desglose de sus visitantes según los segmentos verticales y RTP.

1. Haga clic en **Tablero,** click **Agregar tablero**.

1. Asigne un nombre al tablero **Tablero RTP**.

1. Seleccione el **tamaño del tablero** 3 x 2, 2 x 2.

1. Cree la variable [informe breve](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) y agregue [contenido al tablero](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Adición del informe breve de industrias al tablero

1. Vaya a **Conversiones personalizadas**, haga clic en **Industria**.

1. Configurar gráfico para **Gráfico circular**.

1. Haga clic en **Panel**, agregue **Informe breve**.

1. Asigne un nombre al informe **Principales sectores**.

1. Colocar en el panel **Tablero RTP**.

1. Crear **Nuevo**.

Adición del informe breve Segmentos al tablero

1. Vaya a **Métricas del sitio**. Haga clic en **Eventos personalizados**, **Segmentos**.

1. Configurar gráfico para **Barra vertical**.

1. Haga clic en **Panel**, agregue **Informe breve**.

1. Asigne un nombre al informe **Segmentos principales**.

1. Colocar en el panel **Tablero RTP**.

1. Crear **Nuevo**.

Los informes breves se mostrarán en el tablero.

## Ver impresiones y clics (conversiones) en Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Haga clic en **Vínculos personalizados**.

   ![](assets/sitecatalyst1-1.png)

1. Busque Impresiones para ver los nombres de Segmento y Campaña que representan el número de impresiones de la campaña.\
   ![](assets/sitecatalyst1.png)

1. Busque Conversión para ver los nombres de segmentos y campañas que representan el número de clics de la campaña.

   ![](assets/sitecatalyst2.png)
