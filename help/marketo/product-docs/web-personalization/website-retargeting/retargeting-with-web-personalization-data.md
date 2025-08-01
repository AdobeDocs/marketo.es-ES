---
unique-page-id: 4720796
description: 'Redireccionamiento con datos de Personalization web: documentos de Marketo, documentación del producto'
title: Redireccionamiento con datos de Web Personalization
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 2%

---

# Redireccionamiento con datos de [!DNL Web Personalization] {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>La reorientación del sitio web ahora se encuentra en el mosaico de Web Personalization. Si solo compraste Retargeting, verás este mosaico y accederás al producto [!DNL Web Personalization] con las características de redireccionamiento de **solamente** habilitadas. Esto le proporciona acceso a la configuración de la cuenta, la página de redireccionamiento, los segmentos y las páginas de seguimiento adicionales.

El remarketing se dirige a los posibles clientes que han visitado su sitio en el pasado con publicidad de display en función de quiénes son y qué han hecho. El retargeting personalizado se dirige a audiencias específicas con anuncios relevantes basados en el sector, cuentas con nombre y datos de personas conocidas.

Web Personalization adjunta datos a las siguientes plataformas de remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] envía los siguientes datos a las plataformas de remarketing para crear audiencias y ejecutar campañas de remarketing y publicidad:

<table>
 <tbody>
  <tr>
   <th colspan="1">[!DNL Web Personalization] Datos</th>
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

1. Vaya a **[!UICONTROL Redireccionamiento]**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configuración de redireccionamiento es por dominio o subdominio. Active los demás dominios si desea enviar datos de esos dominios a la plataforma de retargeting.

1. Activar la configuración de Google Analytics o [!DNL Google Universal Analytics] por dominio.

   >[!NOTE]
   >
   >Debe tener la etiqueta de redireccionamiento de Google implementada en el sitio web.
   >
   >Si ya ha configurado la integración con Web Personalization y Google Analytics, no es necesario editar este artículo, ya que es la misma configuración en Configuración de cuenta.

   ![](assets/two.png)

1. Active la configuración para Facebook. Haga clic y expanda el acordeón [!DNL Facebook]. Haga clic en **[!UICONTROL Activado]** para enviar el evento y los datos respectivos a Facebook Audience Manager. Haga clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >Necesita tener [[!DNL Facebook] Píxel de audiencia personalizado](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) instalado en el sitio web para que funcione esta característica.

   ![](assets/three.png)

## Creación de audiencias segmentadas {#creating-segmented-audience}

Una audiencia segmentada le permite seleccionar un segmento existente como una audiencia que usar para campañas de retargeting. Por ejemplo, al seleccionar los segmentos de Persona conocida.

>[!TIP]
>
>No es necesario crear una audiencia segmentada para el sector ni para otros datos que ya se hayan enviado en la configuración del dominio. Se recomienda utilizar Audiencias segmentadas para segmentos basados en datos de personas conocidas.

1. Haga clic en **[!UICONTROL Crear audiencia segmentada]**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Introduzca el nombre de la audiencia, seleccione Canales y seleccione Segmento en la lista de Segmentos existentes.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   Ahora ha completado la Configuración de retargeting en [!DNL Web Personalization], inicie sesión en sus plataformas de retargeting, cree sus audiencias en función de estos datos y configure sus campañas de anuncios de retargeting.
