---
unique-page-id: 2949160
description: 'Integración con Adobe Analytics: Documentos de Marketo: documentación del producto'
title: Integración con Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---

# Integración con Adobe Analytics {#integrate-with-adobe-analytics}

## Introducción {#intro}

Analice el análisis web desde la perspectiva B2B consultando los datos de organización, sector y campaña [!DNL Marketo Real-Time Personalization] (RTP) en su cuenta de Adobe Analytics.

Este documento habilita la integración entre [!DNL Marketo Real-Time Personalization] (RTP) y Adobe Adobe Analytics. Los datos de RTP le permitirán detectar y analizar las tendencias en todos los segmentos del sector y organizaciones que visiten su sitio, así como medir la eficacia de sus campañas de RTP, proporcionando perspectivas y análisis para obtener resultados óptimos.

Puede conseguirlo si observa métricas como la cantidad de visitantes nuevos en comparación con los que regresan en cada segmento, analiza las tasas de clics en las campañas y descubre en qué industrias y segmentos personalizados y campañas en tiempo real generaron los posibles clientes con mejor conversión. Aproveche esta capacidad para obtener el máximo beneficio de su cuenta de RTP.

## RTP AUDIENCE ANALYTICS {#rtp-audience-analytics}

Con la integración RTP - AA, tiene una nueva dimensión dentro de la interfaz de análisis web. RTP mejora automáticamente sus paneles de análisis web con:

1. Datos de la organización e industria
1. Segmentos RTP personalizados
1. Listas de cuentas con nombre (Account-Based Marketing)

Esto mejora los datos B2B y le permite centrarse en los visitantes relevantes optimizando lo siguiente:

1. Canales de salida
1. Contenido
1. Resegmentación

## Informe de canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

El panel de RTP le ayuda a comprender el desglose de sus visitantes según los segmentos verticales y RTP. Puede ver el rendimiento de su visitante según el sector y las diferentes campañas de marketing (de pago, orgánicas y sociales) relacionadas con ese sector. El tablero también proporciona información general de alto nivel sobre qué secciones del sitio están viendo los visitantes según el tipo de sector.

## Informe de comportamiento {#behavioral-report}

En Adobe Analytics se pueden crear diferentes informes de comportamiento basados en los datos de organización, sector y segmento RTP. Estos informes de flujo visualizan la ruta que los visitantes siguen de una página o evento a otro. Este informe puede ayudarle a descubrir qué contenido mantiene a los visitantes comprometidos con el sitio.

## Rendimiento de RTP {#rtp-performance}

Vea las impresiones y conversiones de campañas RTP en Vínculos personalizados en Adobe Analytics.

Este informe de vínculo personalizado muestra las impresiones y conversiones de las campañas con el siguiente formato de nombre:

* Segmento ISegment de impresión: [Nombre de segmento RTP], ICampaign: [Nombre de campaña RTP]
* Segmento de conversión ISegment: [Nombre de segmento RTP], ICampaign: [Nombre de campaña RTP]

![](assets/custom-links-report.png)

## Configuración en Adobe Analytics {#set-up-in-adobe-analytics}

La integración utiliza la API de JavaScript que ofrece Adobe Analytics. En la integración se utilizan variables de conversión personalizadas (eVar), eventos personalizados (evento) y variables de tráfico. Todos deben habilitarse desde un administrador de AA. Debe establecer las variables de conversión, los eventos personalizados y las variables de tráfico en . De lo contrario, no podrá ver los datos en el grupo aunque los haya habilitado en RTP.

Complete los siguientes pasos para configurar estas variables en AA:

