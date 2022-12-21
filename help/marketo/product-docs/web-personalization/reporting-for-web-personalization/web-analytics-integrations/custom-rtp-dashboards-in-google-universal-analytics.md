---
unique-page-id: 7504238
description: Tableros RTP personalizados en Google Universal Analytics - Marketo Docs - Documentación del producto
title: Tableros RTP personalizados en Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Tableros RTP personalizados en Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integración de RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

En esta publicación se explica cómo configurar los paneles RTP en Google Universal Analytics (GUA). Los datos enviados desde RTP a GUA se pueden configurar como dos paneles personalizados independientes llamados:

* RTP B2B
* Participación de RTP

## Configuración de un tablero personalizado {#setting-up-a-custom-dashboard}

1. Inicie sesión en los Google Analytics. Haga clic en **Informes** en el menú superior. Haga clic en **Tableros** y **+Nuevo tablero personalizado**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Select **Lienzo en blanco**, agregue un **Nombre del panel** y haga clic en **Crear tablero**.

1. Haga clic en **Agregar utilidad** para crear un nuevo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Tablero RTP B2B {#rtp-b-b-dashboard}

Este tablero permite a los usuarios analizar el rendimiento de su sitio web desde una perspectiva B2B.

Proporciona información como fuente de visitas y comportamiento en el sitio por sector, ingresos, tamaño, listas basadas en cuentas y segmentos de objetivo.

El tablero consta de 3 columnas

* Fuente de tráfico
* Segmentos
* Exploración en profundidad de firma

1. Cree un nuevo tablero llamado **Tablero RTP B2B** y defina las siguientes utilidades:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Columna 1 - Fuentes de tráfico
    </div></th> 
   <th> 
    <div> <strong>Columna 2: Segmentación</strong> 
    </div></th> 
   <th> 
    <div> <strong>Columna 3 - Desglose Firmográfico</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: Sesiones por segmentos y canales</li> 
     <li>Tipo de utilidad: Barra<br></li> 
     <li>Cree un gráfico de barras que muestre: Sesión</li> 
     <li>Agrupado por: Etiqueta de evento</li> 
     <li>Dinámica por: Agrupación de canales predeterminada</li> 
     <li>Filtro: <br>Mostrar sólo | Categoría de evento (que contiene) RTP-Segments</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: N.º de usuarios segmentados de RTP</li> 
     <li>Tipo: Métrica 2.1</li> 
     <li>Mostrar la siguiente métrica: Usuarios<br></li> 
     <li>Filtro: <br>Mostrar sólo | Categoría de evento (que contiene) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: Sesiones por sector</li> 
     <li>Tipo: Circular<br></li> 
     <li>Cree un gráfico circular que muestre: Sesiones</li> 
     <li>Agrupado por: RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por sector y canales</strong></li> 
     <li><strong>Tipo de utilidad: Barra</strong></li> 
     <li><strong>Cree un gráfico de barras que muestre: Sesión</strong></li> 
     <li><strong>Agrupado por: RTP-Industry</strong></li> 
     <li><strong>Dinámica por: Agrupación de canales predeterminada</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones segmentadas por país</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Diagrama de métrica seleccionada: País | Sesiones</strong></li> 
     <li><strong>Seleccione una región: El mundo</strong></li> 
     <li><strong>Filtro: Mostrar sólo | Categoría de evento (que contiene) RTP-Segments</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por categoría RTP</strong></li> 
     <li><strong>Tipo: Circular</strong></li> 
     <li><strong>Cree un gráfico circular que muestre: Sesiones</strong></li> 
     <li><strong>Agrupado por: RTP-Category</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Segmentos de objetivo principales</li> 
     <li>Tipo: Barra</li> 
     <li>Cree un gráfico de barras que muestre: Usuarios</li> 
     <li>Agrupado por: Acción de evento</li> 
     <li>Filtro: Mostrar sólo | Categoría de evento (que contiene) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones por grupos RTP</li> 
     <li>Tipo: Barra<br></li> 
     <li>Cree un gráfico de barras que muestre: Sesiones</li> 
     <li>Agrupado por: Grupo RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones y objetivos por segmentos principales</li> 
     <li>Tipo: Tabla<br></li> 
     <li>Muestre las columnas siguientes: <br>Etiqueta de evento | Sesiones | Tasa de conversión de objetivos</li> 
     <li>Filtro: <br>Mostrar sólo | Categoría de evento (que contiene) RTP-Segments</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Panel de participación de RTP {#rtp-engagement-dashboard}

Este tablero permite a los usuarios analizar el rendimiento de sus campañas RTP y las participaciones de los motores de recomendación. Proporciona comparación de avg. duración de la sesión y páginas por sesión entre:

* Sin participación
* Participación (impresiones y clics en una campaña personalizada)
* Clics en el motor de recomendación y contenido recomendado

Cree un nuevo tablero llamado **Panel de participación de RTP** y defina las siguientes utilidades:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Columna 1 Exposición de campañas</strong> 
    </div></th> 
   <th> 
    <div> <strong>Columna 2 Pulsaciones en campañas</strong> 
    </div></th> 
   <th> 
    <div> <strong>Motor de recomendación de la columna 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Total de llamada a acción (participación)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (contiene): RTP-Campaigns</strong><br><strong>[mostrar solamente] Acción de evento (que coincida exactamente): Impresión</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Total de llamada a acción (pulsación)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (contiene): RTP-Campaigns</strong><br><strong>[mostrar solamente] Acción de evento (que coincida exactamente): Clics</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>CRE: Total de clics</strong></li> 
     <li>Tipo: <strong>Métrica 2.1</strong><br></li> 
     <li>Mostrar la siguiente métrica: <strong>Vistas de página</strong></li> 
     <li>Filtro: <strong>[mostrar solamente] Página (que contiene): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>Promedio de Duración de la sesión (participación)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Promedio de Duración de la sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (que coincida exactamente): RTP-Campaigns</strong><br><strong>[mostrar solamente] Acción de evento (que coincida exactamente): impresión</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>Promedio de Duración de la sesión (pulsación)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Promedio de Duración de la sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (que coincida exactamente): RTP-Campaigns</strong><br><strong>[mostrar solamente] Acción de evento (que coincida exactamente): clicks</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>CRE: contenido recomendado principal</strong></li> 
     <li>Tipo: <strong>Tabla</strong><br></li> 
     <li>Muestre las columnas siguientes: <br><strong>Título de página | Vistas de página</strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[mostrar solamente] Página (que contiene): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas / Sesión (Participación)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Páginas / Sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (que coincida exactamente): RTP-Campaigns</strong></li> 
     <li><strong>[mostrar solamente] Acción de evento (que coincida exactamente): impresión</strong></li> 
     <li><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas / Sesión (pulsación)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar la siguiente métrica: <strong>Páginas / Sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (que coincida exactamente): RTP-Campaigns</strong></li> 
     <li><strong>[mostrar solamente] Acción de evento (que coincida exactamente): clicks</strong></li> 
     <li><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Impresiones por CTA</strong></li> 
     <li>Tipo: <strong>Tabla</strong></li> 
     <li>Muestre las columnas siguientes: <strong>Etiqueta de evento | Eventos totales | Usuarios</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (que coincida exactamente): RTP-Campaigns</strong><br><strong>[mostrar solamente] Acción de evento (que coincida exactamente): impresión</strong><strong>[no mostrar] Etiqueta de evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Pulsación mediante llamada a acción</strong></li> 
     <li>Tipo: <strong>Tabla</strong></li> 
     <li>Muestre las columnas siguientes: <strong>Etiqueta de evento | Eventos totales | Usuarios</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría del evento (que coincida exactamente): RTP-Campaigns</strong><br><strong>[mostrar solamente] Acción de evento (que coincida exactamente): clicks</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integración de RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Informes RTP personalizados en Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
