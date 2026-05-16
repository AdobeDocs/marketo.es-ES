---
unique-page-id: 1147021
description: Aprenda a cambiar el propietario de Salesforce en un paso de flujo. Asigne un nuevo posible cliente o propietario de contacto cuando las personas entren en el flujo.
title: Cambiar propietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/VU0fT4giNqfkF5g15q0IGIh8XuO2505nz89UuUfqZro
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 2%

---

# Cambiar propietario {#change-owner}

Si tiene personas existentes que ya están asignadas a un propietario, puede utilizar este paso de flujo para reasignarlas a otro propietario.

![](assets/change-owner-1.png)

1. Simplemente elija el propietario o la cola de posibles clientes a la que desee cambiar y vaya.

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce] no permite que los contactos se asignen a colas de posibles clientes. Para un registro que sea un contacto de SFDC:
   >
   >* Marketo creará un posible cliente **solo** duplicado cuando el contacto se sincronice con Salesforce. En otras palabras, si usa el paso de flujo **[Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketo creará un posible cliente duplicado en Salesforce y lo asignará a la cola de posibles clientes.
   >
   >* Si usa el paso de flujo **[!UICONTROL Cambiar propietario]** en un contacto, Marketo crea un posible cliente duplicado en Salesforce. Para evitarlo, utilice un filtro en el campo &quot;Tipo de SFDC&quot; que limite la acción únicamente a los posibles clientes.

   >[!NOTE]
   >
   >Si el registro aún no existe en su cuenta de [!DNL Salesforce], lo sincronizaremos y lo asignaremos al usuario seleccionado.
