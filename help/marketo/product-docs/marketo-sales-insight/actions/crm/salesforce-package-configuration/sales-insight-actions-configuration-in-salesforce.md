---
description: Configuración de acciones de perspectiva de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Configuración de acciones de perspectiva de ventas en Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# Configuración de acciones de perspectiva de ventas en Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Instalar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) o [actualizar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) paquete de perspectivas de ventas en su instancia de Salesforce
>* [Configuración de Marketo Sales Insight en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Agregar un nuevo sitio remoto en Salesforce {#add-new-remote-site-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoSalesInsight1&quot;). Escriba la dirección URL del sitio remoto `https://ims-na1.adobelogin.com` y haga clic en **Guardar**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Vuelva a hacer clic en **Nuevo sitio remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Introduzca el nombre del sitio remoto (puede ser algo como &quot;MarketoSalesInsight2&quot;). Escriba la dirección URL del sitio remoto `https://mkto-sales-connect.adobe.io` y haga clic en **Guardar**.

## Activación de acciones de perspectiva de ventas en CRM {#enabling-sales-insight-actions-across-the-crm}

1. En Salesforce, haga clic en la ficha **Configuración de Marketo Sales Insight**.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Si no ve &quot;Configuración de Marketo Sales Insight&quot; en la barra superior, haga clic en el signo **+** y búsquelo en Todas las fichas.

1. Seleccione la casilla de verificación **Habilitar acciones MSI**.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Introduzca la clave secreta de la API.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Si no tienes a mano tu clave secreta de la API, puedes encontrarla siguiendo los pasos de [este artículo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Haga clic en **Guardar** cuando termine.

Esto habilitará automáticamente todas las características de acciones MSI descritas en el artículo de información general de características.

>[!NOTE]
>
>Puede desactivar todas las funciones de acciones MSI simplemente desmarcando la casilla &quot;Habilitar acciones MSI&quot;.

## Administración de MSI-Actions {#msi-actions-governance}

1. Puede desactivar las campañas de ventas o la pestaña Tarea en la próxima sección. Esto se aplicará a los paneles de posible cliente, contacto, cuenta y oportunidad.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Puede deshabilitar las acciones MSI si desmarca las características correspondientes en la configuración de acciones.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>La configuración de gobernanza se aplica a todos los usuarios de MSI.
