---
unique-page-id: 1147027
description: 'Sincronizar persona con SFDC: documentos de Marketo: documentación del producto'
title: Sincronizar persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 6%

---

# Sincronizar persona con SFDC {#sync-person-to-sfdc}

Este paso de flujo insertará personas creadas por Marketo como posibles clientes en su Salesforce CRM.

>[!NOTE]
>
>Solo está disponible cuando se integra con [!DNL Salesforce].

1. De forma predeterminada, este paso de flujo asignará a los propietarios de posibles clientes en función de las reglas de asignación automática de Salesforce.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] requiere que la persona tenga rellenados los campos Empresa y Apellidos. De lo contrario, rechazará el registro de posibles clientes.

1. Puede establecer un usuario o cola de posibles clientes [!DNL Salesforce] específico como propietario del posible cliente.

   ![](assets/sync-person-to-sfdc-2.png)

   Al utilizar este paso de flujo, la persona se sincroniza inmediatamente como posible cliente de [!DNL Salesforce] y no necesita esperar a la sincronización normal.

   >[!CAUTION]
   >
   >[!DNL Salesforce] no permite que &quot;Contactos&quot; se asigne a colas de posibles clientes. En este caso, Marketo creará un &quot;posible cliente&quot; duplicado en [!DNL Salesforce].
