---
unique-page-id: 3571840
description: Obtenga información sobre cómo se sincronizan los datos de usuario de Microsoft Dynamics con Marketo. Comprenda qué campos de propietario se sincronizan y cómo utilizarlos en listas inteligentes y acciones de flujo.
title: 'Sincronización de Microsoft [!DNL Dynamics]: sincronización de usuarios'
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/8H1bMdkhxcvyTuYtHHk00GUy4uycuQ1unsGbZ19AjCM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%
---
# Sincronización de Microsoft [!DNL Dynamics]: sincronización de usuarios {#microsoft-dynamics-sync-user-sync}

Marketo sincroniza toda la base de datos con [!DNL Dynamics]. Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. Aquí hay algunos detalles sobre cómo Marketo trata específicamente las cuentas de [!DNL Dynamics].

Necesitará un usuario de CRM de Microsoft [!DNL Dynamics] dedicado para la integración. Llamamos a este usuario Usuario de sincronización.

## ¿Cómo se sincronizan los detalles del usuario entre los dos sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La sincronización del usuario es de una manera: [!DNL Dynamics] con Marketo. Si realiza cambios en un usuario de [!DNL Dynamics], los cambios se reflejarán en Marketo.

## ¿Puedo crear un usuario con Marketo? {#can-i-create-an-user-using-marketo}

No. Marketo no puede crear usuarios en [!DNL Dynamics].

## ¿Qué campos se sincronizarán con Marketo? {#which-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la instalación. Pero Marketo solo sincronizará los campos a los que el usuario de sincronización [!DNL Dynamics] tenga acceso.
