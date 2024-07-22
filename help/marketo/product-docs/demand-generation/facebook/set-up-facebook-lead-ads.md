---
unique-page-id: 11379622
description: 'Configuración de anuncios de posibles clientes de Facebook: documentos de Marketo, documentación del producto'
title: Configurar anuncios de posibles clientes de Facebook
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Configurar anuncios de posibles clientes de Facebook {#set-up-facebook-lead-ads}

Use [Facebook Lead Ads](https://www.facebook.com/business/a/lead-ads) para ejecutar campañas publicitarias en Facebook y generar posibles clientes para Marketo.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!AVAILABILITY]
>
>Para que Facebook Lead Ads se añada a su instancia, póngase en contacto con el equipo de la cuenta de Adobe (su administrador de cuentas).

1. Vaya a Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vaya a **LaunchPoint**, haga clic en **Nuevo,** y seleccione **Nuevo servicio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Escriba un **Nombre para mostrar** para su servicio, seleccione el servicio **Facebook Lead Ads** en la lista desplegable y haga clic en **Crear**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Abra una ficha nueva en el mismo explorador y vaya a [facebook.com](https://www.facebook.com). Inicie sesión en Facebook con la cuenta que desee utilizar para la integración.

   >[!NOTE]
   >
   >La cuenta de Facebook necesitará acceso a todas las páginas comerciales de Facebook desde las que desee extraer anuncios potenciales.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Cuando haya iniciado sesión en Facebook, vuelva a Marketo y haga clic en **Autorizar**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Si se le solicita, haga clic en **Aceptar** para aceptar la instalación de la aplicación Marketo en Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Verá que ahora está autorizado. Haga clic en **Siguiente**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Seleccione las páginas de las que quiera que Marketo extraiga anuncios de Facebook Lead y haga clic en **Siguiente**.

   >[!TIP]
   >
   >Si no ve una página que esté esperando, asegúrese de que la cuenta de Facebook utilizada para autenticarse se añada a la página en Facebook e inténtelo de nuevo.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Para aceptar las asignaciones de campo predeterminadas de Facebook a Marketo, simplemente haga clic en **Crear**.

   >[!TIP]
   >
   >Al modificar las asignaciones, puede personalizar dónde se almacenan los datos de los anuncios potenciales en Marketo. También puede [extraer datos de las preguntas personalizadas de los anuncios de posibles clientes](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo no admite la asignación de dos campos Facebook a un único campo Marketo, solo de 1 a 1. Si asigna 2 a 1, es posible que los posibles clientes no entren en el sistema Marketo.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   ¡Bien hecho! Los posibles clientes empezarán a fluir a Marketo a medida que ejecute campañas de publicidad de posibles clientes de Facebook con éxito.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Asignar o quitar permisos en el Administrador de acceso de posibles clientes (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Usar filtros y Déclencheur de anuncios de posibles clientes en una campaña inteligente](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Asignar campos personalizados a Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)
