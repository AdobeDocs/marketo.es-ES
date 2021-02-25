---
unique-page-id: 4720917
description: Remercadotecnia personalizada en Facebook - Documentos de marketing - Documentación del producto
title: Remercadotecnia personalizada en Facebook
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Remercadotecnia personalizada en Facebook {#personalized-remarketing-in-facebook}

La remercadotecnia personalizada le permite volver a interactuar con los usuarios mediante los datos RTP y el poder de la remercadotecnia de Facebook.

>[!PREREQUISITES]
>
>* Complete la configuración de [redireccionamiento con datos de personalización web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Revise la [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [documentación de Facebook sobre Audiencias personalizadas](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) y Remarketing.


## Creación de una Audiencia en Facebook {#creating-an-audience-in-facebook}

1. En Facebook, vaya a la ficha [Audiencia](https://www.facebook.com/ads/audience_manager) en el Administrador de publicidad.

1. Haga clic en **Herramientas** y seleccione **Audiencias**.

   ![](assets/one-1.png)

1. Haga clic en **Crear una Audiencia personalizada**.

   ![](assets/two-1.png)

1. Seleccione **Tráfico del sitio Web**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. En la lista de tráfico del sitio web, seleccione **Combinación personalizada**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. En la lista Incluir, seleccione **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. En la lista Evento, seleccione **Remarketing de RTP** y seleccione un parámetro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Para este ejemplo, seleccione Industria para contener **Educación**. Escriba **Educación** y edite **En el último** para que sea de 180 días. Escriba el nombre de la Audiencia: **Sector educativo**. Haga clic en **Crear Audiencia**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Ahora ha creado una nueva audiencia personalizada con datos RTP en Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Puntos de datos RTP en Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Nombre del evento</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>Remercadotecnia RTP</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parámetro</th> 
        <th>Valor</th> 
       </tr> 
       <tr> 
        <td>LISTA ABM</td> 
        <td>(Nombre de la Lista basada en la cuenta)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Categoría</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Grupo</td> 
        <td colspan="1"><p>Enterprise</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Industria</td> 
        <td><p>Defensa</p><p>Educación</p><p>Servicios financieros</p><p>Gobierno</p><p>Salud, farma, biotecnología</p><p>Software e Internet</p><p>etc... (según las opciones de RTP Industry)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Audiencia segmentada</td> 
        <td colspan="1">(Nombre de la Audiencia segmentada creada en RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Destinatario de su Audiencia con una publicidad {#target-your-audience-with-an-ad}

Para obtener más información, consulte la [documentación de Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vaya al Administrador de publicidad, haga clic en **Crear publicidad**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Seleccione **Enviar personas a su sitio Web** como objetivo de su campaña.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Introduzca la dirección URL del sitio web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Cree su conjunto de publicidad. Seleccione una audiencia personalizada de la lista de Audiencias que ha creado, por ejemplo, Sector educativo.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Seleccione todas las demás opciones de conjuntos de publicidad, establezca su presupuesto y defina sus elementos creativos de publicidad.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Ahora todos están configurados con una campaña de remarketing personalizada en Facebook.

>[!MORELIKETHIS]
>
>* [Redireccionamiento con datos de personalización web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remercadotecnia personalizada en Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

