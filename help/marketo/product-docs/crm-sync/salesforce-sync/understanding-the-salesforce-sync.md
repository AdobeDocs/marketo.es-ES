---
unique-page-id: 4719283
description: Explicación de la sincronización de Salesforce, documentos de Marketo, documentación del producto
title: Explicación de la sincronización de Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Explicación de la sincronización [!DNL Salesforce] {#understanding-the-salesforce-sync}

Marketo Engage y Salesforce van juntos como guisantes y zanahorias. Mantenemos sus datos de ventas y marketing sincronizados.

## Funcionamiento de la sincronización {#how-sync-works}

Marketo se sincroniza con [!DNL Salesforce] todo el día, todos los días. Cada sincronización tarda un poco y luego se detiene durante 5 minutos, luego se inicia nuevamente.

>[!NOTE]
>
>La primera sincronización de su suscripción puede tardar horas o incluso días porque Marketo está copiando toda la base de datos de [!DNL Salesforce]. Después, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

![](assets/sync-illustration.png)

La sincronización entre [!DNL Salesforce] y Marketo es bidireccional solamente para posibles clientes, contactos y campañas de [!DNL Salesforce]. En estos casos, cada vez que realice cambios en [!DNL Salesforce] o Marketo, las actualizaciones se reflejarán en ambos sistemas. Todas las demás sincronizaciones son solo de [!DNL Salesforce] a Marketo. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno de ellos.

## ¿Qué se sincroniza entre Marketo y [!DNL Salesforce]? {#what-is-synced-between-marketo-and-salesforce}

* [Posibles clientes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Contactos](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Cuentas](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Usuarios](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Oportunidades](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Campañas de Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Objetos personalizados](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Actividad](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>Las [credenciales que ingresaste en Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} se usan para sincronizar datos. Solo se incluirán los datos a los que esas credenciales tengan acceso.

La sincronización de Marketo con [!DNL Salesforce] es la más potente de su tipo en el mundo. Se siente como magia; se hace un cambio y el otro sistema está pronto actualizado.
