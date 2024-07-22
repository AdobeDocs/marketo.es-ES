---
unique-page-id: 2953467
description: 'Sincronización de SFDC: sincronización de oportunidades, documentos de Marketo, documentación del producto'
title: 'Sincronización de SFDC: sincronización de oportunidad'
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 6%

---

# Sincronización de SFDC: sincronización de oportunidad {#sfdc-sync-opportunity-sync}

## ¿Cómo se sincronizan los detalles de las oportunidades entre los dos sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronización es de una manera: de Salesforce a Marketo Engage. Las actualizaciones de oportunidades en Salesforce se sincronizarán con Marketo.

>[!NOTE]
>
>Las [credenciales que ingresaste en Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} se usan para sincronizar datos. Solo se incluirán los datos a los que esas credenciales tengan acceso.

## ¿Puedo iniciar una sincronización de oportunidad? {#can-i-initiate-an-opportunity-sync}

No, no puedes. Los cambios que se realicen en cualquier oportunidad de Salesforce se sincronizarán automáticamente con Marketo.

## ¿Admite Marketo más de una divisa en el importe de la oportunidad? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

No, Marketo solo admite una divisa. La cantidad de la oportunidad se sincronizará con Salesforce, pero la divisa será la [moneda predeterminada](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription){target="_blank"} de su suscripción a Marketo.

## ¿Cómo asocia Marketo las oportunidades y los contactos? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo asocia oportunidades y contactos mediante [roles de contacto de oportunidad](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Las oportunidades sin funciones de contacto asignadas se sincronizarán con Marketo, pero no pertenecerán a nadie. Por ejemplo, la persona no calificará para el filtro Tiene oportunidad.

## ¿Cómo puedo ver todas las oportunidades de una persona? {#how-can-i-see-all-the-opportunities-of-a-person}

Puede ver una lista de oportunidades en la ficha **Información de la oportunidad** de la página [Detalle de la persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## ¿Cuáles son los déclencheur relacionados con la oportunidad? {#what-are-the-triggers-filters-related-to-opportunity}

Desencadenadores:

* Añadido a oportunidad
* Se quitó de oportunidad
* La oportunidad está actualizada

Filtros:

* Tiene oportunidad
* Se actualizó la oportunidad/No se actualizó la oportunidad
* Se agregó a oportunidad/No se agregó a oportunidad
* Se eliminó de la oportunidad/No se eliminó de la oportunidad
* Monto total de la oportunidad
* Cantidad de oportunidades
* Ingreso esperado total de la oportunidad

>[!TIP]
>
>Consulte las restricciones de filtros y déclencheur. Hay muchos detalles geniales ahí dentro.
>
>Simplemente cree un nuevo campo en el objeto de oportunidad en Salesforce y se convertirá automáticamente en una restricción.
