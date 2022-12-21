---
unique-page-id: 4720917
description: 'Remarketing personalizado en Facebook: Marketo Docs: documentación del producto'
title: Remarketing personalizado en Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# Remarketing personalizado en Facebook {#personalized-remarketing-in-facebook}

El remarketing personalizado le permite volver a interactuar con sus usuarios mediante el uso de datos RTP y la potencia del remarketing de Facebook.

>[!PREREQUISITES]
>
>* Complete el [Redireccionamiento con datos de personalización web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configuración
>* Consulte la [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Documentación de facebook sobre Audiencias personalizadas](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) y Remarketing.


## Creación de una audiencia en Facebook {#creating-an-audience-in-facebook}

1. En Facebook, vaya a su [Pestaña Audiencia](https://www.facebook.com/ads/audience_manager) en el Administrador de anuncios.

1. Haga clic en **Herramientas** y seleccione **Audiencias**.

   ![](assets/one-1.png)

1. Haga clic en **Crear una audiencia personalizada**.

   ![](assets/two-1.png)

1. Select **Tráfico del sitio web**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. En la lista Tráfico del sitio web, seleccione **Combinación personalizada**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. En la lista Incluir, seleccione **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. En la lista Evento, seleccione **Remarketing de RTP** y seleccione un parámetro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Para este ejemplo, seleccione Industria para contener **Educación**. Entrar **Educación** y editar **En el último** a 180 días. Escriba el nombre de la audiencia: **Sector educativo**. Haga clic en **Crear audiencia**.

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
   <td>Remarketing de RTP</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parámetro</th> 
        <th>Valor</th> 
       </tr> 
       <tr> 
        <td>Lista ABM</td> 
        <td>(Nombre de la lista basada en cuentas)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Categoría</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Grupo</td> 
        <td colspan="1"><p>Empresarial</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Industria</td> 
        <td><p>Defensa</p><p>Educación</p><p>Servicios financieros</p><p>Gobierno</p><p>Salud, Pharma, Biotecnología</p><p>Software e Internet</p><p>etc... (según las opciones de RTP Industry)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Audiencia segmentada</td> 
        <td colspan="1">(Nombre de la audiencia segmentada creada en RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Segmentar la audiencia con una publicidad {#target-your-audience-with-an-ad}

Para obtener más información, consulte [Documentación de facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vaya al Administrador de publicidades, haga clic en **Crear publicidad**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Select **Enviar personas a su sitio web** como objetivo de la campaña.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Introduzca la URL del sitio web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Cree su conjunto de anuncios. Seleccione una audiencia personalizada de la lista de audiencias que ha creado, por ejemplo, Sector educativo.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Seleccione todas las demás opciones de conjuntos de anuncios, establezca su presupuesto y defina sus elementos creativos de publicidad.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Ahora todos están configurados con una campaña de remarketing personalizada en Facebook.

>[!MORELIKETHIS]
>
>* [Redireccionamiento con datos de personalización web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado en Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

