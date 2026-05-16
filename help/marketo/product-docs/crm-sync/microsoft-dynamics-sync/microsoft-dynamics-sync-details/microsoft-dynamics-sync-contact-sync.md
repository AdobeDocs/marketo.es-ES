---
unique-page-id: 3571833
description: Obtenga información acerca de cómo funciona la sincronización de contactos entre Microsoft Dynamics y Marketo. Comprenda la sincronización bidireccional, la creación de contactos desde Marketo y las reglas de colisión de datos.
title: 'Sincronización de Microsoft Dynamics: sincronización de contactos'
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/8Y8vrxxm1VZ99tUIQ5bp8gbWDtduaiOqQl7kpadFvqo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 0%

---

# Sincronización de [!DNL Microsoft Dynamics]: sincronización de contactos {#microsoft-dynamics-sync-contact-sync}

Marketo sincroniza toda la base de datos con [!DNL Dynamics]. Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles acerca de cómo Marketo trata específicamente a [!DNL Dynamics] contactos.

## ¿Cómo se mantienen los detalles sincronizados entre los dos sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto de [!DNL Dynamics] o en una persona de Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque no es habitual, Marketo ganará para las personas y [!DNL Dynamics] para los contactos. Esto se debe a que consideramos que el departamento de marketing tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos se encuentra en el departamento de ventas (CRM).

## ¿Puedo crear un contacto con Marketo? {#can-i-create-a-contact-using-marketo}

Sí. [Más información](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Al utilizar la acción de flujo &quot;Sincronizar persona con Microsoft&quot; (solo en una campaña de déclencheur), el posible cliente/contacto se creará en tiempo real en [!DNL Dynamics].

## ¿Puedo forzar manualmente una sincronización de una persona o un contacto? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

No, la sincronización en segundo plano automatizada es la única manera de sincronizar las actualizaciones entre Marketo y [!DNL Dynamics]. [Sincronizar persona con Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) no forzará una sincronización del posible cliente.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante la instalación. Pero Marketo solo sincronizará los campos a los que el usuario de sincronización [!DNL Dynamics] tenga acceso.

## ¿Marketo respetará las reglas de validación de [!DNL Dynamics]? {#will-marketo-respect-the-dynamics-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de actividad de posibles clientes.
