---
unique-page-id: 10098625
description: Información sobre Microsoft Dynamics Sync - Marketo Docs - Documentación del producto
title: Información sobre Microsoft Dynamics Sync
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 80651a7d3d416f27ef13184b11757943c98bd781
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 1%

---

# Información sobre Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo y Microsoft Dynamics van juntos. Mantenemos sus datos de ventas y marketing sincronizados.

>[!NOTE]
>
>Marketo solo admite certificados SSL compatibles con Java 7 en este momento.

>[!CAUTION]
>
>Actualmente no se admite la actualización de entornos limitados para Marketo Dynamics Sync. Si necesita actualizar el simulador para pruebas de Dynamics CRM, se necesitará un nuevo simulador para pruebas de Marketo. Póngase en contacto con el administrador de éxito de los clientes para obtener más información.

## Cómo funciona la sincronización {#how-sync-works}

Marketo sincroniza datos continuamente con Microsoft Dynamics todo el día, todos los días. Se realiza mediante sincronización de fondo, en lotes, no en tiempo real.

>[!NOTE]
>
>La primera sincronización de la suscripción tarda de minutos a horas, según el tamaño de la base de datos. Marketo copia toda la base de datos desde Dynamics. Después, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

La sincronización entre Marketo y Dynamics es bidireccional para posibles clientes y contactos. Si realiza cambios en Marketo o Dynamics, las actualizaciones se reflejarán en ambos sistemas. Todos los demás campos, como cuentas y oportunidades, se sincronizan de una sola manera, de Dynamics a Marketo.

## ¿Qué se sincroniza entre Marketo y Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contactos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Cuentas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuarios](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipos (grupos de usuarios del sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

Las [credenciales introducidas en Marketo para Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) se utilizan para sincronizar los datos.

>[!NOTE]
>
>La copia de instancia no es compatible si la instancia de origen está integrada con Microsoft Dynamics.
