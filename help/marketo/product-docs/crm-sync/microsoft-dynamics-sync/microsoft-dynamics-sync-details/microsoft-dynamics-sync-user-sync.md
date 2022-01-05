---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Sincronización de usuarios - Documentos de Marketo - Documentación del producto
title: 'Microsoft Dynamics Sync: sincronización de usuarios'
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronización de usuarios {#microsoft-dynamics-sync-user-sync}

¿Sabía que Marketo sincroniza toda la base de datos con Dynamics? Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles sobre cómo trata Marketo específicamente las cuentas de Dynamics.

Necesitará un usuario específico de Microsoft Dynamics CRM para la integración. Llamamos a este usuario de sincronización.

## ¿Cómo se mantienen los detalles del usuario sincronizados entre los dos sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronización de usuarios es unidireccional: de Dynamics a Marketo. Si realiza cambios en un usuario de Dynamics, los cambios se reflejarán en Marketo.

## ¿Puedo crear un usuario con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo no puede crear usuarios en Dynamics.

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) durante la configuración. Sin embargo, Marketo solo sincronizará los campos a los que el usuario de sincronización con Dynamics tiene acceso.
