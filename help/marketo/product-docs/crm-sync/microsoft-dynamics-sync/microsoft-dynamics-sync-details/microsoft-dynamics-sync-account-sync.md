---
unique-page-id: 3571836
description: 'Sincronización de Microsoft Dynamics: sincronización de cuenta, documentos de Marketo: documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de cuenta'
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Sincronización de Microsoft Dynamics: sincronización de cuenta {#microsoft-dynamics-sync-account-sync}

¿Sabía que Marketo sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se muestran algunos detalles sobre cómo Marketo trata específicamente las cuentas de Dynamics.

## ¿En qué sentido se sincroniza la información? {#which-way-does-the-information-sync}

Solo hay una forma: de Dynamics a Marketo.

## ¿Cómo funcionan las actualizaciones? {#how-do-the-updates-work}

Si actualiza un campo Cuenta para un contacto en Marketo, cambia los valores de todos los contactos que pertenecen a esa cuenta en Marketo. No se sincroniza con Dynamics. Sin embargo, la próxima vez que esa cuenta se actualice en Dynamics, los cambios anularán toda la información de la cuenta en Marketo.

## ¿Puedo crear una cuenta con Marketo? {#can-i-create-an-account-using-marketo}

No. Marketo no puede crear cuentas en Dynamics.

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la configuración. Sin embargo, Marketo solo sincronizará los campos a los que el usuario de sincronización de Dynamics tiene acceso.

## ¿Un cambio en un campo de cuenta en Dynamics genera un registro de actividad Cambiar valor de datos para cada contacto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Sobre todo, sí. Sin embargo, si una cuenta tiene más de 5000 contactos y un campo en esa cuenta cambia en Dynamics, sincronizamos el cambio pero no registramos la actividad de más de 5000 contactos.
