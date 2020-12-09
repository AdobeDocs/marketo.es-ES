---
unique-page-id: 11383953
description: Configurar conversiones sin conexión de Facebook - Documentos de marketing - Documentación del producto
title: Configurar conversiones sin conexión de Facebook
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Configurar conversiones sin conexión de Facebook {#set-up-facebook-offline-conversions}

Al enviar datos de conversión sin conexión de vuelta a Facebook para las personas creadas mediante Lead Ads, su equipo de publicidad puede optimizar su inversión en publicidad mejor que nunca. Así es como configurarlo.

>[!PREREQUISITES]
>
>* Debe [configurar las Publicidades de posibles clientes](set-up-facebook-lead-ads.md)de Facebook.
>* Debe tener un modelo aprobado en el [módulo de ciclo de ingresos](http://docs.marketo.com/display/docs/revenue+cycle+models).

>



## Configuración del administrador {#admin-configuration}

1. Vaya a Administrador **de marketing**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vaya a **LaunchPoint** y haga clic con el doble en el servicio Publicidades de posibles clientes de Facebook que creó anteriormente.

   >[!NOTE]
   >
   >Si no lo has hecho, sigue adelante y [configura los anuncios](set-up-facebook-lead-ads.md)de posibles clientes de Facebook, y vuelve aquí.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si lo desea, edite el **Nombre** para mostrar para incluir Conversiones sin conexión. Haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Marque **Habilitar conversiones** sin conexión y haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Haga clic en **Guardar**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   ¡Dulce! Ha terminado de habilitar las conversiones sin conexión de Facebook. Pasemos al módulo de ciclo de ingresos para asignar las etapas.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuración del modelo de ciclo de ingresos {#revenue-cycle-modeler-configuration}

1. Vaya a **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Seleccione el modelo y haga clic en **Editar borrador**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Actualmente, hay 10 eventos de Facebook que puede asignar a las siguientes etapas del ciclo de ingresos:
   >
   >    
   >    
   >    * Añadas de información de pago
   >    * Añade al carro
   >    * Añade a la Lista de deseo
   >    * Registros completados
   >    * Cierres de compras iniciados
   >    * Persona
   >    * Otros
   >    * Compra
   >    * Búsquedas
   >    * Vistas de contenido


1. Seleccione el escenario al que desee asignar y, en la lista desplegable Conversión **de** Facebook, seleccione el Evento de Facebook al que desee asignarlo. Repita este paso para asignar todas las etapas del RCM a las etapas de conversión sin conexión en Facebook.

   ![](assets/1-1.png)

1. Cuando haya terminado la asignación, cierre el modelo.

   ![](assets/2.png)

1. Apruebe su modelo y ya ha terminado.

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ahora, cuando los leads en publicidad de posibles clientes alcanzan las etapas asignadas, las conversiones se envían a Facebook para su sistema de informes.

   >[!CAUTION]
   >
   >Compruebe su cuenta de Facebook y asegúrese de que todas [las publicidades están asociadas](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) al conjunto de Eventos de conversiones sin conexión de Marketing a sin conexión. Si no lo son, la atribución de publicidad puede no funcionar.

   >[!NOTE]
   >
   >Los datos de conversión sin conexión se envían de Marketing a Facebook varias veces al día.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Explicación de las conversiones sin conexión de Facebook](understanding-facebook-offline-conversions.md)

>



