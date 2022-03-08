---
description: Configuración de las acciones de perspectiva de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Configuración de acciones de perspectiva de ventas en Salesforce
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: ba1357e6970ba4e3dc496d27272d067ac87c5e6d
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Configuración de acciones de perspectiva de ventas en Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Instalar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) o [Actualización](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Paquete de perspectivas de ventas en su instancia de Salesforce
>* [Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## Agregar nuevo sitio remoto en Salesforce {#add-new-remote-site-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoSalesInsight&quot;). Introduzca la dirección URL del sitio remoto (https://ims-na1-stg1.adobelogin.com) y haga clic en **Guardar**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## Activación de las acciones de perspectiva de ventas en CRM {#enabling-sales-insight-actions-across-the-crm}

1. En Salesforce, haga clic en la **Configuración de perspectiva de ventas de Marketo** pestaña .

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Si no ve &quot;Marketo Sales Insight Config&quot; en la barra superior, haga clic en el botón **+** marque y busque en Todas las pestañas.

1. Seleccione el **Habilitar acciones MSI** casilla de verificación.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Introduzca la clave secreta de API.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Si no tiene la clave secreta de API a mano, puede encontrarla siguiendo los pasos de [este artículo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Haga clic en **Guardar** cuando haya terminado.

Esto habilitará automáticamente todas las funciones de Acciones MSI descritas en el artículo de descripción general de la función.

>[!NOTE]
>
>Puede desactivar todas las funciones de acciones MSI simplemente desmarcando la casilla de verificación &quot;Habilitar acciones MSI&quot;.

## Administración de MSI-Actions {#msi-actions-governance}

1. Puede desactivar las campañas de ventas o la pestaña Tarea en la sección siguiente. Esto se aplicará a los paneles de posibles clientes, contactos, cuentas y oportunidades.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Puede desactivar las acciones MSI desmarcando las funciones correspondientes en Configuración de acciones .

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>La configuración de administración se aplica a todos los usuarios de MSI.
