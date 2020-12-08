---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Sincronización de cuentas - Documentos de marketing - Documentación del producto
title: Microsoft Dynamics Sync - Sincronización de cuentas
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronización de cuentas {#microsoft-dynamics-sync-account-sync}

¿Sabía que Marketing sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketing específicamente las cuentas de Dynamics.

## ¿De qué manera se sincroniza la información? {#which-way-does-the-information-sync}

Sólo de una manera: de Dynamics a Marketing.

## ¿Cómo funcionan las actualizaciones? {#how-do-the-updates-work}

Si actualiza un campo Cuenta para un contacto en Marketing, cambiará los valores de todos los contactos que pertenecen a esa cuenta en MarketingTo. No se sincroniza con Dynamics. Sin embargo, la próxima vez que la cuenta se actualice en Dynamics, los cambios anularán toda la información de la cuenta en Marketing.

## ¿Puedo crear una cuenta con Marketing? {#can-i-create-an-account-using-marketo}

No. Marketo no puede crear cuentas en Dynamics.

## ¿Qué campos se sincronizarán con Marketing? {#which-fields-will-sync-to-marketo}

Puede [seleccionar los campos que sincronizar](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante la configuración. Sin embargo, Marketing solo sincronizará los campos a los que tiene acceso el usuario de sincronización de Dynamics.

## ¿Un cambio en un campo de cuenta en Dynamics da como resultado un registro de Actividad de cambio de valor de datos para cada contacto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

En su mayoría, sí. Sin embargo, si una cuenta tiene más de 5000 contactos y un campo de esa cuenta cambia en Dynamics, se sincroniza el cambio pero no se registra la actividad de más de 5000 contactos.
