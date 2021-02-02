---
unique-page-id: 4719283
description: Explicación de la sincronización de Salesforce - Documentos de marketing - Documentación del producto
title: Explicación de la sincronización de Salesforce
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Explicación de la sincronización de Salesforce {#understanding-the-salesforce-sync}

Marketo y Salesforce van juntos como guisantes y zanahorias. Mantenemos sus datos de ventas y marketing sincronizados.

## Cómo funciona la sincronización {#how-sync-works}

Marketo se sincroniza con Salesforce todo el día, todos los días. Cada sincronización tarda un tiempo y, a continuación, se pausa durante 5 minutos y, a continuación, se vuelven a realizar inicios.

>[!NOTE]
>
>La primera sincronización de la suscripción puede tardar horas o incluso días porque Marketing está copiando toda la base de datos desde Salesforce. Después de eso, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

![](assets/sync-illustration.png)

La sincronización entre Salesforce y Marketing solo es bidireccional para posibles clientes, contactos y campañas de Salesforce. En estos casos, cada vez que realice cambios en Salesforce o en Marketing, las actualizaciones se reflejarán en ambos sistemas. El resto de sincronizaciones se realizan únicamente de Salesforce a Marketing. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno.

## ¿Qué se sincroniza entre Marketing y Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Posibles clientes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contactos](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Cuentas](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Usuarios](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Oportunidades](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campañas de Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Objetos personalizados](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Actividad](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Las [credenciales introducidas en Marketing para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) se utilizan para sincronizar datos. Solo se incluirán los datos a los que tienen acceso esas credenciales.

La sincronización de Marketo con Salesforce es la más poderosa de este tipo en el mundo. Parece magia; se realiza un cambio y el otro sistema está pronto actualizado.
