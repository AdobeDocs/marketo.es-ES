---
unique-page-id: 1147027
description: Sincronizar persona con SFDC - Documentos de marketing - Documentación del producto
title: Sincronizar persona con SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# Sincronizar persona con SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Sólo disponible cuando se integra con Salesforce.

## Información general {#overview}

Este paso de flujo insertará a las personas creadas en el mercado como posibles clientes en Salesforce CRM.

![](assets/sync-person-to-sfdc.png)

## Uso {#usage}

1. De forma predeterminada, este paso de flujo se asignará a los propietarios de posibles clientes en función de las reglas de asignación automática de Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce requiere que la persona tenga rellenados los campos Compañía y Apellido. De lo contrario, rechazará el registro de posibles clientes.

1. Puede establecer un usuario de Salesforce o una cola de posibles clientes específica como propietario principal.

   ![](assets/sync-person-to-sfdc-2.png)

   Al utilizar este paso de flujo, la persona se sincroniza inmediatamente como posible cliente de Salesforce y no necesita esperar a la sincronización regular.

   >[!CAUTION]
   >
   >Salesforce no permite asignar &quot;Contactos&quot; a las colas de posibles clientes. En este caso, Marketing creará un duplicado &quot;Posible cliente&quot; en Salesforce.

