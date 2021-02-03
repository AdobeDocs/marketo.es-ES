---
unique-page-id: 2360370
description: Cómo hacer coincidir estados de Programa y estados de Campaña de Salesforce antes de la sincronización - Documentos de marketing - Documentación del producto
title: Cómo hacer coincidir estados de Programa y estados de Campaña de Salesforce antes de la sincronización
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Cómo hacer coincidir estados de Programa y estados de Campaña de Salesforce antes de sincronizar {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

En este artículo se describe cómo corregir un error de estado incompatible y asignar estados antes de la sincronización de Campañas de Marketing Programa y Salesforce.

## Qué debe hacer si recibió un mensaje de error {#what-do-you-do-if-you-received-an-error-message}

Si intenta sincronizar con una Campaña existente de Salesforce que contenga leads y la campaña contenga uno o varios estados incompatibles, se muestra un mensaje de error. Un Programa de marketing y una Campaña de Salesforce *no se sincronizarán* si los estados no coinciden exactamente.

![](assets/image2015-7-22-9-3a23-3a29.png)

En este mensaje de error puede optar por:

1. Seleccione una campaña diferente para sincronizar en el menú desplegable O
1. Puede cancelar, corregir los errores de estado e intentar sincronizar una vez que se hayan reparado los errores. Para corregir los errores de estado, realice una de las siguientes acciones:

   * Inicie sesión en Salesforce y elimine o cambie el nombre de los Estados miembros de la Campaña incompatible para asignarlos a los estados de Programa de marketing utilizados para el tipo de canal asociado al Programa de marketing.
   * Modifique los estados de Programa en Marketing para asignarlos a los Estados miembros de la Campaña de Salesforce que tenga establecidos. Esta es una función de administrador de marketing. Para obtener más información, consulte [Creación de un Canal de Programa](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
