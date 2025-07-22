---
unique-page-id: 3571840
description: Microsoft [!DNL Dynamics] Sync - Sincronización de usuarios - Documentos de Marketo - Documentación del producto
title: 'Sincronizar  [!DNL Dynamics] Microsoft: sincronización de usuario'
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Sincronización de Microsoft [!DNL Dynamics]: sincronización de usuarios {#microsoft-dynamics-sync-user-sync}

¿Sabía que Marketo sincroniza toda su base de datos con [!DNL Dynamics]? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. Aquí hay algunos detalles sobre cómo Marketo trata específicamente las cuentas de [!DNL Dynamics].

Necesitará un usuario de CRM de Microsoft [!DNL Dynamics] dedicado para la integración. Llamamos a este usuario Usuario de sincronización.

## ¿Cómo se sincronizan los detalles del usuario entre los dos sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronización del usuario es de una manera: [!DNL Dynamics] con Marketo. Si realiza cambios en un usuario de [!DNL Dynamics], los cambios se reflejarán en Marketo.

## ¿Puedo crear un usuario con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo no puede crear usuarios en [!DNL Dynamics].

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la instalación. Pero Marketo solo sincronizará los campos a los que el usuario de sincronización [!DNL Dynamics] tenga acceso.
