---
unique-page-id: 4720796
description: 'Redireccionamiento con datos de personalización web: documentos de Marketo, documentación del producto'
title: Redireccionamiento con datos de personalización web
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Redireccionamiento con datos de personalización web {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>El redireccionamiento de sitios web ahora se encuentra en el mosaico de Personalización web. Si solo ha comprado Retargeting, verá este mosaico y accederá al producto Personalización web con **solamente** Funciones de redireccionamiento habilitadas. Esto le proporciona acceso a la configuración de la cuenta, la página de redireccionamiento, los segmentos y las páginas de seguimiento adicionales.

El remarketing se dirige a los posibles clientes que han visitado su sitio en el pasado con publicidad de display en función de quiénes son y qué han hecho. El retargeting personalizado se dirige a audiencias específicas con anuncios relevantes basados en el sector, cuentas con nombre y datos de personas conocidas.

Actualmente, Web Personalization anexa datos a las siguientes plataformas de remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

La personalización web envía los siguientes datos a las plataformas de remarketing para crear audiencias y ejecutar campañas de publicidad de remarketing:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Datos de personalización web</th> 
  </tr> 
  <tr> 
   <th><p>Industria</p></th> 
  </tr> 
  <tr> 
   <th><p>Grupo (empresas, pymes)</p></th> 
  </tr> 
  <tr> 
   <th><p>Categoría (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>Lista ABM (listas de cuentas con nombre)</p></th> 
  </tr> 
  <tr> 
   <th><p>Audiencia segmentada (según segmentos)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campañas web en las que se hizo clic</p></th> 
  </tr> 
 </tbody> 
</table>

## Configuración de remarketing {#remarketing-configuration}

1. Ir a **Redireccionamiento**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configuración de redireccionamiento es por dominio o subdominio. Active los demás dominios si desea enviar datos de esos dominios a la plataforma de retargeting.

1. Active Configuración para Google Analytics o Google Universal Analytics por dominio.

   >[!NOTE]
   >
   >Debe tener la etiqueta de redireccionamiento de Google implementada en el sitio web.
   >
   >Si ya ha configurado la integración con Personalización web y Google Analytics, no es necesario editar este artículo, ya que es la misma configuración en Configuración de cuenta.

   ![](assets/two.png)

1. Active la configuración de para Facebook. Haga clic en y expanda el acordeón de Facebook, haga clic en **Activado** para enviar los datos y el evento correspondientes al Audience Manager de Facebook. Clic **Guardar**.

   >[!NOTE]
   >
   >Tiene que tener [Píxel de audiencia personalizada de facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)ha instalado el sitio web para que funcione esta función.

   ![](assets/three.png)

## Creación de audiencias segmentadas {#creating-segmented-audience}

Una audiencia segmentada le permite seleccionar un segmento existente como una audiencia que usar para campañas de retargeting. Por ejemplo, al seleccionar los segmentos de Persona conocida.

>[!TIP]
>
>No es necesario crear una audiencia segmentada para el sector ni para otros datos que ya se hayan enviado en la configuración del dominio. Se recomienda utilizar Audiencias segmentadas para segmentos basados en datos de personas conocidas.

1. Clic **Crear audiencia segmentada**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Introduzca el nombre de la audiencia, seleccione Canales y seleccione Segmento en la lista de Segmentos existentes.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Clic **Guardar**.

   Ahora ha completado la Configuración de retargeting en Personalización web, ha iniciado sesión en sus plataformas de retargeting, ha creado sus audiencias en función de estos datos y ha configurado sus campañas de publicidad de retargeting.
