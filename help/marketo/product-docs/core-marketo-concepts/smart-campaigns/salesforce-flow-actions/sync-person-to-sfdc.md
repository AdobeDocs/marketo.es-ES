---
unique-page-id: 1147027
description: 'Sincronizar persona con SFDC: documentos de Marketo, documentación del producto'
title: Sincronizar persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 6%

---

# Sincronizar persona con SFDC {#sync-person-to-sfdc}

Este paso de flujo insertará personas creadas por Marketo como posibles clientes en su Salesforce CRM.

![](assets/sync-person-to-sfdc.png)

>[!NOTE]
>
>Solo está disponible cuando se integra con Salesforce.

1. De forma predeterminada, este paso de flujo asignará a los propietarios de posibles clientes en función de las reglas de asignación automática de Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce requiere que la persona tenga rellenados los campos Empresa y Apellidos. De lo contrario, rechazará el registro de posibles clientes.

1. Puede establecer un usuario de Salesforce específico o una cola de posibles clientes como propietario del posible cliente.

   ![](assets/sync-person-to-sfdc-2.png)

   Al utilizar este paso de flujo, la persona se sincroniza inmediatamente como posible cliente de Salesforce y no necesita esperar a la sincronización normal.

   >[!CAUTION]
   >
   >Salesforce no permite que &quot;Contactos&quot; se asigne a colas de posibles clientes. En este caso, Marketo creará un &quot;posible cliente&quot; duplicado en Salesforce.
