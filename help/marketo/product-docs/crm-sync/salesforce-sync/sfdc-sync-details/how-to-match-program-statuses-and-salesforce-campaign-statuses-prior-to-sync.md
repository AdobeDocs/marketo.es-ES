---
unique-page-id: 2360370
description: Coincidencia de los estados del programa y los estados de la campaña de Salesforce antes de la sincronización - Documentos de Marketo - Documentación del producto
title: Coincidencia de estados de programa y estados de campaña de Salesforce antes de la sincronización
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Coincidencia de estados de programa y estados de campaña de Salesforce antes de la sincronización {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

En este artículo se describe cómo corregir un error de estado incompatible y los estados de asignación antes de la sincronización de Marketo Program y Salesforce Campaign.

## Qué hacer si recibió un mensaje de error {#what-do-you-do-if-you-received-an-error-message}

Si intenta sincronizar con una campaña de Salesforce existente que contiene posibles clientes y la campaña contiene uno o más estados incompatibles, se muestra un mensaje de error. Un programa de Marketo y una campaña de Salesforce *no se sincronizarán* si los estados no coinciden exactamente.

![](assets/image2015-7-22-9-3a23-3a29.png)

Desde este mensaje de error, puede optar por:

1. Seleccione una campaña distinta a la que sincronizar en el menú desplegable O
1. Puede cancelar, corregir los errores de estado e intentar sincronizar una vez reparados los errores. Para corregir los errores de estado, realice una de las siguientes acciones:

   * Inicie sesión en Salesforce y elimine o cambie el nombre de los estados miembros de la campaña incompatibles para asignarlos a los estados del programa de Marketo que se usan para el tipo de canal asociado con su programa de Marketo.
   * Modifique los estados del programa en Marketo para asignarlos a los estados miembros de la campaña de Salesforce que tenga establecidos. Se trata de una función de administración de Marketo. Para obtener más información, consulte [Crear un canal de programa](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
