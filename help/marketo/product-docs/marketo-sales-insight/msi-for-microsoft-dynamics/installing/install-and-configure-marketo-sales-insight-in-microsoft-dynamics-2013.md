---
unique-page-id: 3571737
description: 'Instalación y configuración de Marketo Sales Insight en Microsoft Dynamics 2013: documentos de Marketo: documentación del producto'
title: Instalar y configurar Marketo Sales Insight en Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 4%

---

# Instalar y configurar [!DNL Marketo Sales Insight] en [!DNL Microsoft Dynamics 2013] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] es una herramienta fantástica para ofrecer a su equipo de ventas una &quot;ventana&quot; sobre la gran cantidad de datos que tiene el equipo de marketing. A continuación se muestra cómo instalarlo y configurarlo.

>[!PREREQUISITES]
>
>Complete la integración de Marketo y Microsoft.
>
>[Descargue la solución correcta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para su versión de [!DNL Microsoft Dynamics] CRM.

## Importar solución {#import-solution}

Bien, ahora es el momento de importar la solución [!DNL Marketo Sales Insight] en [!DNL Microsoft Dynamics].

1. En **[!UICONTROL Microsoft Dynamics CRM]**, haga clic en **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Personalizaciones]**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Haga clic en **[!UICONTROL Soluciones]**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Ya debería haber instalado y configurado Marketo antes de continuar

1. Haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. En la nueva ventana, haz clic en **[!UICONTROL Examinar]**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Busque y seleccione la solución que descargó anteriormente.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Se cargará la solución. Si lo desea, puede ver el contenido del paquete. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Asegúrese de dejar la casilla marcada y haga clic en **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. No dude en descargar el archivo de registro. Haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. ¡Fantástico! Debería ver la solución ahora. Si no está allí, actualice la pantalla.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Conectar Marketo y Sales Insight {#connect-marketo-and-sales-insight}

Vinculemos su instancia de Marketo a [!DNL Sales Insight] en [!DNL Dynamics].

>[!NOTE]
>
>Se requieren derechos de administrador.

1. Inicie sesión en Marketo y vaya a la sección **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. En la sección **[!UICONTROL Sales Insight]**, haga clic en **[!UICONTROL Editar configuración de API]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** y **[!UICONTROL API User Id]** para usarlos en un paso posterior. Escribe una **[!UICONTROL clave secreta de API]** de tu elección y haz clic en **[!UICONTROL Guardar]**.

   >[!CAUTION]
   >
   >No use el signo &amp; en la clave secreta de la API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Los campos siguientes se deben sincronizar con Marketo para que _tanto el posible cliente como el contacto_ funcionen para Sales Insight:
   >
   >* Prioridad
   >* Urgencia
   >* Puntaje relativo
   >
   >Si falta alguno de estos campos, verá un mensaje de error en Marketo con el nombre de los campos que faltan. Para solucionarlo, realice [este procedimiento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. En [!DNL Microsoft Dynamics], ve a **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Configuración de la API de Marketo]**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Haga clic en **[!UICONTROL Nuevo]**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Escriba la información que tomó de Marketo anteriormente y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Definir acceso de usuario {#set-user-access}

Por último, puede otorgar acceso a [!DNL Marketo Sales Insight] a usuarios concretos.

1. Vaya a **[!UICONTROL Configuración]**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Haga clic en **[!UICONTROL Usuarios]**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Seleccione a los usuarios a los que desea otorgar acceso a Sales Insight y haga clic en **[!UICONTROL Administrar roles]**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Seleccione el rol de **[!UICONTROL Marketo Sales Insight]** y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   ¡Y tú deberías haber terminado! Por último, para realizar pruebas, inicie sesión en [!DNL Dynamics] como usuario que tiene acceso a [!DNL Marketo Sales Insight] y observe a un posible cliente o contacto.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Ahora ha desbloqueado el poder de [!DNL Marketo Sales Insight] para su equipo de ventas.

>[!MORELIKETHIS]
>
>[Configuración de estrellas y llamas para registros de contactos o posibles clientes](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
