---
description: 'Explicación de la sincronización de Veva CRM: Marketo Docs: Documentación del producto'
title: Explicación de la sincronización de Veva CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
source-git-commit: 884c9a27f3876ec3036f2f7187db30565cdd49a7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Explicación de la sincronización de Veva CRM {#understanding-the-veeva-crm-sync}

En pocos pasos, es fácil ejecutar una sincronización entre Adobe Marketo Engage y Veeva CRM.

## Cómo funciona la sincronización {#how-the-sync-works}

El Marketo Engage se sincroniza con Veeva CRM todo el día, todos los días. Cada sincronización tarda un tiempo, se detiene durante 5 minutos y, a continuación, se inicia de nuevo.

>[!NOTE]
>
>La primera sincronización podría tardar horas o incluso días porque el Marketo Engage está copiando toda la base de datos de Veva. Después, cada sincronización suele tardar minutos (a veces segundos) y solo sincroniza los datos que han cambiado.

![](assets/understanding-the-veeva-sync-1.png)

La sincronización entre Veeva y el Marketo Engage solo es bidireccional para los campos Contacto en el objeto Cuenta de persona . En estos casos, cada vez que realice cambios en Veva o en el Marketo Engage, las actualizaciones se reflejarán en ambos sistemas. Todas las demás sincronizaciones son de Veva a Marketo Engage solamente. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno.

## ¿Qué se sincroniza entre Marketo Engage y Veeva? {#what-is-synced-between-marketo-engage-and-veeva}

* [Cuentas de persona](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target=&quot;_blank&quot;}
* Usuarios
* [Llamar a objetos clave y llamar a ellos](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
* [Objetos personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}

## Aspectos importantes {#things-to-know}

* La variable [credenciales que introduzca en el Marketo Engage de Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target=&quot;_blank&quot;} se usan para sincronizar datos. Solo se incluirán los datos a los que tengan acceso esas credenciales.

* Veeva CRM se basa en force.com y el Marketo Engage de experiencias enriquecidas con la plataforma se hereda en esta sincronización.

* El CRM de Veva muestra: Posible cliente, Contacto, Cuentas (Cuentas comerciales, Oportunidad, Campaña y Actividad). Sin embargo, no son compatibles con la sincronización con el Marketo Engage.
