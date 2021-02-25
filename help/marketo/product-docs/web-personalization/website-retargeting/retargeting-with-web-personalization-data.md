---
unique-page-id: 4720796
description: Redireccionamiento con datos de personalización web - Documentos de marketing - Documentación del producto
title: Redireccionamiento con datos de personalización web
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---


# Redireccionamiento con datos de personalización web {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>El redireccionamiento de sitios web ahora se encuentra en el mosaico Personalización web. Si solo compró Retargeting, verá este mosaico y accederá al producto de Personalización web con **sólo** características de redireccionamiento habilitadas. Esto le permite acceder a la configuración de la cuenta, la página de redireccionamiento, los segmentos y las páginas de seguimiento adicionales.

Destinatarios de remercadotecnia clientes potenciales que han visitado su sitio en el pasado con anuncios en pantalla basados en quiénes son y qué han hecho. La reorientación personalizada destinatario audiencias específicas con anuncios relevantes basados en el sector, cuentas con nombre y datos de personas conocidas.

Personalización web anexa datos a las siguientes plataformas de remercadotecnia:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Personalización web envía los siguientes datos a las plataformas de remercadotecnia para crear audiencias y ejecutar campañas de publicidad de remercadotecnia:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Datos de personalización de Web</th> 
  </tr> 
  <tr> 
   <th><p>Industria</p></th> 
  </tr> 
  <tr> 
   <th><p>Grupo (Enterprise, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Categoría (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>LISTA ABM (Listas de cuenta con nombre)</p></th> 
  </tr> 
  <tr> 
   <th><p>Audiencia segmentada (basada en segmentos)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campañas Web en las que se hizo clic</p></th> 
  </tr> 
 </tbody> 
</table>

## Configuración de remercadotecnia {#remarketing-configuration}

1. Vaya a **Retargeting**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configuración de redireccionamiento es por dominio o subdominio. Active los otros dominios si desea enviar datos desde esos dominios a través de la plataforma de resegmentación.

1. Activar la configuración para Google Analytics o Google Universal Analytics por dominio.

   >[!NOTE]
   >
   >Debe implementar la etiqueta de redireccionamiento de Google en su sitio web.
   >
   >Si ya ha configurado la integración con Google Analytics y Personalización web, no es necesario que edite esta parte, ya que es la misma configuración en Configuración de cuenta.

   ![](assets/two.png)

1. Active la configuración para Facebook. Haga clic y expanda el acordeón de Facebook, haga clic en **Activado** para enviar el Evento y los datos respectivos a través del Audience Manager de Facebook. Haga clic en **Guardar**.

   >[!NOTE]
   >
   >Debe tener [Píxel de Audiencia personalizada de Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)instalado el sitio web para que esta función funcione.

   ![](assets/three.png)

## Creación de Audiencia segmentada {#creating-segmented-audience}

Una Audiencia segmentada le permite seleccionar un segmento existente como audiencia para usar para volver a segmentar campañas. Por ejemplo, si selecciona los segmentos de Persona conocida.

>[!TIP]
>
>No es necesario crear una Audiencia segmentada para datos del sector u otros datos que ya se han enviado en la Configuración de dominio. Es mejor utilizar Audiencias segmentadas para segmentos basados en datos de personas conocidas.

1. Haga clic en **Crear Audiencia segmentada**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Introduzca el nombre de la audiencia, seleccione Canales y seleccione Segmento en la lista de segmentos existentes.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Haga clic en **Guardar**.

   Ha completado la configuración de redireccionamiento en la personalización web, inicie sesión en las plataformas de redireccionamiento y cree sus audiencias basadas en estos datos y configure sus campañas de redireccionamiento de publicidad.
