---
unique-page-id: 4719283
description: 'Explicación de la sincronización de Salesforce: Marketo Docs: Documentación del producto'
title: Explicación de la sincronización de Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Explicación de la sincronización de Salesforce {#understanding-the-salesforce-sync}

Marketo y Salesforce van juntos como guisantes y zanahorias. Mantenemos sus datos de ventas y marketing sincronizados.

## Cómo funciona la sincronización {#how-sync-works}

Marketo se sincroniza con Salesforce todo el día, todos los días. Cada sincronización tarda un tiempo y luego se detiene durante 5 minutos y luego se inicia de nuevo.

>[!NOTE]
>
>La primera sincronización de la suscripción puede tardar horas o incluso días, ya que Marketo está copiando toda la base de datos de Salesforce. Después, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

![](assets/sync-illustration.png)

La sincronización entre Salesforce y Marketo solo es bidireccional para posibles clientes, contactos y campañas de Salesforce. En estos casos, cada vez que realice cambios en Salesforce o Marketo, las actualizaciones se reflejarán en ambos sistemas. Todas las demás sincronizaciones son de Salesforce a Marketo solamente. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno.

## ¿Qué se sincroniza entre Marketo y Salesforce? {#what-is-synced-between-marketo-and-salesforce}

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
>Las [credenciales introducidas en Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) se utilizan para sincronizar los datos. Solo se incluirán los datos a los que tengan acceso esas credenciales.

La sincronización de Marketo con Salesforce es la más poderosa de su tipo en el mundo. Parece magia; se realiza un cambio y el otro sistema está actualizado próximamente.
