---
unique-page-id: 10098625
description: 'Explicación de la sincronización de Microsoft Dynamics: documentos de Marketo, documentación del producto'
title: Explicación de la sincronización de Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Explicación de la sincronización de Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

Marketo y Microsoft Dynamics van juntos. Mantenemos sus datos de ventas y marketing sincronizados.

>[!NOTE]
>
>Marketo solo admite certificados SSL compatibles con Java 7 en este momento.

>[!CAUTION]
>
>Actualmente no se admite la actualización de la zona protegida para la sincronización de Marketo Dynamics. Si necesita actualizar la zona protegida de Dynamics CRM, se necesitará una nueva zona protegida de Marketo. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

## Funcionamiento de la sincronización {#how-sync-works}

Marketo sincroniza continuamente los datos con Microsoft Dynamics todo el día, todos los días. Se realiza mediante sincronización en segundo plano, por lotes, no en tiempo real.

>[!NOTE]
>
>La primera sincronización de la suscripción tarda de minutos a horas, según el tamaño de la base de datos. Marketo copia toda la base de datos desde Dynamics. Después, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

La sincronización entre Marketo y Dynamics es bidireccional para posibles clientes y contactos. Si realiza cambios en Marketo o Dynamics, las actualizaciones se reflejarán en ambos sistemas. Todos los demás campos, como cuentas y oportunidades, se sincronizan solo de una manera, de Dynamics a Marketo.

## ¿Qué se sincroniza entre Marketo y Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contactos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Cuentas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuarios](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipos (grupos de usuarios del sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

El [credenciales introducidas en Marketo para Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) se utilizan para sincronizar datos.

>[!NOTE]
>
>No se admite la copia de instancia si la instancia de origen está integrada con Microsoft Dynamics.
