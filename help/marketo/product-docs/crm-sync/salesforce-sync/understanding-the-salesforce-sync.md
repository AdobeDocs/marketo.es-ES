---
unique-page-id: 4719283
description: Descubra cómo la sincronización de Salesforce mantiene sincronizados los datos de Marketo y Salesforce. Ver qué se sincroniza y cómo funciona la sincronización bidireccional para posibles clientes y contactos.
title: Explicación de la sincronización de Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/1H8ol0eKIzfQoQR-Je4jCdZX7R-rWWD63qrhkrsWtyg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 224
ht-degree: 81%

---

# Explicación de la sincronización de [!DNL Salesforce] {#understanding-the-salesforce-sync}

Descubra cómo la sincronización de Salesforce mantiene sincronizados los datos de Marketo y Salesforce.

## Funcionamiento de la sincronización {#how-sync-works}

Marketo se sincroniza con [!DNL Salesforce] todo el día, todos los días. Cada sincronización tarda cierto tiempo en realizarse y luego se detiene durante cinco minutos antes de iniciarse otra vez.

>[!NOTE]
>
>La primera sincronización de su suscripción puede tardar horas o incluso días porque Marketo está copiando toda la base de datos de [!DNL Salesforce]. A partir de ahí, cada sincronización suele tardar segundos o minutos y solo se sincronizan los datos que han cambiado.

![](assets/sync-illustration.png)

La sincronización entre [!DNL Salesforce] y Marketo es bidireccional solamente para clientes potenciales, contactos y campañas de [!DNL Salesforce]. En estos casos, cada vez que realice cambios en [!DNL Salesforce] o en Marketo, las actualizaciones se reflejan en ambos sistemas. Todas las demás sincronizaciones son de [!DNL Salesforce] a Marketo solamente. Haga clic en los vínculos siguientes para obtener información detallada sobre cada una de ellas.

## ¿Qué se sincroniza entre Marketo y [!DNL Salesforce]? {#what-is-synced-between-marketo-and-salesforce}

* [Clientes potenciales](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Contactos](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Cuentas](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Usuarios](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Oportunidades](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Campañas de Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Objetos personalizados](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Actividad](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>Las [credenciales introducidas en Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} se usan para sincronizar datos. Solo se incluirán los datos a los que esas credenciales tengan acceso.

La sincronización de Marketo con [!DNL Salesforce] es la más potente de su tipo en el mundo. Parece magia: se realiza un cambio y el otro sistema se actualiza al instante.
