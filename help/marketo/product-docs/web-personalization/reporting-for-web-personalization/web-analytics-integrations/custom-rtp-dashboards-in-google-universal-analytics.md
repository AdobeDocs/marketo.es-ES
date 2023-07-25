---
unique-page-id: 7504238
description: Paneles RTP personalizados en Google Universal Analytics - Documentos de Marketo - Documentación del producto
title: Paneles RTP personalizados en Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Paneles RTP personalizados en Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integración de RTP con Universal Analytics de Google](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

En esta publicación se explica cómo configurar paneles RTP en Google Universal Analytics (GUA). Los datos enviados desde RTP a GUA pueden configurarse como dos paneles personalizados independientes llamados:

* RTP B2B
* Compromiso RTP

## Configuración de un tablero personalizado {#setting-up-a-custom-dashboard}

1. Inicie sesión en Google Analytics. Haga clic en **Informes** en el menú superior. Clic **Paneles** y **+Nuevo tablero personalizado**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Seleccionar **Lienzo en blanco**, añada un **Nombre de panel** y haga clic en **Crear tablero**.

1. Clic **Añadir widget** para crear un widget nuevo.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Panel RTP B2B {#rtp-b-b-dashboard}

Este tablero permite a los usuarios analizar el rendimiento de su sitio web desde una perspectiva B2B.

Proporciona información como el origen de la visita y el comportamiento en el sitio por sector, ingresos, tamaño, listas basadas en cuentas y segmentos de destino.

El tablero consta de 3 columnas

* Fuente de tráfico
* Segmentación
* Profundización firmográfica

1. Cree un nuevo tablero llamado **Panel RTP B2B** y defina los siguientes widgets:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Columna 1: Fuentes de tráfico
    </div></th> 
   <th> 
    <div> <strong>Columna 2: Segmentación</strong> 
    </div></th> 
   <th> 
    <div> <strong>Columna 3 - Profundización en el plano Firmográfico</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: Sesiones por segmentos y canales</li> 
     <li>Tipo de widget: Barra<br></li> 
     <li>Crear un gráfico de barras que muestre: Sesión</li> 
     <li>Agrupado por: etiqueta de evento</li> 
     <li>Pivot by: agrupación de canales predeterminada</li> 
     <li>Filtro: <br>Mostrar solo | Categoría de evento (contenedor) RTP-Segmentos</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: N.º de usuarios segmentados RTP</li> 
     <li>Tipo: Métrica 2.1</li> 
     <li>Mostrar la siguiente métrica: Usuarios<br></li> 
     <li>Filtro: <br>Mostrar solo | Categoría de evento (contenedor) RTP-Segmentos</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: Sesiones por sector</li> 
     <li>Tipo: Circular<br></li> 
     <li>Crear un gráfico circular que muestre: Sesiones</li> 
     <li>Agrupadas por: RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por sector y canales</strong></li> 
     <li><strong>Tipo de widget: Barra</strong></li> 
     <li><strong>Crear un gráfico de barras que muestre: Sesión</strong></li> 
     <li><strong>Agrupadas por: RTP-Industry</strong></li> 
     <li><strong>Pivot by: agrupación de canales predeterminada</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones segmentadas por país</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Trazar métrica seleccionada: País | Sesiones</strong></li> 
     <li><strong>Selecciona una región: El mundo</strong></li> 
     <li><strong>Filtro: Mostrar solo | Categoría de evento (contenedor) RTP-Segmentos</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por Categoría RTP</strong></li> 
     <li><strong>Tipo: Circular</strong></li> 
     <li><strong>Crear un gráfico circular que muestre: Sesiones</strong></li> 
     <li><strong>Agrupado por: RTP-Category</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Segmentos de destinatario principales</li> 
     <li>Tipo: barra</li> 
     <li>Crear un gráfico de barras que muestre: Usuarios</li> 
     <li>Agrupado por: Acción de evento</li> 
     <li>Filtro: Mostrar solo | Categoría de evento (contenedor) RTP-Segmentos</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones por grupos RTP</li> 
     <li>Tipo: barra<br></li> 
     <li>Crear un gráfico de barras que muestre: Sesiones</li> 
     <li>Agrupado por: RTP-Group</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones y objetivos por segmentos principales</li> 
     <li>Tipo: Tabla<br></li> 
     <li>Mostrar las columnas siguientes: <br>Etiqueta de evento | Sesiones | Tasa de conversión de objetivos</li> 
     <li>Filtro: <br>Mostrar solo | Categoría de evento (contenedor) RTP-Segmentos</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Tablero de participación de RTP {#rtp-engagement-dashboard}

Este tablero permite a los usuarios analizar el rendimiento de sus campañas RTP y las participaciones en el motor de recomendaciones. Proporciona una comparación de los promedios. duración de la sesión y páginas por sesión entre:

* Descomprometido
* Participación (impresiones y clics en una campaña personalizada)
* Clics en el motor de recomendaciones y el contenido principal recomendado

Cree un nuevo tablero llamado **Tablero de participación de RTP** y defina los siguientes widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Exposición de campañas en la columna 1</strong> 
    </div></th> 
   <th> 
    <div> <strong>Clic en campañas de la columna 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Columna 3 Motor de recomendaciones</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Total de CTA (participación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[only show] Categoría del evento (contiene): RTP-Campaigns</strong><br><strong>[only show] Acción de evento (exactamente igual): impresión</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Total de CTA (clic)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[only show] Categoría del evento (contiene): RTP-Campaigns</strong><br><strong>[only show] Acción de evento (exactamente igual): clics</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>CRE: clics totales</strong></li> 
     <li>Tipo: <strong>2.1 Métrica</strong><br></li> 
     <li>Mostrar la siguiente métrica: <strong>Pageviews</strong></li> 
     <li>Filtro: <strong>[sólo mostrar] Página (que contiene): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>El Promedio de Duración de la sesión (participación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>El Promedio de Duración de sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría del evento (exactamente igual): RTP-Campaigns</strong><br><strong>[only show] Acción de evento (exactamente igual): impresión</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>El Promedio de Duración de la sesión (clic)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>El Promedio de Duración de sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría del evento (exactamente igual): RTP-Campaigns</strong><br><strong>[only show] Acción de evento (exactamente igual): clics</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>CRE: Contenido recomendado principal</strong></li> 
     <li>Tipo: <strong>Tabla</strong><br></li> 
     <li>Mostrar las columnas siguientes: <br><strong>Título de página | Vistas de página</strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[sólo mostrar] Página (que contiene): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas/sesión (participación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Páginas/sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría del evento (exactamente igual): RTP-Campaigns</strong></li> 
     <li><strong>[only show] Acción de evento (exactamente igual): impresión</strong></li> 
     <li><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas/sesión (clic)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Páginas/sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría del evento (exactamente igual): RTP-Campaigns</strong></li> 
     <li><strong>[only show] Acción de evento (exactamente igual): clics</strong></li> 
     <li><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Impresiones por CTA</strong></li> 
     <li>Tipo: <strong>Tabla</strong></li> 
     <li>Mostrar las columnas siguientes: <strong>Etiqueta de evento | Total de eventos | Usuarios</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría del evento (exactamente igual): RTP-Campaigns</strong><br><strong>[only show] Acción de evento (exactamente igual): impresión</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Clickthrough de CTA</strong></li> 
     <li>Tipo: <strong>Tabla</strong></li> 
     <li>Mostrar las columnas siguientes: <strong>Etiqueta de evento | Total de eventos | Usuarios</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría del evento (exactamente igual): RTP-Campaigns</strong><br><strong>[only show] Acción de evento (exactamente igual): clics</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integración de RTP con Universal Analytics de Google](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Informes RTP personalizados en Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
