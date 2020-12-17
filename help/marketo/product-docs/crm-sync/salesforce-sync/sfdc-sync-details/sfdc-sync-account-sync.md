---
unique-page-id: 2953459
description: Sincronización de SFDC - Sincronización de cuentas - Documentos de marketing - Documentación del producto
title: 'Sincronización de SFDC: Sincronización de cuenta'
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Sincronización SFDC: Sincronización de cuentas {#sfdc-sync-account-sync}

Marketo también sincroniza la información de su cuenta con Salesforce. ¡Aquí hay algunas cosas específicas que deberías saber!

## ¿De qué manera se sincroniza la información? {#which-way-does-the-information-sync}

Sólo de una manera: de SFDC a Marketing.

## ¿Cómo funcionan las actualizaciones? {#how-do-the-updates-work}

Si actualiza un campo Cuenta para un contacto en Marketing, cambiará los valores de todos los contactos que pertenecen a esa cuenta en MarketingTo. No se sincroniza con SFDC. Sin embargo, la próxima vez que la cuenta se actualice en SFDC, los cambios anularán toda la información de la cuenta en Marketing.

## ¿Puede un contacto pertenecer a varias cuentas?  {#can-a-contact-belong-to-multiple-accounts}

No. Una cuenta puede tener muchos contactos, un contacto solo puede tener una cuenta.

## ¿Puedo crear cuentas desde Marketing? {#can-i-create-accounts-from-marketo}

En su mayoría, no. Sin embargo, si utiliza el paso de flujo [Convertir persona](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) en una persona, creará un nuevo contacto, una nueva cuenta y una nueva oportunidad.

>[!CAUTION]
>
>Este paso de flujo tiene un caso de uso muy limitado. Si no estás seguro, probablemente no deberías usarlo.

## ¿Un cambio en un campo de cuenta en Salesforce produce un registro de Actividad de cambio de valor de datos para cada contacto?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

En su mayoría, sí. Sin embargo, si una cuenta tiene más de 5000 contactos y un campo de esa cuenta cambia en SFDC, se sincroniza el cambio pero no se registra la actividad de más de 5000 contactos.
