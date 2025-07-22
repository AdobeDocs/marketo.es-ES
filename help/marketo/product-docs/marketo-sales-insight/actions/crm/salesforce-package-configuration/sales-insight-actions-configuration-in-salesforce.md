---
description: Configuración de acciones de Insight de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Configuración de acciones de Insight de ventas en Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 1%

---

# Configuración de [!DNL Sales Insight Actions] en [!DNL Salesforce] {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Instalar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) o [actualizar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) paquete Sales Insight en su instancia de [!DNL Salesforce]
>* [Configurar Marketo Sales Insight en [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Agregar nuevo sitio remoto en [!DNL Salesforce] {#add-new-remote-site-in-salesforce}

1. En [!DNL Salesforce], haga clic en **[!UICONTROL Configuración]**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Busque &quot;[!UICONTROL sitio remoto]&quot; y seleccione **[!UICONTROL Configuración de sitio remoto]**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Haga clic en **[!UICONTROL Nuevo sitio remoto]**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoSalesInsight1&quot;). Escriba la dirección URL del sitio remoto `https://ims-na1.adobelogin.com` y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Vuelva a hacer clic en **[!UICONTROL Nuevo sitio remoto]**.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoSalesInsight2&quot;). Escriba la dirección URL del sitio remoto `https://mkto-sales-connect.adobe.io` y haga clic en **[!UICONTROL Guardar]**.

## Habilitando [!DNL Sales Insight Actions] en CRM {#enabling-sales-insight-actions-across-the-crm}

1. En [!DNL Salesforce], haga clic en la ficha **[!UICONTROL Configuración de Marketo Sales Insight]**.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Si no ve &quot;[!UICONTROL Configuración de Marketo Sales Insight]&quot; en la barra superior, haga clic en el signo **+** y búsquelo en Todas las fichas.

1. Seleccione la casilla de verificación **[!UICONTROL Habilitar acciones MSI]**.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Escriba la [!UICONTROL clave secreta de la API].

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Si no tienes a mano tu [!UICONTROL clave secreta de la API], puedes encontrarla siguiendo los pasos de [este artículo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.

Esto habilitará automáticamente todas las características de acciones MSI descritas en el artículo de información general de características.

>[!NOTE]
>
>Puede desactivar todas las funciones de acciones MSI simplemente desmarcando la casilla &quot;Habilitar acciones MSI&quot;.

## Administración de MSI-Actions {#msi-actions-governance}

1. Puede desactivar las campañas de ventas o la pestaña Tarea en la próxima sección. Esto se aplicará a los paneles de posible cliente, contacto, cuenta y oportunidad.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Puede deshabilitar las acciones MSI si desmarca las características correspondientes en [!UICONTROL Configuración de acciones].

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>La configuración de gobernanza se aplica a todos los usuarios de MSI.
