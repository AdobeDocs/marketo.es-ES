---
unique-page-id: 37355602
description: Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics Online - Documentos de marketing - Documentación del producto
title: Instalación y configuración de la perspectiva de ventas de marketing en Microsoft Dynamics Online
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# Instalar y configurar MarketingTo Sales Insight en Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

La perspectiva de ventas de marketing es una herramienta fantástica para dar a su equipo de ventas una &quot;ventana&quot; a la abundancia de datos que posee el equipo de mercadotecnia. A continuación se muestra cómo instalarlo y configurarlo en Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Complete la integración de Marketing con Microsoft.
>
>[Descargue la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) solución correcta para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

>[!NOTE]
>
>Si está utilizando la interfaz unificada, antes del Paso 1 a continuación, haga clic en el icono Configuración en la esquina superior derecha y seleccione **Configuración avanzada**.

1. En Microsoft Dynamics CRM, haga clic en **Configuración**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. En Configuración, haga clic en **Personalizaciones**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Haga clic en **Soluciones**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Ya debería haber instalado y configurado la solución de marketing antes de avanzar.

1. Haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. En la nueva ventana, haga clic en **Examinar**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. En el equipo, busque e instale la solución que acaba de descargar.

1. Haga clic en **Siguiente**.

   ![](assets/seven.png)

1. Se cargará la solución. Puede vista del contenido del paquete si lo desea. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Asegúrese de dejar la casilla marcada y haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. No dude en descargar el archivo de registro y haga clic en **Cerrar**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. ¡Increíble! Deberías ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/eleven.png)

1. Haga clic en **Personalización de publicación**.

   >[!NOTE]
   >
   >Asegúrese de habilitar la sincronización de Global MS Dynamics.

## Connect Marketing y perspectiva de ventas {#connect-marketo-and-sales-insight}

Vinculemos la instancia de Marketing a Sales Insight en Dynamics. Así es como:

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en Marketing y vaya a la sección **Administración**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. En la sección Perspectiva de ventas, haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie el **host de marketing**, **URL de API** y el **ID de usuario de API** para usarlos en un paso posterior. Introduzca una clave secreta de API de su elección y haga clic en **Guardar**.

   >[!CAUTION]
   >
   >No utilice un símbolo &amp; en la clave secreta de API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. En **Configuración**, haga clic en **Configuración de API de marketing**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Haga clic en **Nuevo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Escriba la información que tomó de Marketing anteriormente y haga clic en **Guardar**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Habilitar sincronización {#enable-sync}

1. En Marketing, haga clic en **Administración**.

   ![](assets/enable-one.png)

1. En Integración, seleccione **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Haga clic en **Habilitar sincronización**.

   ![](assets/enable-three.png)

1. Haga clic en **Editar** junto a Detalles de sincronización de campos.

   ![](assets/enable-four.png)

1. Esto _automáticamente_ seleccionará los campos MSI que anteriormente estaban deshabilitados (Urgencia, Puntuación relativa y Prioridad). Simplemente haga clic en **Guardar** en para sincronizar datos de inicio.

   ![](assets/enable-five.png)

## Establecer acceso de usuario {#set-user-access}

Por último, tiene que dar acceso a usuarios específicos para utilizar la Perspectiva de ventas de Marketing to.

1. Vaya a **Configuración**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vaya a **Seguridad**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Seleccione los usuarios a los que desea dar acceso a Sales Insight y haga clic en **Administrar funciones**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Seleccione la función de perspectiva de ventas de marketing y haga clic en **Aceptar**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   ¡Y todos ustedes deberían terminar! Finalmente, para realizar pruebas, inicie sesión en Dynamics como un usuario que tiene acceso a Marketing Cloud Sales Insight y vea un posible cliente o contacto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contacto/posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
