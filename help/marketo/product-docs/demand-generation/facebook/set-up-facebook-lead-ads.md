---
unique-page-id: 11379622
description: Configuración de Facebook Lead Ads - Marketo Docs - Documentación del producto
title: Configuración de anuncios de posibles clientes de Facebook
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Configuración de anuncios de posibles clientes de Facebook {#set-up-facebook-lead-ads}

Uso [Anuncios de posible cliente de facebook](https://www.facebook.com/business/a/lead-ads) para ejecutar campañas publicitarias en Facebook y generar posibles clientes para Marketo.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!AVAILABILITY]
>
>Para que se añadan los anuncios de posibles clientes de Facebook a su instancia, póngase en contacto con el administrador de éxito de los clientes.

1. Vaya a Marketo **Administrador**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vaya a **LaunchPoint**, haga clic en **Nuevo,** y seleccione **Nuevo servicio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Escriba un **Nombre para mostrar** para el servicio, seleccione la opción **Anuncios de posible cliente de facebook** del menú desplegable y haga clic en **Crear**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Abra una nueva pestaña en el mismo explorador y vaya a [facebook.com](https://www.facebook.com). Inicie sesión en Facebook con la cuenta que desee utilizar para la integración.

   >[!NOTE]
   >
   >La cuenta de Facebook necesitará acceder a todas las páginas de negocio de Facebook de las que desee extraer los anuncios de posibles clientes.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Una vez que haya iniciado sesión en Facebook, vuelva a Marketo y haga clic en **Autorizar**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Si se le solicita, haga clic en **OK** para aceptar la instalación de la aplicación de Marketo en Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Verá que ahora está autorizado. Haga clic en **Siguiente**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Seleccione las páginas desde las que desea que Marketo extraiga los anuncios de posibles clientes de Facebook y haga clic en **Siguiente**.

   >[!TIP]
   >
   >Si no ve la página que espera, asegúrese de que la cuenta de Facebook utilizada para autenticarse se agrega a la página en Facebook y vuelva a intentarlo.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Para aceptar las asignaciones de campo predeterminadas de Facebook a Marketo, simplemente haga clic en **Crear**.

   >[!TIP]
   >
   >Al modificar las asignaciones, puede personalizar dónde se almacenan los datos de los posibles clientes en Marketo. También puede [extraer datos de las preguntas personalizadas de posibles clientes](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo no admite la asignación de dos campos de Facebook a un único campo de Marketo, solo de 1 a 1. Si asigna 2 a 1, es posible que los posibles clientes no entren en el sistema Marketo.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   ¡Bien hecho! Los posibles clientes empezarán a fluir a Marketo a medida que ejecute campañas de anuncios de posibles clientes de Facebook con éxito.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Asignación/eliminación de permisos en el administrador de acceso de posibles clientes (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Uso de filtros y Déclencheur de anuncios de posibles clientes en una campaña inteligente](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Asignación de campos personalizados a Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)

