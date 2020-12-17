---
unique-page-id: 3571735
description: Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2011 - Documentos de marketing - Documentación del producto
title: Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2011
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

La perspectiva de ventas de marketing es una herramienta fantástica para su equipo de ventas. Esta es la instrucción paso a paso de cómo instalarla y configurarla en locales de Microsoft Dynamics 2011.

>[!PREREQUISITES]
>
>Complete la integración [de Marketing a Microsoft](http://docs.marketo.com/x/DoA2).
>
>[Descargue la ](http://docs.marketo.com/x/LoJo) solución correcta para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

1. Inicie sesión en Microsoft Dynamics CRM. Haga clic en **Configuración** en el menú inferior izquierdo.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleccione **Soluciones** en el árbol.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Haga clic en **Importar** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Ya debe tener [instalado y configurado](install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la solución de Marketing para avanzar.

1. Haga clic en **Examinar**. Seleccione la solución de perspectiva de ventas de marketing que [descargó](download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Haga clic en **Siguiente**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Compruebe los detalles de la solución y haga clic en **Siguiente**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Asegúrese de que la opción de mensaje SDK está marcada. Haga clic en **Siguiente**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Ahora espere a que finalice la importación.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Haga clic en **Cerrar**.

   ![](assets/crmhand.png)

1. La perspectiva de ventas de marketing ahora se mostrará en la lista de la solución. ¡Sí!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Seleccione Marketing to Sales Insight y haga clic en **Publicar todas las personalizaciones** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketing y perspectiva de ventas {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en Marketing y haga clic en **Administración**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección **Perspectiva de ventas **haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie el **host de marketing**, **URL de API** y el **ID de usuario de API** para usarlos en un paso posterior. Escriba una **Clave secreta de API** de su elección y haga clic en **GUARDAR**.

   >[!CAUTION]
   >
   >No utilice un símbolo &amp; en la clave secreta de API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Los siguientes campos deben sincronizarse con Marketing para *Posible cliente y Contacto* para que Sales Insight funcione:
   >
   >    
   >    
   >    * Prioridad
   >    * Urgencia
   >    * Puntuación relativa

   >    
   >    
   >Si falta alguno de estos campos, verá un mensaje de error en el menú de marketing con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Vuelva a Dynamics, seleccione **Configuración**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleccione **Configuración de API de marketing** en el árbol.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Haga clic en **Configuración predeterminada**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Escriba la información que tomó de Marketing anteriormente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Haga clic en **Guardar.**

   ** ![](assets/image2015-5-4-11-3a28-3a13.png)

   **

## Establecer acceso de usuario {#set-user-access}

Configure las funciones de usuario para que los usuarios específicos tengan acceso a la perspectiva de ventas.

1. Seleccione **Configuración**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Seleccione **Administración** en el árbol.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Seleccione los usuarios a los que desea otorgar acceso y haga clic en **Administrar funciones**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Seleccione la función **Marketing to Sales Insight** y haga clic en **Aceptar**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   ¡Y eso es todo! Ahora todos los usuarios tendrán acceso a la sección de perspectiva de ventas de la vista de detalles de contacto/posible cliente.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Felicidades. Ahora ha desatado la potencia de Marketingto Sales Insight.

>[!NOTE]
>
>**Artículos relacionados**
>
>[Configuración de estrellas y llamas para registros de contacto/posibles clientes](http://docs.marketo.com/x/BICMAg)

