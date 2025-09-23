---
unique-page-id: 11383953
description: 'Configuración de conversiones sin conexión de Facebook: documentos de Marketo: documentación del producto'
title: Configuración de conversiones de Facebook sin conexión
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 4%

---

# Configurar [!DNL Facebook] conversiones sin conexión {#set-up-facebook-offline-conversions}

Al enviar los datos de conversión sin conexión de vuelta a [!DNL Facebook] para las personas creadas mediante anuncios de posibles clientes, su equipo de publicidad puede optimizar el gasto de su publicidad mejor que nunca. A continuación se muestra cómo configurarlo.

>[!PREREQUISITES]
>
>* Debe [configurar anuncios de clientes potenciales de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Debe tener un modelo aprobado en [Modeler del ciclo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Configuración de administración {#admin-configuration}

1. Vaya a Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vaya a **[!UICONTROL LaunchPoint]** y haga doble clic en el servicio de anuncios de posibles clientes de Facebook que creó anteriormente.

   >[!NOTE]
   >
   >Si aún no lo has hecho, continúa y [configura [!UICONTROL anuncios de clientes potenciales de Facebook]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), y vuelve aquí.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si lo desea, edite el **[!UICONTROL Nombre para mostrar]** para incluir las conversiones sin conexión. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Marque **[!UICONTROL Habilitar conversiones sin conexión]** y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   ¡Dulce! Ya ha completado la mitad del proceso para habilitar [!DNL Facebook] conversiones sin conexión. Vamos a saltar a la Modeler del ciclo de ingresos para asignar las fases.

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

1. ¡Apruebe su modelo y ha terminado!

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
