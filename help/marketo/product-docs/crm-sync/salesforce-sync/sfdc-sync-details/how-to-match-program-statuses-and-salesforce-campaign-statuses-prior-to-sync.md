---
unique-page-id: 2360370
description: Obtenga información sobre cómo hacer coincidir los estados de programas de Marketo con los estados de miembros de campañas de Salesforce antes de sincronizar. Corrija los errores y asigne los estados para que los programas se sincronicen con las campañas.
title: Igualar estados de programas y estados de Salesforce Campaign antes de la sincronización
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/54XVLabyXlccM45i9yxPRoMqyrCtoDsATu1o1bEy-50'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 5%
---
# Cómo hacer coincidir estados de programas y [!DNL Salesforce] estados de campañas antes de la sincronización {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Este artículo describe cómo corregir un error de estado incompatible y asignar estados antes del Programa Marketo y la sincronización de campaña [!DNL Salesforce].

## ¿Qué debe hacer si recibe un mensaje de error? {#what-do-you-do-if-you-received-an-error-message}

Si intenta sincronizar con una campaña [!DNL Salesforce] existente que contenga posibles clientes y la campaña contiene uno o más estados incompatibles, se mostrará un mensaje de error. Un programa de Marketo y una campaña [!DNL Salesforce] *no se sincronizarán* si los estados no coinciden exactamente.

![](assets/image2015-7-22-9-3a23-3a29.png)

Desde este mensaje de error, puede optar por:

1. Seleccione una campaña diferente a la que sincronizar desde el menú desplegable O
1. Puede cancelar, corregir los errores de estado e intentar sincronizar una vez reparados. Para corregir los errores de estado, realice una de las siguientes acciones:

   * Inicie sesión en Salesforce y elimine o cambie el nombre de los Estados miembros de Campaign incompatibles para asignarlos a los Estados de programa de Marketo utilizados para el tipo de canal asociado con su programa de Marketo.
   * Modifique los estados de los programas en Marketo para asignarlos a los estados miembros de Salesforce Campaign que tenga. Esta es una función de administración de Marketo. Para obtener más información, consulte [Crear un canal de programa](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.
