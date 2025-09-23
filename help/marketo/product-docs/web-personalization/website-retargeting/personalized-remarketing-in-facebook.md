---
unique-page-id: 4720917
description: Remarketing personalizado en Facebook - Documentos de Marketo - Documentación del producto
title: Remarketing personalizado en Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 6%

---

# Remarketing personalizado en [!DNL Facebook] {#personalized-remarketing-in-facebook}

El remarketing personalizado le permite volver a interactuar con los usuarios mediante datos RTP y el poder del remarketing de Facebook.

>[!PREREQUISITES]
>
>* Complete la configuración [Redireccionamiento con datos de Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Revise la [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [documentación de Facebook sobre audiencias personalizadas](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) y remarketing.

## Creando una audiencia en [!DNL Facebook] {#creating-an-audience-in-facebook}

1. En [!DNL Facebook], ve a tu [pestaña Audiencia](https://www.facebook.com/ads/audience_manager) en el Administrador de anuncios.

1. Haga clic en **[!UICONTROL Herramientas]** y seleccione **[!UICONTROL Audiencias]**.

![](assets/one-1.png)

1. Haga clic en **[!UICONTROL Crear una audiencia personalizada]**.

![](assets/two-1.png)

1. Seleccione **[!UICONTROL Tráfico del sitio web]**.

![](assets/image2015-1-19-16-3a32-3a2.png)

1. En la lista [!UICONTROL Tráfico del sitio web], seleccione **[!UICONTROL Combinación personalizada]**.

![](assets/image2015-1-19-16-3a33-3a21.png)

1. En la lista Incluir, seleccione **[!UICONTROL Evento]**.

![](assets/image2015-1-19-16-3a34-3a9.png)

1. En la lista [!UICONTROL Event], seleccione **[!UICONTROL RTP Remarketing]** y un parámetro.

![](assets/image2015-1-19-16-3a52-3a29.png)

1. Para este ejemplo, seleccione [!UICONTROL Sector] que contendrá **[!UICONTROL Educación]**. Ingresa a **[!UICONTROL Educación]** y edita **[!UICONTROL En los últimos]** 180 días. Escriba el nombre de la audiencia: **Sector educativo**. Haga clic en **[!UICONTROL Crear audiencia]**.

![](assets/image2015-1-19-16-3a56-3a15.png)

1. Ha creado una nueva audiencia personalizada con datos RTP en [!DNL Facebook].

![](assets/image2015-1-19-16-3a59-3a2.png)

## Puntos de datos RTP en [!DNL Facebook] {#rtp-data-points-in-facebook}

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
        <td colspan="1"><p>Enterprise</p><p>SMB</p></td>
       </tr>
       <tr>
        <td>Industria</td>
        <td><p>Defensa</p><p>Education</p><p>Servicios financieros</p><p>Government</p><p>Sanidad, Farmacia, Biotecnología</p><p>Software e Internet</p><p>etc... (según las opciones del sector RTP)</p></td>
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

## Dirija su audiencia a un anuncio {#target-your-audience-with-an-ad}

Para obtener más información, consulte [Documentación de Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vaya al Administrador de anuncios y haga clic en **[!UICONTROL Crear anuncio]**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Seleccione **[!UICONTROL Enviar personas a su sitio web]** como objetivo de su campaña.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Introduzca la URL de su sitio web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Cree su conjunto de anuncios. Seleccione una audiencia personalizada de la lista de audiencias que ha creado, por ejemplo, la industria educativa.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Seleccione todas las demás opciones del conjunto de anuncios, establezca el presupuesto y defina los elementos creativos del anuncio.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Ya está todo configurado con una campaña de remarketing personalizada en [!DNL Facebook].

>[!MORELIKETHIS]
>
>* [Redireccionamiento con datos de Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado en Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
