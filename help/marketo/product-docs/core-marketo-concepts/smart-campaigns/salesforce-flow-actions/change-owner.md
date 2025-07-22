---
unique-page-id: 1147021
description: Cambiar propietario - Documentos de Marketo - Documentación del producto
title: Cambiar propietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
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
