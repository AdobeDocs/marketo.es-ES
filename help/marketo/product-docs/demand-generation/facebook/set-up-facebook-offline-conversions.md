---
unique-page-id: 11383953
description: 'Configuración de conversiones sin conexión de Facebook: documentos de Marketo, documentación del producto'
title: Configurar conversiones sin conexión de Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Configurar conversiones sin conexión de Facebook {#set-up-facebook-offline-conversions}

Al enviar datos de conversión sin conexión de vuelta a Facebook para las personas creadas mediante anuncios de posibles clientes, su equipo de publicidad puede optimizar su gasto en publicidad mejor que nunca. A continuación se muestra cómo configurarlo.

>[!PREREQUISITES]
>
>* Usted debe [Configurar anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Debe tener un modelo aprobado en [Modelador del ciclo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Configuración de administración {#admin-configuration}

1. Ir a Marketo **Administrador**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Ir a **LaunchPoint** y haga doble clic en el servicio Facebook Lead Ads que creó anteriormente.

   >[!NOTE]
   >
   >Si no lo has hecho, adelante y... [Configurar anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)Entonces, vuelve aquí.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si lo desea, edite el **Nombre para mostrar** para incluir las conversiones sin conexión. Clic **Siguiente**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Marque **Habilitar conversiones sin conexión** y haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Clic **Siguiente**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Clic **Guardar**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   ¡Dulce! Ya ha completado la mitad de la operación para habilitar las conversiones sin conexión de Facebook. Vamos a saltar al Modelador del ciclo de ingresos para asignar las etapas.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuración del Modelador del ciclo de ingresos {#revenue-cycle-modeler-configuration}

1. Ir a **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Seleccione el modelo y haga clic en **Editar borrador**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Actualmente, hay 10 eventos de Facebook a los que puede asignar etapas del ciclo de ingresos:
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
   >* Vistas de contenido

1. Seleccione el escenario que desee asignar y, a continuación, en el **Conversión de facebook** , seleccione el Evento de Facebook al que desee asignarlo. Repita este paso para asignar todas las fases del RCM a fases de conversión sin conexión en Facebook.

   ![](assets/1-1.png)

1. Cuando haya terminado de asignar, cierre el modelo.

   ![](assets/2.png)

1. ¡Apruebe su modelo y ha terminado!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ahora, cuando los posibles clientes de Lead Ad alcanzan las fases asignadas, las conversiones se envían a Facebook para sistema de informes.

   >[!CAUTION]
   >
   >Compruebe su cuenta de Facebook y asegúrese de que todas las [los anuncios están asociados](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) al conjunto de eventos de conversiones sin conexión de Marketo. Si no es así, es posible que la atribución de publicidad no funcione.

   >[!NOTE]
   >
   >Los datos de conversión sin conexión se envían de Marketo a Facebook varias veces al día.

>[!MORELIKETHIS]
>
>[Explicación de las conversiones sin conexión Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
