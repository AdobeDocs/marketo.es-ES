---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Sincronización de cuentas - Documentos de Marketo - Documentación del producto
title: Microsoft Dynamics Sync - Sincronización de cuentas
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronización de cuentas {#microsoft-dynamics-sync-account-sync}

¿Sabía que Marketo sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketo específicamente las cuentas de Dynamics.

## ¿Cómo se sincroniza la información? {#which-way-does-the-information-sync}

Solo de una manera: de Dynamics a Marketo.

## ¿Cómo funcionan las actualizaciones? {#how-do-the-updates-work}

Si actualiza un campo Cuenta para un contacto en Marketo, cambia los valores de todos los contactos que pertenecen a esa cuenta en Marketo. No se sincroniza con Dynamics. Sin embargo, la próxima vez que la cuenta se actualice en Dynamics, los cambios anularán toda la información de la cuenta en Marketo.

## ¿Puedo crear una cuenta con Marketo? {#can-i-create-an-account-using-marketo}

No. Marketo no puede crear cuentas en Dynamics.

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante la configuración. Sin embargo, Marketo solo sincronizará los campos a los que el usuario de sincronización con Dynamics tiene acceso.

## ¿Un cambio en un campo de cuenta en Dynamics genera un registro de actividad de cambio de valor de datos para cada contacto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

En su mayoría, sí. Sin embargo, si una cuenta tiene más de 5000 contactos y un campo de esa cuenta cambia en Dynamics, se sincroniza el cambio pero no se registra la actividad de los más de 5000 contactos.
