---
unique-page-id: 11383953
description: 'Configuración de conversiones sin conexión de Facebook: Documentos de Marketo: Documentación del producto'
title: Configuración de conversiones sin conexión de Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Configuración de conversiones sin conexión de Facebook {#set-up-facebook-offline-conversions}

Al enviar de vuelta los datos de conversión sin conexión a Facebook para las personas creadas mediante anuncios de posibles clientes, su equipo de publicidad puede optimizar su gasto en publicidad mejor que nunca. Así es como configurarlo.

>[!PREREQUISITES]
>
>* Debe [configuración de anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Debe tener un modelo aprobado en [Modelador de ciclo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).


## Configuración de administración {#admin-configuration}

1. Vaya a Marketo **Administrador**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vaya a **LaunchPoint** y haga doble clic en el servicio Facebook Lead Ads que creó anteriormente.

   >[!NOTE]
   >
   >Si no lo has hecho, sigue adelante y [Configuración de anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)y luego vuelve aquí.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si lo desea, edite la **Nombre para mostrar** para incluir las conversiones sin conexión. Haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Marque **Habilitar conversiones sin conexión** y haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Haga clic en **Guardar**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   ¡Dulce! Ya está a medio camino habilitando Conversiones sin conexión de Facebook. Pasemos al modelador de ciclo de ingresos para asignar las etapas.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuración del modelado del ciclo de ingresos {#revenue-cycle-modeler-configuration}

1. Vaya a **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Seleccione el modelo y haga clic en **Editar borrador**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Actualmente, hay 10 eventos de Facebook a los que puede asignar las etapas del ciclo de ingresos:
   >
   >* Adiciones a Información de Pago
   >* Adiciones al carro de compras
   >* Agrega a la lista de deseos
   >* Registros completados
   >* Cierres de compra iniciados
   >* Persona
   >* Otro
   >* Compra
   >* Búsquedas
   >* Vistas del contenido


1. Seleccione el escenario que desee asignar y, a continuación, en el **Conversión de facebook** , seleccione el evento de Facebook al que desea asignarlo. Repita este paso para asignar todas las etapas del RCM a las fases de conversión sin conexión en Facebook.

   ![](assets/1-1.png)

1. Cuando haya terminado de asignar, cierre el modelo.

   ![](assets/2.png)

1. Apruebe su modelo y ya ha terminado!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ahora, cuando los posibles clientes de Lead Ad llegan a las etapas asignadas, las conversiones se envían a Facebook para su informe.

   >[!CAUTION]
   >
   >Compruebe su cuenta de Facebook y asegúrese de que todas las [las publicidades están asociadas](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) al conjunto de eventos de conversiones sin conexión de Marketo. Si no lo son, es posible que la atribución de publicidad no funcione.

   >[!NOTE]
   >
   >Los datos de conversión sin conexión se envían de Marketo a Facebook varias veces al día.

>[!MORELIKETHIS]
>
>[Explicación de las conversiones sin conexión de Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
