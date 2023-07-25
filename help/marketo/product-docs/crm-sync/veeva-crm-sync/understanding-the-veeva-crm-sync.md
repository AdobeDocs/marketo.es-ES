---
description: 'Explicación de la sincronización de Veeva CRM: documentos de Marketo: documentación del producto'
title: Explicación de la sincronización de Veeva CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Explicación de la sincronización de Veeva CRM {#understanding-the-veeva-crm-sync}

En unos pocos pasos, es fácil ejecutar una sincronización entre Adobe Marketo Engage y el Veeva CRM.

## Funcionamiento de la sincronización {#how-the-sync-works}

El Marketo Engage se sincroniza con Veeva CRM todo el día, todos los días. Cada sincronización tarda un poco, se pausa durante 5 minutos y se inicia de nuevo.

>[!NOTE]
>
>La primera sincronización puede tardar horas o incluso días porque Marketo Engage está copiando toda la base de datos de Veeva. Después, cada sincronización suele tardar minutos (a veces segundos) y solo sincroniza los datos que han cambiado.

![](assets/understanding-the-veeva-sync-1.png)

La sincronización entre Veeva y Marketo Engage es bidireccional solo para los campos de Contacto en el objeto de cuenta Persona. En estos casos, cada vez que realice cambios en Veeva o en Marketo Engage, las actualizaciones se reflejarán en ambos sistemas. Todas las demás sincronizaciones son solo de Veeva a Marketo Engage. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno de ellos.

## Qué se sincroniza entre Marketo Engage y Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* [Cuentas de persona](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Usuarios
* [Objetos de clave de llamada y llamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Objetos personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Cosas que saber {#things-to-know}

* El [las credenciales que introduce en Marketo Engage para Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} se utilizan para sincronizar datos. Solo se incluirán los datos a los que esas credenciales tengan acceso.

* Veeva CRM se basa en force.com y el Marketo Engage de experiencia enriquecida con la plataforma se hereda en esta sincronización.

* Veeva CRM muestra: posible cliente, contacto, cuentas (cuentas empresariales), oportunidad, campaña y actividad. Sin embargo, no son compatibles con la sincronización con el Marketo Engage.
