---
unique-page-id: 3571735
description: 'Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2011: documentos de Marketo: documentación del producto'
title: Instalar y configurar Marketo Sales Insight en Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 4%

---

# Instalar y configurar [!DNL Marketo Sales Insight] en [!DNL Microsoft Dynamics 2011] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] es una herramienta fantástica para su equipo de ventas. Esta es la instrucción paso a paso de cómo instalarla y configurarla en [!DNL Microsoft Dynamics 2011] local.

>[!PREREQUISITES]
>
>Complete la integración de Marketo y Microsoft.
>
>[Descargue la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de [!DNL Microsoft Dynamics] CRM.

## Importar solución {#import-solution}

1. Iniciar sesión en [!DNL Microsoft Dynamics] CRM. Haga clic en **[!UICONTROL Configuración]** en el menú inferior izquierdo.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleccione **[!UICONTROL Soluciones]** en el árbol.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Haga clic en **Importar** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Ya debería tener [instalada y configurada](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la solución de Marketo antes de continuar.

1. Haga clic en **[!UICONTROL Examinar]**. Seleccione la solución [!DNL Marketo Sales Insight] que [descargó](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Compruebe los detalles de la solución y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Asegúrese de que la opción SDK message esté seleccionada. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Ahora espere a que finalice la importación.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight] aparecerá ahora en la lista de soluciones. ¡Yay!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Seleccione [!DNL Marketo Sales Insight] y haga clic en **Publicar todas las personalizaciones** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Conectar Marketo y Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Inicie sesión en Marketo y haga clic en **[!UICONTROL Administrador]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección **[!UICONTROL Sales Insight]**, haga clic en **[!UICONTROL Editar configuración de API]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** y **[!UICONTROL API User Id]** para usarlos en un paso posterior. Escribe una **[!UICONTROL clave secreta de API]** de tu elección y haz clic en **[!UICONTROL Guardar]**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Los campos siguientes se deben sincronizar con Marketo para que _tanto el posible cliente como el contacto_ funcionen para Sales Insight:
   >
   >* Prioridad
   >* Urgencia
   >* Puntaje relativo
   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Vuelva a Dynamics y seleccione **[!UICONTROL Configuración]**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleccione **[!UICONTROL Configuración de la API de Marketo]** en el árbol.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Haga clic en **[!UICONTROL Configuración predeterminada]**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Escriba la información que tomó de Marketo anteriormente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Definir acceso de usuario {#set-user-access}

Configure los roles de usuario para que determinados usuarios tengan acceso a [!DNL Sales Insight].

1. Seleccione **[!UICONTROL Configuración]**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Seleccione **[!UICONTROL Administración]** en el árbol.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Haga clic en **[!UICONTROL Usuarios]**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Seleccione a los usuarios a los que desea conceder acceso y haga clic en **[!UICONTROL Administrar roles]**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Seleccione el rol de **[!UICONTROL Marketo Sales Insight]** y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   ¡Y eso es todo! Todos los usuarios que tengan acceso ahora podrán ver la sección de insight de ventas en la vista de detalles del posible cliente/contacto.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Enhorabuena. Ahora ha liberado el poder de [!DNL Marketo Sales Insight].

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contactos o posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
