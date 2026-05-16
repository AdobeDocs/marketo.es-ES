---
unique-page-id: 1147027
description: Obtenga información sobre cómo sincronizar una persona con Salesforce mediante un paso de flujo. Insertar datos de contactos o posibles clientes en SFDC cuando entren en el flujo.
title: Sincronizar persona con SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/jU7Hg1x8TUfxR4GnO1oxvJXh-8X3LVXll9z8k5Eck80
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 143
ht-degree: 5%

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
