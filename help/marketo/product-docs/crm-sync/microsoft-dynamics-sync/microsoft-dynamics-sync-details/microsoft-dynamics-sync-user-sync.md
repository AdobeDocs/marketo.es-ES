---
unique-page-id: 3571840
description: 'Sincronización de Microsoft Dynamics: sincronización de usuarios, documentos de Marketo: documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de usuarios'
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Sincronización de Microsoft Dynamics: sincronización de usuarios {#microsoft-dynamics-sync-user-sync}

¿Sabía que Marketo Engage sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se muestran algunos detalles sobre cómo Marketo trata específicamente las cuentas de Dynamics.

Necesitará un usuario de Microsoft Dynamics CRM específico para la integración. Llamamos a este usuario Usuario de sincronización.

## ¿Cómo se sincronizan los detalles del usuario entre los dos sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronización de usuarios es unidireccional: de Dynamics a Marketo. Si realiza cambios en un usuario en Dynamics, los cambios se reflejarán en Marketo.

## ¿Puedo crear un usuario con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo no puede crear usuarios en Dynamics.

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante la instalación. Sin embargo, Marketo solo sincronizará los campos a los que el usuario de sincronización de Dynamics tiene acceso.
