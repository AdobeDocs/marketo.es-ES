---
unique-page-id: 3571848
description: 'Sincronización de Microsoft Dynamics: sincronización de posibles clientes - Documentos de Marketo: documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de posibles clientes'
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Sincronización [!DNL Microsoft Dynamics]: sincronización de posibles clientes {#microsoft-dynamics-sync-lead-sync}

La sincronización de Marketo con [!DNL Dynamics] es muy eficaz. A continuación se muestran los detalles:

## ¿Cómo se mantienen los detalles sincronizados entre los dos sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional. Si realiza cambios en un posible cliente de [!DNL Dynamics] o en una persona de Marketo, la actualización se reflejará en ambos sistemas.

>[!NOTE]
>
>Las eliminaciones no siempre se sincronizan automáticamente en ambas direcciones. Ver [Eliminando un posible cliente o contacto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Conflicto de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque no es habitual, Marketo ganará para las personas (posibles clientes) y [!DNL Dynamics] para los contactos. Esto se debe a que consideramos que el departamento de marketing tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos se encuentra en el departamento de ventas (CRM).

## ¿Puedo crear un posible cliente en [!DNL Dynamics] mediante Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sí, usar la acción de flujo [[!UICONTROL Sincronizar persona con Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Esto creará un posible cliente en [!DNL Dynamics] si el posible cliente no existe. Si el posible cliente no existe, el paso de flujo no realizará ninguna acción.

>[!NOTE]
>
>Al usar la acción de flujo &quot;[!UICONTROL Sincronizar persona con Microsoft]&quot; (solo en una campaña de déclencheur), el posible cliente/contacto se creará en tiempo real en [!DNL Dynamics].

## ¿Puedo forzar manualmente una sincronización de una persona de Marketo con un posible cliente de [!DNL Dynamics]? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

No, la sincronización en segundo plano automatizada es la única manera de sincronizar las actualizaciones entre Marketo y [!DNL Dynamics]. La acción de flujo [[!UICONTROL Sincronizar persona con Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) no forzará la sincronización del posible cliente.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante la instalación.

## ¿Marketo respetará las reglas de validación de [!DNL Dynamics]? {#will-marketo-respect-the-dynamics-validation-rules}

Sí. La sincronización fallará si el formato de datos es incorrecto o si falta información de campo necesaria. Marketo registrará el resultado en el registro de actividad de la persona si esto sucede.
