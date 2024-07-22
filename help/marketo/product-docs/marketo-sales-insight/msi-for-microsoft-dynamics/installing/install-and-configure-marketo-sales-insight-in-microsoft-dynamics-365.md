---
unique-page-id: 3571739
description: 'Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 365: documentos de Marketo: documentación del producto'
title: Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 1%

---

# Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight es una herramienta fantástica para ofrecer a su equipo de ventas una &quot;ventana&quot; sobre la gran cantidad de datos que tiene el equipo de marketing. Así se instala y configura.

>[!PREREQUISITES]
>
>Complete la integración de Marketo y Microsoft.
>
>[Descargue la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de Microsoft Dynamics CRM.

## Importar solución {#import-solution}

1. Inicie sesión en [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Haga clic en el menú ![—](assets/image2015-3-16-16-1-13.png) y seleccione **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Haga clic en el menú ![—](assets/image2015-5-13-10-5-8.png). En la lista desplegable, seleccione **Configuración** y, a continuación, seleccione **Soluciones**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Ya debería tener [instalada y configurada la solución Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) antes de continuar.

1. Haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. En la nueva ventana, haz clic en **Examinar**. Elija la solución [Marketo Sales Insight que descargó en el paso 1](#msi). Haga clic en **Siguiente**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Se cargará la solución. Si lo desea, puede ver el contenido del paquete. Haga clic en **Siguiente**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Asegúrese de dejar la casilla **marcada** y haga clic en **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. No dude en descargar el archivo de registro. Haga clic en **Cerrar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. ¡Fantástico! Debería ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Haga clic en **Publish All Customization**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Conectar Marketo y perspectivas de ventas {#connect-marketo-and-sales-insight}

Vinculemos su instancia de Marketo al conocimiento de ventas en Dynamics. A continuación se muestra cómo:

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en Marketo y vaya a la sección **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección **Perspectiva de ventas**, haga clic en **Editar configuración de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie el **host de Marketo**, la **URL de la API** y el **ID de usuario de la API** para usarlos en un paso posterior. Escribe una **clave secreta de API** de tu elección y haz clic en **Guardar**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Los campos siguientes se deben sincronizar con Marketo para que _el posible cliente y el contacto_ funcionen con la perspectiva de ventas:
   >
   > * Prioridad
   > * Urgencia
   > * Puntaje relativo
   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De nuevo en Microsoft Dynamics, haga clic en el icono ![](assets/image2015-5-13-15-3a49-3a19.png) junto a Configuración y, a continuación, seleccione **Configuración de la API de Marketo** en el menú desplegable.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Haga clic en **Configuración predeterminada**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Introduzca la información que copió de Marketo anteriormente.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Haga clic en el icono ![](assets/image2015-5-13-16-3a8-3a51.png) en la esquina inferior derecha para guardar los cambios.

## Definir acceso de usuario {#set-user-access}

Debe conceder permisos a los usuarios para que utilicen la perspectiva de ventas.

1. Haga clic en el menú ![](assets/image2015-5-13-10-3a5-3a8.png). En el menú desplegable, seleccione **Configuración** y, a continuación, seleccione **Seguridad**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Haga clic en **Usuarios**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Seleccione a los usuarios a los que desea otorgar acceso a Información sobre ventas y haga clic en **Administrar roles**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Seleccione el rol **Marketo Sales Insight** y haga clic en **Aceptar**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   ¡Y tú deberías haber terminado! Por último, para realizar pruebas, inicie sesión en Dynamics como un usuario que tiene acceso a Marketo Sales Insight y observe a un posible cliente o contacto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ahora ha desbloqueado el poder de Marketo Sales Insight para su equipo de ventas.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contactos o posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
