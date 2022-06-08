---
unique-page-id: 2953467
description: Sincronización SFDC - Sincronización de oportunidades - Documentos de Marketo - Documentación del producto
title: 'Sincronización de SFDC: sincronización de oportunidades'
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 4%

---

# Sincronización SFDC: Sincronización de oportunidades {#sfdc-sync-opportunity-sync}

## ¿Cómo se mantienen los detalles de oportunidad sincronizados entre los dos sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronización es unidireccional: de Salesforce a Marketo. Las actualizaciones de las oportunidades de Salesforce se sincronizarán con Marketo.

>[!NOTE]
>
>La variable [credenciales introducidas en Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) se utilizan para sincronizar datos. Solo se incluirán los datos a los que tengan acceso esas credenciales.

## ¿Puedo iniciar una sincronización de oportunidad? {#can-i-initiate-an-opportunity-sync}

No, no puedes. Los cambios realizados en cualquier oportunidad de Salesforce se sincronizarán automáticamente con Marketo.

## ¿Marketo admite más de una moneda en la cantidad de oportunidad? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

No, Marketo solo admite una moneda. La cantidad de oportunidad se sincronizará con Salesforce, pero la moneda será la [moneda predeterminada](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) en su suscripción a Marketo.

## ¿Cómo asocia Marketo las oportunidades y los contactos? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo asocia oportunidades y contactos mediante [Funciones de contacto de oportunidad](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Las oportunidades sin ninguna función de contacto asignada se sincronizarán con Marketo, pero no pertenecerán a nadie. Por ejemplo, la persona no calificará el filtro Tiene oportunidad .

## ¿Cómo puedo ver todas las oportunidades de una persona? {#how-can-i-see-all-the-opportunities-of-a-person}

Puede ver una lista de oportunidades en la **Información de oportunidad** en la ficha [Detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) página.

## ¿Cuáles son los déclencheur/filtros relacionados con la oportunidad? {#what-are-the-triggers-filters-related-to-opportunity}

Desencadenadores:

* Se ha añadido a la oportunidad
* Eliminada de la oportunidad
* Se ha actualizado la oportunidad

Filtros:

* Tiene una oportunidad
* Se actualizó la oportunidad/no se actualizó la oportunidad
* Se agregó a la oportunidad/no se agregó a la oportunidad
* Se eliminó de la oportunidad/no se eliminó de la oportunidad
* Monto total de la oportunidad
* Cantidad de oportunidades
* Ingreso esperado total de la oportunidad

>[!TIP]
>
>Consulte las restricciones de los filtros y déclencheur. Muchos detalles geniales ahí dentro.
>
>Simplemente haga un nuevo campo en el objeto de oportunidad en Salesforce y se convertirá automáticamente en una restricción!
