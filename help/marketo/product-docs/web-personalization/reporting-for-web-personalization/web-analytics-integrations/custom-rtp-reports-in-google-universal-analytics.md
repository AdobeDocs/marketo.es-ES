---
unique-page-id: 7504218
description: Informes RTP personalizados en Google Universal Analytics - Documentos de marketing - Documentación del producto
title: Informes RTP personalizados en Google Universal Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---


# Informes RTP personalizados en Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

En este artículo se explica cómo configurar informes personalizados RTP para Google Universal Analytics (GUA).  Los datos enviados desde RTP a GUA pueden configurarse como dos informes personalizados independientes llamados:

* RTP B2B
* Participación de RTP

## Configuración de un informe personalizado {#setting-up-a-custom-report}

1. Inicie sesión en Google Analytics.

1. Haga clic en **Personalización** en el menú superior.

1. Haga clic en **+Nuevo informe personalizado**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## Informe RTP B2B {#rtp-b-b-report}

1. Asigne un nombre al informe **Informe RTP B2B**.

1. Asigne un nombre a la primera ficha **Industria**.

>[!NOTE]
>
>Va a **Duplicado esta ficha** y creará otras similares - paso 5)

1. Seleccione el tipo de informe **Explorador**.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. En la sección **Grupos de métricas**, seleccione las métricas que son relevantes para su negocio.

   a. Recomendamos lo siguiente:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplicado esta ficha 4 veces y asígneles un nombre:

   1. **Industria**
   1. **Grupo**
   1. **Categoría**
   1. **ABM**
   1. **Organizaciones**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. En la sección **Desgloses de Dimension** establezca las dimensiones relevantes para cada ficha como se muestra a continuación.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nombre de ficha 
    </div></th> 
   <th> 
    <div>
      Desgloses de Dimension
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Industria</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Categoría</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Organizaciones</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. No configure ningún filtros y establezca este informe para que esté disponible para **Todos los datos del sitio web** (o cambie si es relevante para una cuenta específica de Analytics).

1. Haga clic en **Guardar**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Informe de participación de RTP {#rtp-engagement-report}

1. Asigne un nombre al informe **Informe de participación de RTP**.

1. Establezca el nombre de la primera ficha en **Todos los compromisos**.

>[!NOTE]
>
>Esta ficha se Duplicado y se crean otras similares - paso 5)

1. Seleccione el tipo de informe **Explorador**.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. En la sección Grupos de métricas, seleccione las métricas que son relevantes para su negocio. Esta es una recomendación:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplicado esta ficha 4 veces y asígneles un nombre:

   1. **Todos los compromisos**
   1. **Participación por sector**
   1. **Participación por grupo**
   1. **Participación por Categoría**
   1. **Participación de ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. En la sección **Desgloses de Dimension** establezca las dimensiones relevantes para cada ficha como se muestra a continuación:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nombre de ficha 
    </div></th> 
   <th> 
    <div>
      Desgloses de Dimension 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Todos los compromisos</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participación de ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participación por Categoría</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participación por grupo</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participación por sector</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Establezca los siguientes filtros:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Campo 
    </div></th> 
   <th> 
    <div>
      Tipo de coincidencia 
    </div></th> 
   <th> 
    <div>
      Valores 
    </div></th> 
   <th colspan="1"> 
    <div>
      Comentarios 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>Incluir</p></td> 
   <td><p>Categoría evento</p></td> 
   <td>Regex</td> 
   <td>Campañas RTP|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">Filtrará todos los demás eventos personalizados que no estén relacionados con RTP</td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>Etiqueta evento</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Permite filtrar desde la campaña de informes utilizando # en el nombre de la campaña</td> 
  </tr> 
 </tbody> 
</table>

1. Configure este informe para que esté disponible para **Todos los datos del sitio Web** (o cambie si es necesario).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Haga clic en **Guardar**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrar RTP con Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Paneles RTP personalizados en Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
