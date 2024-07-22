---
unique-page-id: 4720810
description: Remarketing personalizado en Google - Documentos de Marketo - Documentación del producto
title: Remarketing personalizado en Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Remarketing personalizado en Google {#personalized-remarketing-in-google}

El remarketing personalizado le permite volver a interactuar con los usuarios mediante datos RTP y la potencia de los Google Analytics con el alcance de la red de pantallas de Google.

>[!PREREQUISITES]
>
>* Complete la configuración de [Redireccionamiento con datos de Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Revise la documentación de [Remarketing con ayuda para Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645).

## Creación de una audiencia de remarketing en Google {#creating-a-remarketing-audience-in-google}

1. Inicie sesión en sus Google Analytics. Haga clic en **Administrador**, **Cuenta**, **Propiedad**. Haga clic en **Definiciones de audiencias** y **Audiencias**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Haga clic en **+Nueva audiencia**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configuración del vínculo**: vincule a su cuenta de Google AdWords. **Definir audiencia**: Haga clic en **Crear nuevo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. En el Generador de audiencias, haga clic en **Secuencias** y **Busque los datos RTP** en Dimension personalizados, variables personalizadas y eventos.

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
>* Dimension personalizados: Organización, Sector, Categoría (Fortune 500,1000, Global 2000), Grupo (Enterprise, SMB), Lista ABM (Lista de cuentas con nombre)
>* Categoría del evento: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Etiqueta de evento: Nombre del segmento, Nombre de la campaña, Nombre de la audiencia segmentada

**Ejemplo de audiencia de remarketing a partir de datos de audiencia segmentados RTP**

1. Haga clic en **Secuencias.**
1. Seleccionar **Etiqueta de evento.**
1. Escriba **Nombre de la audiencia segmentada** (tal como aparece en RTP).
1. Haga clic en **Aplicar**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Ejemplo de audiencia de datos del sector RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Haga clic en **Secuencias**.
1. Seleccione **RTP-Industry**.
1. Escriba **Nombre del sector** (p. ej. Servicios Financieros, Educación...).
1. Haga clic en **Aplicar**.
1. Escriba un **Nombre de audiencia**. Haga clic en **Guardar**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Creación de una campaña de publicidad de remarketing en Google AdWords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Inicie sesión en **Google Adwords**. Haga clic en **Campañas**, seleccione **Solo red de visualización**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Escriba **Nombre De Campaña**, Seleccione **Remarketing De Tipo.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Escriba **Nombre del grupo de anuncios,** escriba **CPC mejorado**, seleccione **Lista de remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Haga clic en Guardar y continuar.
1. Añada su imagen o anuncio de texto e inicie su campaña de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Redireccionamiento con datos de Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado en Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
