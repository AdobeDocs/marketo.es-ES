---
description: 'Configuración de acciones MSI en Salesforce: Marketo Docs: documentación del producto'
title: Configuración de acciones MSI en Salesforce
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 84e3c4d525c5bde9e3ebd17d2f29ad42578777ff
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# Configuración de acciones MSI en Salesforce {#msi-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Instalar]() o [Actualización]() Paquete de perspectivas de ventas en su instancia de Salesforce Instalar/Actualizar a [Paquete de acciones MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) en su instancia de Salesforce.
>* [Configurar la perspectiva de ventas de Marketo en Salesforce Enterprise/Unlimited]()


## Agregar nuevo sitio remoto en Salesforce {#add-new-remote-site-in-salesforce}

1. En Salesforce, haga clic en **Configuración**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Busque &quot;sitio remoto&quot; y seleccione **Configuración del sitio remoto**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Haga clic en **Nuevo sitio remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Introduzca el Nombre del sitio remoto (puede ser algo así como &quot;MarketoSalesInsight&quot;). Introduzca la dirección URL del sitio remoto (https://ims-na1-stg1.adobelogin.com) y haga clic en **Guardar**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## Habilitar MSI-Actions en CRM {#enabling-msi-actions-across-the-crm}

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
