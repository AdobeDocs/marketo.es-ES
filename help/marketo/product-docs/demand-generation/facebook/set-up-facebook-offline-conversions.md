---
unique-page-id: 11383953
description: Obtenga información sobre cómo configurar conversiones sin conexión de Facebook en Marketo. Envíe datos de conversión de Marketo a Facebook para la optimización de anuncios.
title: Configuración de conversiones de Facebook sin conexión
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
TQID: https://experienceleague.adobe.com/p5G-mS4yYAv-TvloYNSl52-IpEhQl8UuQwBN4M5KA2U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 321
ht-degree: 5%

---

# Configurar [!DNL Facebook] conversiones sin conexión {#set-up-facebook-offline-conversions}

Al enviar los datos de conversión sin conexión de vuelta a [!DNL Facebook] para las personas creadas mediante anuncios de posibles clientes, su equipo de publicidad puede optimizar el gasto de su publicidad mejor que nunca. Siga estos pasos para configurarlo.

>[!PREREQUISITES]
>
>Debe [configurar anuncios de clientes potenciales de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).

## Configuración de administración {#admin-configuration}

1. Vaya a Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vaya a **[!UICONTROL LaunchPoint]** y haga doble clic en el servicio de anuncios de posibles clientes de Facebook que creó anteriormente.

   >[!NOTE]
   >
   >Si aún no lo has hecho, continúa y [configura [!UICONTROL anuncios de clientes potenciales de Facebook]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), y vuelve aquí.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si lo desea, edite el **[!UICONTROL Nombre para mostrar]** para incluir las conversiones sin conexión. Haga clic en **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Marque **[!UICONTROL Habilitar conversiones sin conexión]** y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Haga clic en **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Ha completado la mitad del proceso al habilitar [!DNL Facebook] conversiones sin conexión. Continúe con el Modeler del ciclo de ingresos para asignar las fases.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuración de Modeler del ciclo de ingresos {#revenue-cycle-modeler-configuration}

1. Ir a **[!UICONTROL Analytics]**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Seleccione el modelo y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Actualmente, hay 10 eventos [!DNL Facebook] a los cuales puede asignar etapas de ciclo de ingresos:
   >
   >* Adiciones de información de pago
   >* Agrega al carro
   >* Añade a la lista de deseos
   >* Registros completados
   >* Cierres de compra iniciados
   >* Persona
   >* Otro
   >* Comprar
   >* Búsquedas
   >* Vistas del contenido

1. Seleccione el escenario que desee asignar y, a continuación, en el menú desplegable **[!UICONTROL Conversión de Facebook]**, seleccione el evento [!DNL Facebook] al que desee asignarlo. Repita este paso para asignar todas las fases del equipo a las fases de conversión sin conexión en [!DNL Facebook].

   ![](assets/1-1.png)

1. Cuando haya terminado de asignar, cierre el modelo.

   ![](assets/2.png)

1. Apruebe el modelo y habrá terminado.

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ahora, cuando los posibles clientes de Lead Ad alcancen las fases que ha asignado, las conversiones se enviarán a [!DNL Facebook] para sistema de informes.

   >[!CAUTION]
   >
   >Compruebe su cuenta de [!DNL Facebook] y asegúrese de que todos los [anuncios están asociados](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&cmsid&creative=link&creative_detail=advertiser-help-center&create_type&destination_cms_id&orig_http_referrer) al conjunto de eventos de conversiones sin conexión de Marketo. Si no es así, es posible que la atribución de publicidad no funcione.

   >[!NOTE]
   >
   >Los datos de conversión sin conexión se envían de Marketo a [!DNL Facebook] varias veces al día.

>[!MORELIKETHIS]
>
>[Explicación de [!DNL Facebook] conversiones sin conexión](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
