---
unique-page-id: 10098625
description: Explicación de Microsoft Dynamics Sync - Documentos de marketing - Documentación del producto
title: Información sobre Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---


# Información sobre Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketing y Microsoft Dynamics van juntos. Mantenemos sus datos de ventas y marketing sincronizados.

>[!NOTE]
>
>Marketing solo admite certificados SSL compatibles con Java 7 en este momento.

## Cómo funciona la sincronización {#how-sync-works}

Marketo sincroniza datos continuamente con Microsoft Dynamics todo el día, todos los días. Se realiza mediante sincronización en segundo plano, en lotes, no en tiempo real.

>[!NOTE]
>
>La primera sincronización de la suscripción tarda de minutos a horas, según el tamaño de la base de datos. Marketo copia toda la base de datos desde Dynamics. Después de eso, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

La sincronización entre Marketing y Dynamics es bidireccional para posibles clientes y contactos. Si realiza cambios en Marketing o Dynamics, las actualizaciones se reflejarán en ambos sistemas. Todos los demás campos, como cuentas y oportunidades, se sincronizan solo de una forma, de Dynamics a Marketing.

## ¿Qué se sincroniza entre Marketing y Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Posibles clientes](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contactos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Cuentas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuarios](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipos (grupos de usuarios del sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Las [credenciales introducidas en Marketing para Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) se utilizan para sincronizar datos.

>[!CAUTION]
>
>Actualmente no se admite la actualización del entorno limitado para Marketing Dynamics Sync. Si necesita actualizar el simulador para pruebas de Dynamics CRM, se necesitará un nuevo simulador para pruebas de Marketing. Póngase en contacto con el administrador de éxito del cliente para obtener más detalles.
