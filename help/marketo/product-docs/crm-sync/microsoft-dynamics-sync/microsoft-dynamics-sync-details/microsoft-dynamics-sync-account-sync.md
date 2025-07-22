---
unique-page-id: 3571836
description: 'Sincronización de Microsoft Dynamics: sincronización de cuenta, documentos de Marketo: documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de cuenta'
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Sincronización de [!DNL Microsoft Dynamics]: sincronización de cuenta {#microsoft-dynamics-sync-account-sync}

¿Sabía que Marketo sincroniza toda su base de datos con [!DNL Dynamics]? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. Aquí hay algunos detalles sobre cómo Marketo trata específicamente las cuentas de [!DNL Dynamics].

## ¿En qué sentido se sincroniza la información? {#which-way-does-the-information-sync}

Solo hay una forma: de [!DNL Dynamics] a Marketo.

## ¿Cómo funcionan las actualizaciones? {#how-do-the-updates-work}

Si actualiza un campo Cuenta para un contacto en Marketo, cambia los valores de todos los contactos que pertenecen a esa cuenta en Marketo. No se sincroniza con [!DNL Dynamics]. Sin embargo, la próxima vez que se actualice esa cuenta en [!DNL Dynamics], los cambios anularán toda la información de la cuenta en Marketo.

## ¿Puedo crear una cuenta con Marketo? {#can-i-create-an-account-using-marketo}

No. Marketo no puede crear cuentas en [!DNL Dynamics].

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la instalación. Pero Marketo solo sincronizará los campos a los que el usuario de sincronización [!DNL Dynamics] tenga acceso.

## ¿Un cambio en un campo de cuenta en [!DNL Dynamics] genera un registro de actividad de valor de datos de cambio para cada contacto?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Sobre todo, sí. Sin embargo, si una cuenta tiene más de 5000 contactos y un campo de esa cuenta cambia en [!DNL Dynamics], se sincronizará el cambio, pero no se registrará la actividad de más de 5000 contactos.
