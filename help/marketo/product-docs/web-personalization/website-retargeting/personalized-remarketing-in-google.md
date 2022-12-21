---
unique-page-id: 4720810
description: 'Remarketing personalizado en Google: Marketo Docs: documentación del producto'
title: Remarketing personalizado en Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Remarketing personalizado en Google {#personalized-remarketing-in-google}

La Remarketing personalizado le permite volver a interactuar con sus usuarios mediante el uso de datos RTP y la potencia de los Google Analytics con el alcance de la red de visualización de Google.

>[!PREREQUISITES]
>
>* Complete el [Redireccionamiento con datos de personalización web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configuración
>* Consulte [Ayuda de Remarketing con Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) documentación.


## Creación de una audiencia de remarketing en Google {#creating-a-remarketing-audience-in-google}

1. Inicie sesión en sus Google Analytics. Haga clic en **Administrador**, **Cuenta**, **Propiedad**. Haga clic en **Definiciones de audiencias** y **Audiencias**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Haga clic en **+Nueva audiencia**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configuración de vínculos**: Vincule a su cuenta de Google Adwords . **Definir audiencia**: Haga clic en **Crear nuevo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. En el Generador de audiencias, haga clic en **Secuencias** y **Buscar los datos RTP** en Dimension personalizados, variables personalizadas, eventos.

>[!TIP]
>
>¿Cómo encontrar los datos RTP en Analytics para crear su audiencia?
>
>En Google Analytics:
>
>* Variables personalizadas: Organización, sector
>* Categoría del evento: Segmento, Insightera-CTA, Remarketing RTP
>* Etiqueta de evento: Nombre del segmento, Nombre de campaña, Nombre de audiencia segmentada
>
>En Google Universal Analytics:
>
>* Dimension personalizados: Organización, sector, categoría (Fortune 500,1000, Global 2000), grupo (Enterprise, SMB), lista ABM (Named Account List)
>* Categoría del evento: RTP-Segmento, RTP-Campaign RTP-Remarketing
>* Etiqueta de evento: Nombre del segmento, Nombre de campaña, Nombre de audiencia segmentada


**Ejemplo de audiencia de remarketing a partir de datos de audiencia segmentados de RTP**

1. Haga clic en **Secuencias.**
1. Select **Etiqueta de evento.**
1. Entrar **Nombre de la audiencia segmentada** (como aparece en RTP).
1. Haga clic en **Aplicar**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Ejemplo de audiencia a partir de datos del sector RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Haga clic en **Secuencias**.
1. Select **RTP-Industry**.
1. Entrar **Nombre del sector** (p. ej. Servicios financieros, educación...).
1. Haga clic en **Aplicar**.
1. Introduzca un **Nombre de audiencia**. Haga clic en **Guardar**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Creación de una campaña de anuncios de remarketing en Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Inicie sesión en **Adobe**. Haga clic en **Campañas**, seleccione **Mostrar solo red**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Entrar **Nombre de campaña**, seleccione **Escriba Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Entrar **Nombre del grupo de publicidad,** enter **CPC mejorado**, seleccione **Lista de remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Haga clic en Guardar y continúe.
1. Añada su imagen o publicidad de texto e inicie su campaña de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Redireccionamiento con datos de personalización web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado en Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