1. Vaya a **[!UICONTROL Herramientas de administración]** en su cuenta de AA.
1. Seleccione el **[!UICONTROL grupo de informes]** que se usará con la integración.
1. En **[!UICONTROL Editar configuración]**, vaya a **[!UICONTROL Conversión]** y seleccione **[[!UICONTROL Variables de conversión]](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.
Seleccione el número [Variable de conversión](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) (se recomienda):

   1. Evar n.º 20 para conversiones personalizadas del sector
   1. Evar n.º 21 para conversiones personalizadas de organización

   >[!NOTE]
   >
   >Si se toman estos #, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP.

   1. Cambiar estado a _[!UICONTROL Habilitado_].

      1. Cambie el nombre a **Sector** y **Organización**. (Así es como aparecerá en el grupo de informes).

      1. Cambie el campo Caduca después de a **[!UICONTROL Visita]**.

1. En **[!UICONTROL Editar configuración]**, vaya a **[!UICONTROL Conversión]** y seleccione **[[!UICONTROL Eventos de éxito]](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Seleccione el número de evento de eventos de éxito personalizados (se recomienda):

      1. event20 para campañas RTP
      1. event21 para segmentos RTP

      >[!NOTE]
      >
      >Si se toman estos #, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP.

      1. Cambie los nombres de los dos eventos a **Campañas RTP** y **Segmentos RTP**. Este es el nombre que aparecerá en el grupo de informes.

   1. Seleccione el campo Tipo que se **Contador (sin subrelaciones)**

1. En **[!UICONTROL Editar configuración]**, vaya a **[Tráfico](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** y seleccione **[Variables de tráfico](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Seleccione la variable de tráfico Nº de propiedad (se recomienda):

      1. Propiedad n.º 20 - Nombre: RTP Segment Organization
      1. N.º de propiedad 21 - Nombre: RTP Segment Industry
      1. Propiedad n.º 25 - Nombre: Campaign Organization
      1. Propiedad n.º 26 - Nombre: RTP Campaign Industry

      >[!NOTE]
      >
      >Si se toman estos #, seleccione otro número disponible. Alinee este número con el número de ranura en Configuración de cuenta RTP)

      1. Cambie los 4 nombres de propiedades. Este es el nombre que aparecerá en el grupo de informes.

   1. Seleccione el campo [!UICONTROL Habilitado] para **[!UICONTROL Habilitado]**.

   1. Seleccione el campo [!UICONTROL Informes de ruta] para **[!UICONTROL Habilitado]**.

## Configurado en [!DNL Marketo Real-Time Personalization] (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. En la plataforma RTP, vaya a **[!UICONTROL Configuración de la cuenta]**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. En **[!UICONTROL Configuración de la cuenta]**, haga clic en **[!UICONTROL Dominio]**.
1. En **[!UICONTROL Analytics]**, haga clic en **Adobe Analytics**.
1. Activa **[!UICONTROL 1} las opciones de Conversión, Personalizado y Tráfico.]**
1. Asigne las variables de conversión, evento y tráfico **números de ranura** para que coincidan con los números de ranura creados en AA
1. Haga clic en **[!UICONTROL Guardar]**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nuestros ajustes de ranura recomendados son
>
>**Variables de conversión**
>
>* [!UICONTROL Conversiones personalizadas del sector] - Ranura 20
>* [!UICONTROL Conversiones personalizadas de organización] - Ranura 21
>
>**Eventos personalizados**
>
>* [!UICONTROL Evento personalizado de campaña] - Ranura 20
>* [!UICONTROL Evento personalizado de segmento] - Ranura 21
>
>**Variables de tráfico**
>
>* [!UICONTROL Variable de tráfico de organización de segmentos] - Ranura 20
>* [!UICONTROL Variable de tráfico del sector de segmentos] - Ranura 21
>* [!UICONTROL Variable de tráfico de organización de campaña] - Ranura 22
>* [!UICONTROL Variable de tráfico de la industria de campaña] - Ranura 23
>
>**Asegúrese de que estos números de ranura se alinean con los números de variables y eventos creados en AA.**

## Informes {#reports}

Cree informes mejorados de Adobe Analytics del sitio según los nombres de las organizaciones, los sectores y los segmentos de RTP y los datos de las campañas en tiempo real.

Algunos ejemplos de informes y paneles personalizados en AA son:

* Rendimiento por sector o segmento definido (listas con nombre basadas en cuentas)
* Desglose del sector por rendimiento de KPI
* Páginas visitadas por organización
* Rendimiento del canal de marketing según la organización, el sector y los segmentos

**- Ejemplos de informes -**

**Informe de industrias principales**

![](assets/top-industries-report.png)

**Informe de organizaciones**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Creando el tablero RTP**

Cree un [nuevo panel](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), llamado **panel RTP**. Este tablero le ayudará a comprender el desglose de sus visitantes según los segmentos verticales y RTP.

1. Haga clic en **[!UICONTROL Tablero],** haga clic en **[!UICONTROL Agregar tablero]**.

1. Asigne un nombre al tablero **RTP Dashboard**.

1. Seleccione el **tamaño del tablero** 3 x 2, 2 x 2.

1. Cree el [informe breve](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) y agregue [contenido al tablero](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Agregar el informe breve de industrias al panel

1. Vaya a **[!UICONTROL Conversiones personalizadas]** y haga clic en **[!UICONTROL Sector]**.

1. Configurar gráfico en **gráfico circular**.

1. Haz clic en **[!UICONTROL Tablero]** y agrega **[!UICONTROL Informe breve]**.

1. Asigne un nombre al informe **Industrias principales**.

1. Colocar en el tablero **RTP Dashboard**.

1. Crear **Nuevo**.

Adición del informe breve de segmentos al panel

1. Vaya a **[!UICONTROL Métricas del sitio]**. Haz clic en **[!UICONTROL Eventos personalizados]**, **[!UICONTROL Segmentos]**.

1. Configurar gráfico en **barra vertical**.

1. Haz clic en **[!UICONTROL Tablero]** y agrega **[!UICONTROL Informe breve]**.

1. Asigne un nombre al informe **Segmentos principales**.

1. Colocar en el tablero **RTP Dashboard**.

1. Crear **Nuevo**.

Los informes breves se mostrarán en el tablero.

## Ver impresiones y clics (conversiones) en Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Haga clic en **[!UICONTROL Vínculos personalizados]**.

   ![](assets/sitecatalyst1-1.png)

1. Busque Impresiones para ver los nombres de segmentos y campañas que representan el número de impresiones de la campaña.
   ![](assets/sitecatalyst1.png)

1. Busque Conversión para ver los nombres de segmentos y campañas que representan el número de clics de la campaña.

   ![](assets/sitecatalyst2.png)
