---
unique-page-id: 1147027
description: Sincronizar persona con SFDC - Marketo Docs - Documentación del producto
title: Sincronizar persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---

# Sincronizar persona con SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Solo disponible cuando se integra con Salesforce.

## Información general {#overview}

Este paso de flujo insertará personas creadas por Marketo como posibles clientes en Salesforce CRM.

![](assets/sync-person-to-sfdc.png)

## Uso {#usage}

1. De forma predeterminada, este paso de flujo se asignará a los propietarios de posibles clientes en función de las reglas de asignación automática de Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce requiere que la persona tenga rellenados los campos Empresa y Apellido. De lo contrario, rechazará el registro de posibles clientes.

1. Puede establecer un usuario específico de Salesforce o una cola de posibles clientes como propietario principal.

   ![](assets/sync-person-to-sfdc-2.png)

   Al utilizar este paso de flujo, la persona se sincroniza inmediatamente como posible cliente de Salesforce y no necesita esperar a la sincronización normal.

   >[!CAUTION]
   >
   >Salesforce no permite asignar &quot;Contactos&quot; a las colas de posibles clientes. En este caso, Marketo creará un &quot;posible cliente&quot; duplicado en Salesforce.
