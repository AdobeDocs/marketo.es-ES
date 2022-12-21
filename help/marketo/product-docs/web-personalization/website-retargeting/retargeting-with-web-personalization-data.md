---
unique-page-id: 4720796
description: 'Redireccionamiento con datos de personalización web: Documentos de Marketo: Documentación del producto'
title: Redireccionamiento con datos de personalización web
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Redireccionamiento con datos de personalización web {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>El redireccionamiento de sitios web ahora se encuentra en el mosaico Personalización web . Si solo ha comprado redireccionamiento, verá este mosaico y accederá al producto de personalización web con **only** Funciones de redireccionamiento habilitadas. Esto le permite acceder a la configuración de la cuenta, a la página de redirección, a los segmentos y a las páginas de seguimiento adicionales.

El remarketing se dirige a aquellos clientes potenciales que han visitado su sitio en el pasado con publicidad gráfica basada en quiénes son y qué han hecho. La reorientación personalizada se dirige a audiencias específicas con anuncios relevantes basados en el sector, cuentas con nombre y datos de personas conocidas.

La personalización web actualmente anexa datos a las siguientes plataformas de remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

La personalización web envía los siguientes datos a las plataformas de remarketing para crear audiencias y ejecutar campañas de anuncios de remarketing:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Datos de personalización web</th> 
  </tr> 
  <tr> 
   <th><p>Industria</p></th> 
  </tr> 
  <tr> 
   <th><p>Grupo (Empresa, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Categoría (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>Lista ABM (Listas de cuentas con nombre)</p></th> 
  </tr> 
  <tr> 
   <th><p>Audiencia segmentada (basada en segmentos)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campañas web en las que se hizo clic</p></th> 
  </tr> 
 </tbody> 
</table>

## Configuración de remarketing {#remarketing-configuration}

1. Vaya a **Redireccionamiento**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configuración de redireccionamiento es por dominio o subdominio. Active los demás dominios si desea enviar datos de esos dominios a la plataforma de resegmentación.

1. Activar la configuración para Google Analytics o Google Universal Analytics por dominio.

   >[!NOTE]
   >
   >Debe implementar la etiqueta de redireccionamiento de Google en el sitio web.
   >
   >Si ya ha configurado la integración con la personalización web y los Google Analytics, no es necesario que edite esta parte, ya que es la misma configuración en Configuración de cuenta.

   ![](assets/two.png)

1. Active la configuración para Facebook. Haga clic en y expanda el acordeón de Facebook, haga clic en **Activado** para enviar el evento y los datos respectivos a Facebook Audience Manager. Haga clic en **Guardar**.

   >[!NOTE]
   >
   >Debe tener [Píxel de audiencia personalizado de facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)ha instalado su sitio web para que funcione esta función.

   ![](assets/three.png)

## Creación de audiencias segmentadas {#creating-segmented-audience}

Una audiencia segmentada le permite seleccionar un segmento existente como audiencia para usarlo en campañas de resegmentación. Por ejemplo, si selecciona los segmentos de persona conocida .

>[!TIP]
>
>No es necesario crear una audiencia segmentada para datos del sector u otros datos que ya se hayan enviado en la configuración del dominio. Es mejor utilizar Audiencias segmentadas para segmentos basados en datos de personas conocidas.

1. Haga clic en **Crear audiencia segmentada**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Introduzca el nombre de la audiencia, seleccione Canales y seleccione Segmento en la lista de Segmentos existentes.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Haga clic en **Guardar**.

   Ya ha completado la configuración de redireccionamiento en la personalización web, ha iniciado sesión en las plataformas de redireccionamiento y ha creado audiencias basadas en estos datos, además de configurar las campañas de redireccionamiento de anuncios.
