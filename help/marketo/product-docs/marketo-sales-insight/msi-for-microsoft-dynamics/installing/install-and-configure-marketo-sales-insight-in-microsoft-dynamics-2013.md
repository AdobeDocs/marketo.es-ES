---
unique-page-id: 3571737
description: Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2013 - Documentos de marketing - Documentación del producto
title: Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2013
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

La perspectiva de ventas de marketing es una herramienta fantástica para dar a su equipo de ventas una &quot;ventana&quot; a la gran cantidad de datos que posee el equipo de mercadotecnia. Así es como instalarlo y configurarlo.

>[!PREREQUISITES]
>
>Complete la integración de Marketing con Microsoft.
>
>[Descargue la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) solución correcta para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

Bien, ahora es el momento de importar la solución de perspectiva de ventas de marketing en Microsoft Dynamics.

1. En **Microsoft Dynamics CRM** haga clic en **Configuración**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. En **Configuración**, haga clic en **Personalizaciones**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Haga clic en **Soluciones**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Ya debería haber instalado y configurado Marketing para avanzar

1. Haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. En la nueva ventana, haga clic en **Examinar**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Busque y seleccione la solución que descargó anteriormente.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Se cargará la solución. Puede vista del contenido del paquete si lo desea. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Asegúrese de dejar la casilla marcada y haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. No dude en descargar el archivo de registro. Haga clic en **Cerrar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. ¡Increíble! Deberías ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketing y perspectiva de ventas {#connect-marketo-and-sales-insight}

Vinculemos la instancia de Marketing a Sales Insight en Dynamics.

>[!NOTE]
>
>Se requieren derechos de administrador.

1. Inicie sesión en Marketing y vaya a la sección **Administración**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección **Perspectiva de ventas** haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie el **host de marketing**, **URL de API** y el **ID de usuario de API** para usarlos en un paso posterior. Escriba una **Clave secreta de API** de su elección y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No utilice un símbolo &amp; en la clave secreta de API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Los siguientes campos deben sincronizarse con Marketing para _Posible cliente y Contacto_ para que Sales Insight funcione:
   >
   >* Prioridad
   >* Urgencia
   >* Puntuación relativa

   >
   >Si falta alguno de estos campos, verá un mensaje de error en el menú de marketing con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De nuevo en Microsoft Dynamics, vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. En **Configuración**, haga clic en **Configuración de API de marketing**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Escriba la información que tomó de Marketing anteriormente y haga clic en **Guardar**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Establecer acceso de usuario {#set-user-access}

Por último, puede proporcionar a usuarios específicos acceso a Marketing to Sales Insight.

1. Vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Seleccione los usuarios a los que desea dar acceso a Sales Insight y haga clic en **Administrar funciones**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Seleccione la función **Marketing to Sales Insight** y haga clic en **Aceptar**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   ¡Y todos ustedes deberían terminar! Por último, para realizar la prueba, inicie sesión en Dynamics como usuario que tiene acceso a Marketing Cloud Sales Insight y observe un posible cliente o contacto.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Ahora ha desbloqueado la potencia de la perspectiva de ventas de marketing para su equipo de ventas.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contacto/posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
