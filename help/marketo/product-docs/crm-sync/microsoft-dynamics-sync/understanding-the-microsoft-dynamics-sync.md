---
unique-page-id: 10098625
description: 'Explicación de la sincronización  [!DNL Microsoft Dynamics] Documentos de Marketo: documentación del producto'
title: Explicación de la sincronización de Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 4%

---

# Explicación de la sincronización [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo y [!DNL Microsoft Dynamics] van juntos. Mantenemos sus datos de ventas y marketing sincronizados.

>[!CAUTION]
>
>Actualmente no se admite la actualización de la zona protegida para la sincronización de [!DNL Marketo Dynamics]. Si necesita actualizar su zona protegida de CRM [!DNL Dynamics], se necesitará una nueva zona protegida de Marketo. Póngase en contacto con el administrador de éxito del cliente para obtener más información.

## Funcionamiento de la sincronización {#how-sync-works}

Marketo sincroniza continuamente los datos con [!DNL Microsoft Dynamics] todo el día, todos los días. Se realiza mediante sincronización en segundo plano, por lotes, no en tiempo real.

>[!NOTE]
>
>La primera sincronización de la suscripción tarda de minutos a horas, según el tamaño de la base de datos. Marketo copia toda la base de datos desde [!DNL Dynamics]. Después, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

La sincronización entre Marketo y [!DNL Dynamics] es bidireccional para posibles clientes y contactos. Si realiza cambios en Marketo o [!DNL Dynamics], las actualizaciones se reflejarán en ambos sistemas. Todos los demás campos, como cuentas y oportunidades, se sincronizan de una sola manera, de [!DNL Dynamics] a Marketo.

## ¿Qué se sincroniza entre Marketo y [!DNL Microsoft Dynamics]? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Clientes potenciales](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contactos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Cuentas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuarios](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipos (grupos de usuarios del sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Las [credenciales que ingresaste en Marketo para [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) se usan para sincronizar datos.

>[!NOTE]
>
>No se admite la copia de instancia si la instancia de origen está integrada con [!DNL Microsoft Dynamics].
