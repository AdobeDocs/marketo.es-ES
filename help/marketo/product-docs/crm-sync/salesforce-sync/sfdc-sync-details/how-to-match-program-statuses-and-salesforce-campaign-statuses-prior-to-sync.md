---
unique-page-id: 2360370
description: 'Cómo hacer coincidir los estados de los programas y de Salesforce Campaign antes de la sincronización: Documentos de Marketo: documentación del producto'
title: Igualar estados de programas y estados de Salesforce Campaign antes de la sincronización
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '219'
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
