---
unique-page-id: 7504238
description: Paneles RTP personalizados en Google Universal Analytics - Documentos de Marketo - Documentación del producto
title: Paneles RTP personalizados en Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Paneles RTP personalizados en Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

En esta publicación se explica cómo configurar paneles RTP en Google Universal Analytics (GUA). Los datos enviados desde RTP a GUA pueden configurarse como dos paneles personalizados independientes llamados:

* RTP B2B
* Compromiso RTP

## Configuración de un tablero personalizado {#setting-up-a-custom-dashboard}

1. Inicie sesión en Google Analytics. Haz clic en **[!UICONTROL Informes]** en el menú superior. Haga clic en **[!UICONTROL Paneles]** y **[!UICONTROL Nuevo panel]**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Seleccione **Lienzo en blanco**, agregue un **Nombre de panel** y haga clic en **[!UICONTROL Crear panel]**.

1. Haga clic en **[!UICONTROL Agregar widget]** para crear un widget nuevo.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Panel RTP B2B {#rtp-b-b-dashboard}

Este tablero permite a los usuarios analizar el rendimiento de su sitio web desde una perspectiva B2B.

Proporciona información como el origen de la visita y el comportamiento en el sitio por sector, ingresos, tamaño, listas basadas en cuentas y segmentos de destino.

El tablero consta de 3 columnas

* Traffic source
* Segmentación
* Profundización firmográfica

1. Cree un nuevo tablero llamado **RTP B2B Dashboard** y defina los siguientes widgets:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Columna 1: Fuentes de tráfico
    </div></th> 
   <th> 
    <div> <strong>Columna 2 - Segmentación</strong> 
    </div></th> 
   <th> 
    <div> <strong>Columna 3 - Exploración en profundidad por firmografía</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: Sesiones por segmentos y canales</li> 
     <li>Tipo de widget: <span class="uicontrol">Barra</span><br></li> 
     <li><span class="uicontrol">Crear un gráfico de barras que muestre</span>: <span class="uicontrol">Sesión</span></li> 
     <li><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">Etiqueta de evento</span></li> 
     <li><span class="uicontrol">Tabla dinámica por</span>: <span class="uicontrol">Agrupación de canales predeterminada</span></li> 
     <li>Filtro: <br><span class="uicontrol">Mostrar solo</span> | <span class="uicontrol">Segmentos RTP de categoría de evento</span> (<span class="uicontrol">que contienen</span>)</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: N.º de usuarios segmentados RTP</li> 
     <li>Tipo: <span class="uicontrol">2.1 Métrica</span></li> 
     <li><span class="uicontrol">Mostrar la siguiente métrica</span>: <span class="uicontrol">Usuarios</span><br></li> 
     <li>Filtro: <br><span class="uicontrol">Mostrar solo</span> | <span class="uicontrol">Categoría de evento</span> (que contiene) segmentos RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: Sesiones por sector</li> 
     <li>Tipo: <span class="uicontrol">Circular</span><br></li> 
     <li><span class="uicontrol">Crear un gráfico circular que muestre</span>: <span class="uicontrol">Sesiones</span></li> 
     <li><span class="uicontrol">Agrupado por</span> : <span class="uicontrol">RTP-Industry</span></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por sector y canales</strong></li> 
     <li><strong>Tipo de widget: <span class="uicontrol">Barra</span></strong></li> 
     <li><strong><span class="uicontrol">Crear un gráfico de barras que muestre</span>: <span class="uicontrol">Sesión</span></strong></li> 
     <li><strong><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">RTP-Industry</span></strong></li> 
     <li><strong><span class="uicontrol">Tabla dinámica por</span>: <span class="uicontrol">Agrupación de canales predeterminada</span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones segmentadas por país</strong></li> 
     <li><strong>Tipo: <span class="uicontrol">Geomap</span></strong></li> 
     <li><strong><span class="uicontrol">Métrica seleccionada en el diagrama</span>: <span class="uicontrol">País</span> | <span class="uicontrol">Sesiones</span></strong></li> 
     <li><strong><span class="uicontrol">Seleccionar una región</span>: <span class="uicontrol">El mundo</span></strong></li> 
     <li><strong>Filtro: <span class="uicontrol">Mostrar solo</span> | <span class="uicontrol">Categoría de evento</span> (que contiene) segmentos RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por Categoría RTP</strong></li> 
     <li><strong>Tipo: <span class="uicontrol">Circular</span></strong></li> 
     <li><strong><span class="uicontrol">Crear un gráfico circular que muestre</span>: <span class="uicontrol">Sesiones</span></strong></li> 
     <li><strong><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">RTP-Category</span></strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Segmentos de destinatario principales</li> 
     <li>Tipo: <span class="uicontrol">Barra</span></li> 
     <li><span class="uicontrol">Crear un gráfico de barras que muestre</span>: <span class="uicontrol">Usuarios</span></li> 
     <li><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">Acción de evento</span></li> 
     <li>Filtro: <span class="uicontrol">Mostrar solo</span> | <span class="uicontrol">Categoría de evento</span> (que contiene) segmentos RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones por grupos RTP</li> 
     <li>Tipo: barra<br></li> 
     <li>Crear un gráfico de barras que muestre: Sesiones</li> 
     <li>Agrupado por: RTP-Group</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones y objetivos por segmentos principales</li> 
     <li>Tipo: Tabla<br></li> 
     <li>Mostrar las siguientes columnas: <br>Etiqueta de evento | Sesiones | Tasa de conversión de objetivos</li> 
     <li>Filtro: <br>Mostrar solo | Categoría de evento (contenedor) RTP-Segmentos</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
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
    <div> <strong>Clic en campañas en la columna 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Motor de recomendación de columna 3</strong> 
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
     <li>Filtros:<br><strong>[mostrar solo] Categoría de evento (contiene): RTP-Campaigns</strong><br><strong>[mostrar solo] Acción de evento (exactamente coincidente): Impresión</strong>[no mostrar] Etiqueta de evento (contiene): #</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>CTA total (clic)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría de evento (contiene): RTP-Campaigns</strong><br><strong>[mostrar solo] Acción de evento (exactamente coincidente): Clics</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>CRE - Total de clics</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">2.1 Métrica</span></strong><br></li> 
     <li><span class="uicontrol">Mostrar la siguiente métrica</span>: <strong><span class="uicontrol">Vistas de página</span></strong></li> 
     <li>Filtro: <strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Página</span> (<span class="uicontrol">que contiene</span>): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>Promedio Duración de la sesión (participación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Promedio Duración de la sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría de evento (exactamente igual): RTP-Campaigns</strong><br><strong>[mostrar solo] Acción de evento (exactamente igual): impression</strong><strong>[no mostrar] Etiqueta de evento (conteniendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>Promedio Duración de la sesión (clic)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Promedio Duración de la sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría de evento (exactamente igual): RTP-Campaigns</strong><br><strong>[mostrar solo] Acción de evento (exactamente igual): clicks</strong><strong>[no mostrar] Etiqueta de evento (conteniendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>CRE - Contenido principal recomendado</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabla</span></strong><br></li> 
     <li><span class="uicontrol">Mostrar las siguientes columnas</span>: <br><strong><span class="uicontrol">Título de la página</span> | <span class="uicontrol">Vistas de página</span></strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Página</span> (<span class="uicontrol">que contiene</span>): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas / Sesión (Participación)</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">2.1 Métrica</span> </strong></li> 
     <li><span class="uicontrol">Mostrar la siguiente métrica</span>: <strong><span class="uicontrol">Páginas / Sesión</span></strong></li> 
     <li>Filtros:<br><strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Categoría de evento</span> (<span class="uicontrol">exactamente igual</span>): RTP-Campaigns</strong></li> 
     <li><strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Acción de evento</span> (<span class="uicontrol">exactamente igual a</span>): impresión</strong></li> 
     <li><strong>[<span class="uicontrol">no mostrar</span>] <span class="uicontrol">Etiqueta de evento</span> (<span class="uicontrol">que contiene</span>): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas / Sesión (Pulsación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Páginas / Sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solo] Categoría de evento (exactamente igual): RTP-Campaigns</strong></li> 
     <li><strong>[only show] Acción de evento (exactamente igual): clics</strong></li> 
     <li><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Impresiones de CTA</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabla</span></strong></li> 
     <li><span class="uicontrol">Mostrar las siguientes columnas</span>: <strong><span class="uicontrol">Etiqueta de evento</span> | <span class="uicontrol">Eventos totales</span> | <span class="uicontrol">Usuarios</span></strong></li> 
     <li>Filtros:<br><strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Categoría de evento</span> (<span class="uicontrol">exactamente igual</span>): RTP-Campaigns</strong><br><strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Acción de evento</span> (<span class="uicontrol">exactamente igual</span>): impresión</strong><strong>[<span class="uicontrol">no mostrar</span>] <span class="uicontrol">Etiqueta de evento</span> (<span class="uicontrol">que contiene</span>): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Clic de CTA</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabla</span></strong></li> 
     <li><span class="uicontrol">Mostrar las siguientes columnas</span>: <strong><span class="uicontrol">Etiqueta de evento</span> | <span class="uicontrol">Eventos totales</span> | <span class="uicontrol">Usuarios</span></strong></li> 
     <li>Filtros:<br><strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Categoría de evento</span> (<span class="uicontrol">exactamente igual</span>): RTP-Campaigns</strong><br><strong>[<span class="uicontrol">solo mostrar</span>] <span class="uicontrol">Acción de evento</span> (<span class="uicontrol">exactamente igual</span>): clicks</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integrar RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Informes RTP personalizados en Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
