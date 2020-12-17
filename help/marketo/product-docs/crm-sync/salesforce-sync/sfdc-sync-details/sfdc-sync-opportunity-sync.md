---
unique-page-id: 2953467
description: Sincronización SFDC - Sincronización de oportunidades - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: Sincronización de oportunidades'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización de oportunidad {#sfdc-sync-opportunity-sync}

## ¿Cómo se mantienen sincronizados los detalles de oportunidad entre los dos sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronización es de una manera: de Salesforce a Marketing. Las actualizaciones de las oportunidades en Salesforce se sincronizarán con Marketing.

>[!NOTE]
>
>Las [credenciales introducidas en Marketing para Salesforce](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) se utilizan para sincronizar datos. Solo se incluirán los datos a los que tienen acceso esas credenciales.

## ¿Puedo iniciar una sincronización de oportunidad? {#can-i-initiate-an-opportunity-sync}

No, no puedes. Los cambios realizados en cualquier oportunidad de Salesforce se sincronizarán automáticamente con Marketing.

## ¿Es compatible Marketing con más de una moneda en la cantidad de oportunidad? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

No, Marketo solo admite una moneda. La cantidad de oportunidad se sincronizará desde Salesforce, pero la moneda será la [divisa predeterminada](https://docs.marketo.com/display/DOCS/Set+Default+Location+Settings+for+a+Subscription#SetDefaultLocationSettingsforaSubscription-SettheDefaultCurrencySettingsforaSubscription) en la suscripción de Marketing.

## ¿Cómo asocia Marketing a oportunidades y contactos? {#how-does-marketo-associate-opportunities-and-contacts}

Marketing asocia oportunidades y contactos mediante [Funciones de contacto de oportunidad](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Las oportunidades sin ninguna función de contacto asignada se sincronizarán con Marketing, pero no pertenecerán a nadie. Por ejemplo, la persona no calificará el filtro Tiene oportunidad.

## ¿Cómo puedo ver todas las oportunidades de una persona? {#how-can-i-see-all-the-opportunities-of-a-person}

Puede vista de una lista de oportunidades en la ficha **Información de oportunidad** de la página [Detalles de persona](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## ¿Cuáles son los activadores/filtros relacionados con la oportunidad? {#what-are-the-triggers-filters-related-to-opportunity}

Desencadenadores:

* Añadido a la oportunidad
* Eliminado de la oportunidad
* Se ha actualizado la oportunidad

Filtros:

* Tiene oportunidad
* Se actualizó la oportunidad o no se actualizó la oportunidad
* Se Añadió a Oportunidad/No se Añadió a Oportunidad
* Se eliminó la oportunidad/No se eliminó la oportunidad
* Importe total de la opción
* Número de opciones
* Total de ingresos esperados de opción

>[!TIP]
>
>Consulte las restricciones de filtros y activadores. Muchos detalles geniales ahí dentro.
>
>Simplemente haz un nuevo campo en el objeto de oportunidad en Salesforce y automáticamente se convertirá en una restricción!

Marketo tiene la mejor sincronización de Salesforce del mundo!