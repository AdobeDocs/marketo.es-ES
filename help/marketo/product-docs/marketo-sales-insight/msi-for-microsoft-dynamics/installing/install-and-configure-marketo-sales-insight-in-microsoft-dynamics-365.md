---
unique-page-id: 3571739
description: Instalación y configuración de Marketingto Sales Insight en Microsoft Dynamics 365 - Documentos de marketing - Documentación del producto
title: Instalación y configuración de Marketingto Sales Insight en Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Instalar y configurar Marketingto Sales Insight en Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

La perspectiva de ventas de marketing es una herramienta fantástica para dar a su equipo de ventas una &quot;ventana&quot; a la abundancia de datos que posee el equipo de mercadotecnia. A continuación se explica cómo instalar y configurar.

>[!PREREQUISITES]
>
>Complete la integración de Marketing con Microsoft.
>
>[Descargue la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) solución correcta para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

1. Inicie sesión en [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Haga clic en el menú ![—](assets/image2015-3-16-16-1-13.png) y seleccione **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Haga clic en el menú ![—](assets/image2015-5-13-10-5-8.png). En la lista desplegable, seleccione **Configuración** y, a continuación, seleccione **Soluciones**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Ya debería haber [instalado y configurado la solución de Marketing](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) antes de avanzar.

1. Haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. En la nueva ventana, haga clic en **Examinar**. Elija la [solución de perspectiva de ventas de marketing que descargó en el paso 1](#msi). Haga clic en **Siguiente**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Se cargará la solución. Puede vista del contenido del paquete si lo desea. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Asegúrese de dejar la casilla **marcada** y haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. No dude en descargar el archivo de registro. Haga clic en **Cerrar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. ¡Increíble! Deberías ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Haga clic en **Publicar todas las personalizaciones**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketing y perspectiva de ventas {#connect-marketo-and-sales-insight}

Vinculemos la instancia de Marketing a Sales Insight en Dynamics. Así es como:

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en Marketing y vaya a la sección **Administración**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección **Perspectiva de ventas**, haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie el **host de marketing**, **URL de API** y **ID de usuario de API** para usarlos en un paso posterior. Escriba una **Clave secreta de API** de su elección y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No utilice un símbolo &amp; en la clave secreta de API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Los siguientes campos deben sincronizarse con Marketing para _Posible cliente y Contacto_ para que Sales Insight funcione:
   >
   > * Prioridad
   > * Urgencia
   > * Puntuación relativa

   >
   >Si falta alguno de estos campos, verá un mensaje de error en el menú de marketing con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De nuevo en Microsoft Dynamics, haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19.png) junto a Configuración y, a continuación, seleccione **Configuración de API de marketing** en la lista desplegable.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Haga clic en **Configuración predeterminada**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Introduzca la información que ha copiado de Marketing anteriormente.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Haga clic en el icono ![](assets/image2015-5-13-16-3a8-3a51.png) en la esquina inferior derecha para guardar los cambios.

## Establecer acceso de usuario {#set-user-access}

Debe otorgar a los usuarios permisos para utilizar Sales Insight.

1. Haga clic en el menú ![](assets/image2015-5-13-10-3a5-3a8.png). En el menú desplegable, seleccione **Configuración** y, a continuación, seleccione **Seguridad**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Seleccione los usuarios a los que desea dar acceso a Sales Insight y haga clic en **Administrar funciones**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Seleccione la función **Marketing to Sales Insight** y haga clic en **Aceptar**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   ¡Y todos ustedes deberían terminar! Finalmente, para realizar pruebas, inicie sesión en Dynamics como un usuario que tiene acceso a Marketing Cloud Sales Insight y vea un posible cliente o contacto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ahora ha desbloqueado la potencia de la perspectiva de ventas de marketing para su equipo de ventas.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contacto/posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
