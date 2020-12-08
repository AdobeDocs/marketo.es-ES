---
unique-page-id: 4719283
description: Explicación de la sincronización de Salesforce - Documentos de marketing - Documentación del producto
title: Explicación de la sincronización de Salesforce
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Explicación de la sincronización de Salesforce {#understanding-the-salesforce-sync}

Marketo y Salesforce van juntos como guisantes y zanahorias. Mantenemos sus datos de ventas y marketing sincronizados.

## Funcionamiento de la sincronización {#how-sync-works}

Marketo se sincroniza con Salesforce todo el día, todos los días. Cada sincronización tarda un tiempo y, a continuación, se pausa durante 5 minutos y, a continuación, se vuelven a realizar inicios.

>[!NOTE]
>
>La primera sincronización de la suscripción puede tardar horas o incluso días porque Marketing está copiando toda la base de datos desde Salesforce. Después de eso, cada sincronización suele tardar segundos o minutos y solo sincroniza los datos que han cambiado.

![](assets/sync-illustration.png)

La sincronización entre Salesforce y Marketing solo es bidireccional para posibles clientes, contactos y campañas de Salesforce. En estos casos, cada vez que realice cambios en Salesforce o en Marketing, las actualizaciones se reflejarán en ambos sistemas. El resto de sincronizaciones se realizan únicamente de Salesforce a Marketing. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno.

## ¿Qué se sincroniza entre Marketing y Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Posibles clientes](sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contactos](sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Cuentas](sfdc-sync-details/sfdc-sync-account-sync.md)
* [Usuarios](sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Oportunidades](sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campañas de Salesforce](sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Objetos personalizados](sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Actividad](sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Las [credenciales introducidas en Marketing para Salesforce](setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) se utilizan para sincronizar los datos. Solo se incluirán los datos a los que tienen acceso esas credenciales.

Hay muchos matices y características sobre la sincronización de Salesforce. Consulte los detalles en la sección [Detalles de sincronización de](http://docs.marketo.com/display/docs/sfdc+sync+details)SFDC.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Configuración de sincronización de Salesforce](http://docs.marketo.com/display/docs/setup)
>* [Detalles de sincronización SFDC](http://docs.marketo.com/display/docs/sfdc+sync+details)

>



La sincronización de Marketo con Salesforce es la más poderosa de este tipo en el mundo. Se siente como magia - se hace un cambio y el otro sistema está pronto actualizado.