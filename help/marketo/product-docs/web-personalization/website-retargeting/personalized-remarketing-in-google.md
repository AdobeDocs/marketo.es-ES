---
unique-page-id: 4720810
description: Remarketing personalizado en Google - Documentos de Marketo - Documentación del producto
title: Remarketing personalizado en Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Remarketing personalizado en Google {#personalized-remarketing-in-google}

El remarketing personalizado le permite volver a interactuar con los usuarios mediante datos RTP y la potencia de Google Analytics con el alcance de la red de pantallas de Google.

>[!PREREQUISITES]
>
>* Complete la configuración de [Redireccionamiento con [!DNL Web Personalization] Datos](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Revise la documentación de [Remarketing con la Ayuda de Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645).

## Creación de una audiencia de remarketing en Google {#creating-a-remarketing-audience-in-google}

1. Inicie sesión en su Google Analytics. Haga clic en **[!UICONTROL Administrador]**, **[!UICONTROL Cuenta]**, **[!UICONTROL Propiedad]**. Haga clic en **[!UICONTROL Definiciones de audiencias]** y **[!UICONTROL Audiencias]**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Haga clic en **[!UICONTROL +Nueva audiencia]**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Configuración del vínculo]**: vincule a su cuenta de [!DNL Google Adwords]. **[!UICONTROL Definir audiencia]**: Haga clic en **[!UICONTROL Crear nuevo]**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. En el Generador de audiencias, haga clic en **[!UICONTROL Secuencias]** y **[!UICONTROL Busque los datos RTP]** en [!UICONTROL Dimensiones personalizadas], [!UICONTROL UICONTROL [.]Variables personalizadas &#x200B;], [!UICONTROL Eventos].

>[!TIP]
>
>¿Cómo se encuentran los datos RTP en Analytics para crear una audiencia?
>
>En Google Analytics:
>
>* Variables personalizadas: organización, sector
>* Categoría de evento: Segmento, Insightera-CTA, RTP-Remarketing
>* Etiqueta de evento: Nombre del segmento, Nombre de la campaña, Nombre de la audiencia segmentada
>
>En Google Universal Analytics:
>
>* Dimensiones personalizadas: Organización, Sector, Categoría (Fortune 500,1000, Global 2000), Grupo (Empresa, SMB), Lista ABM (Lista de cuentas con nombre)
>* Categoría del evento: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Etiqueta de evento: Nombre del segmento, Nombre de la campaña, Nombre de la audiencia segmentada

**Ejemplo de audiencia de remarketing a partir de datos de audiencia segmentados RTP**

1. Haga clic en **[!UICONTROL Secuencias].**
1. Seleccionar **[!UICONTROL Etiqueta de evento].**
1. Escriba **[!UICONTROL Nombre de la audiencia segmentada]** (tal como aparece en RTP).
1. Haga clic en **[!UICONTROL Aplicar]**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Ejemplo de audiencia de datos del sector RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Haga clic en **[!UICONTROL Secuencias]**.
1. Seleccione **[!UICONTROL RTP-Industry]**.
1. Escriba **Nombre del sector** (p. ej. [!UICONTROL Servicios Financieros], [!UICONTROL Educación]...).
1. Haga clic en **[!UICONTROL Aplicar]**.
1. Escriba un **[!UICONTROL Nombre de audiencia]**. Haga clic en **[!UICONTROL Guardar]**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Crear una campaña de anuncios de remarketing en [!DNL Google Adwords] {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Inicie sesión en **[!DNL Google Adwords]**. Haga clic en **[!UICONTROL Campañas]**, seleccione **[!UICONTROL Solo red de visualización]**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Escriba **[!UICONTROL Nombre De Campaña]**, Seleccione **[!UICONTROL Remarketing De Tipo].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Escriba **[!UICONTROL Nombre del grupo de anuncios],**, **[!UICONTROL CPC mejorado]**, seleccione **[!UICONTROL Lista de remarketing]**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Haga clic en **[!UICONTROL Guardar]** y continúe.
1. Añada su imagen o anuncio de texto e inicie su campaña de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Redireccionamiento con [!DNL Web Personalization] datos](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado en [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
