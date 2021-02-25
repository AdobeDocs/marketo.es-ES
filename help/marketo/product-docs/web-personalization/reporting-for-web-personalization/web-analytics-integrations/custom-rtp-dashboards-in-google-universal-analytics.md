---
unique-page-id: 7504238
description: Paneles RTP personalizados en Google Universal Analytics - Documentos de marketing - Documentación del producto
title: Paneles RTP personalizados en Google Universal Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# Paneles RTP personalizados en Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

En esta publicación se explica cómo configurar paneles RTP en Google Universal Analytics (GUA). Los datos enviados desde RTP a GUA pueden configurarse como dos paneles personalizados independientes llamados:

* RTP B2B
* Participación de RTP

## Configuración de un Panel personalizado {#setting-up-a-custom-dashboard}

1. Inicie sesión en Google Analytics. Haga clic en **Sistema de informes** en el menú superior. Haga clic en **Paneles** y **+Nuevo Panel personalizado**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Seleccione **Lienzo en blanco**, agregue un **nombre de Panel** y haga clic en **Crear Panel**.

1. Haga clic en **Añadir utilidad** para crear una nueva utilidad.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Panel RTP B2B {#rtp-b-b-dashboard}

Este panel permite a los usuarios analizar el rendimiento del sitio web desde una perspectiva B2B.

Proporciona información como el origen de visitas y el comportamiento en el sitio por sector, ingresos, tamaño, listas basadas en cuenta y segmentos de destinatarios.

El panel consta de 3 columnas

* Fuente de tráfico
* Segmentación
* Exploración en profundidad en firma

1. Cree un nuevo panel llamado **Panel RTP B2B** y defina los siguientes widgets:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Columna 1 - Fuentes de tráfico
    </div></th> 
   <th> 
    <div> <strong>Columna 2 - Segmentación</strong> 
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
     <li>Nombre: Sesiones por segmentos y Canales</li> 
     <li>Tipo de utilidad: Barra<br></li> 
     <li>Cree un gráfico de barras que muestre: Sesión</li> 
     <li>Agrupado por: Etiqueta de evento</li> 
     <li>Tabla dinámica por: Agrupación de Canales predeterminada</li> 
     <li>Filtro: <br>Mostrar sólo | Categoría de Evento (que contiene) RTP-Segments</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: N.º de usuarios segmentados de RTP</li> 
     <li>Tipo: 2.1 Métrica</li> 
     <li>Mostrar la métrica siguiente: Usuarios<br></li> 
     <li>Filtro: <br>Mostrar sólo | Categoría de Evento (que contiene) RTP-Segments</li> 
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
     <li><strong>Nombre: Sesiones por industria y Canales</strong></li> 
     <li><strong>Tipo de utilidad: Barra</strong></li> 
     <li><strong>Cree un gráfico de barras que muestre: Sesión</strong></li> 
     <li><strong>Agrupado por: RTP-Industry</strong></li> 
     <li><strong>Tabla dinámica por: Agrupación de Canales predeterminada</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones segmentadas por país</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Trazar la métrica seleccionada: País | Sesiones</strong></li> 
     <li><strong>Seleccione una región: El mundo</strong></li> 
     <li><strong>Filtro: Mostrar sólo | Categoría de Evento (que contiene) RTP-Segments</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nombre: Sesiones por Categoría RTP</strong></li> 
     <li><strong>Tipo: Circular</strong></li> 
     <li><strong>Cree un gráfico circular que muestre: Sesiones</strong></li> 
     <li><strong>Agrupado por: Categoría RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Segmentos de Destinatario principales</li> 
     <li>Tipo: Barra</li> 
     <li>Cree un gráfico de barras que muestre: Usuarios</li> 
     <li>Agrupado por: Acción de evento</li> 
     <li>Filtro: Mostrar sólo | Categoría de Evento (que contiene) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones por grupos RTP</li> 
     <li>Tipo: Barra<br></li> 
     <li>Cree un gráfico de barras que muestre: Sesiones</li> 
     <li>Agrupado por: RTP-Group</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nombre: Sesiones y objetivos por segmentos principales</li> 
     <li>Tipo: Tabla<br></li> 
     <li>Muestre las siguientes columnas: <br>Etiqueta de Evento | Sesiones | Tasa de conversión de objetivos</li> 
     <li>Filtro: <br>Mostrar sólo | Categoría de Evento (que contiene) RTP-Segments</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Panel de compromiso RTP {#rtp-engagement-dashboard}

Este panel permite a los usuarios analizar el rendimiento de la campaña RTP y las participaciones de los motores de recomendación. Proporciona una comparación del promedio. duración de la sesión y páginas por sesión entre:

* No comprometido
* Participación (impresiones y clics en una campaña personalizada)
* Clics en el motor de recomendación y en el contenido recomendado principal

Cree un nuevo panel llamado **Panel de compromiso RTP** y defina los siguientes widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Exposición de Campañas de columna 1</strong> 
    </div></th> 
   <th> 
    <div> <strong>Pulsaciones de Campañas de la columna 2</strong> 
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
     <li>Nombre: <strong>Llamada a acción total (participación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la métrica siguiente: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (contiene): Acción de Evento RTP-Campañas</strong><br><strong>[mostrar solamente] (coincidencia exacta): Impresión</strong><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Llamada a acción total (pulsación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la métrica siguiente: <strong>Eventos totales</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (contiene): Acción de Evento RTP-Campañas</strong><br><strong>[mostrar solamente] (exactamente coincidente): Clics</strong><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>CRE - Total de clics</strong></li> 
     <li>Tipo: <strong>Métrica 2.1</strong><br></li> 
     <li>Mostrar la métrica siguiente: <strong>Vistas de página</strong></li> 
     <li>Filtro: <strong>[solamente mostrar] Página (que contiene): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>Promedio Duración de la sesión (compromiso)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la métrica siguiente: <strong>Promedio Duración de la sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (coincidencia exacta): Acción de Evento RTP-Campañas</strong><br><strong>[mostrar solamente] (exactamente coincidente): impresiones</strong><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>Promedio Duración de la sesión (pulsación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la métrica siguiente: <strong>Promedio Duración de la sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (coincidencia exacta): Acción de Evento RTP-Campañas</strong><br><strong>[mostrar solamente] (exactamente coincidente): clicks</strong><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nombre: <strong>CRE - Contenido recomendado principal</strong></li> 
     <li>Tipo: <strong>Tabla</strong><br></li> 
     <li>Muestre las siguientes columnas: <br><strong>Título de página | Vistas de página</strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[solamente mostrar] Página (que contiene): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas / Sesión (compromiso)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la métrica siguiente: <strong>Páginas / Sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (coincidencia exacta): Campañas RTP</strong></li> 
     <li><strong>Acción de Evento [solo mostrar] (exactamente coincidente): impresión</strong></li> 
     <li><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Páginas / Sesión (pulsación)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar la métrica siguiente: <strong>Páginas / Sesión</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (coincidencia exacta): Campañas RTP</strong></li> 
     <li><strong>Acción de Evento [solo mostrar] (exactamente coincidente): clics</strong></li> 
     <li><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Impresiones de CTA</strong></li> 
     <li>Tipo: <strong>Tabla</strong></li> 
     <li>Muestre las siguientes columnas: <strong>Etiqueta de Evento | Eventos totales | Usuarios</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (coincidencia exacta): Acción de Evento RTP-Campañas</strong><br><strong>[mostrar solamente] (exactamente coincidente): impresiones</strong><strong>[no mostrar] Etiqueta de Evento (que contiene): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nombre: <strong>Pulsación por CTA</strong></li> 
     <li>Tipo: <strong>Tabla</strong></li> 
     <li>Muestre las siguientes columnas: <strong>Etiqueta de Evento | Eventos totales | Usuarios</strong></li> 
     <li>Filtros:<br><strong>[mostrar solamente] Categoría de Evento (coincidencia exacta): Acción de Evento RTP-Campañas</strong><br><strong>[mostrar solamente] (exactamente coincidente): clicks</strong></li> 
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
