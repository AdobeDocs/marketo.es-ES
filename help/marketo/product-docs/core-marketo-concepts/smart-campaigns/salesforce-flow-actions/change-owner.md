---
unique-page-id: 1147021
description: Cambiar propietario - Documentos de Marketo - Documentación del producto
title: Cambiar propietario
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Cambiar propietario {#change-owner}

Si tiene personas existentes que ya están asignadas a un propietario, puede utilizar este paso de flujo para reasignarlas a otro propietario.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Uso**

1. Simplemente elija el propietario o la cola de posibles clientes a la que desee cambiar y vaya.

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce no permite asignar contactos a colas de posibles clientes. Para un registro que sea un contacto SFDC:
   >
   >1. Marketo creará un posible cliente duplicado **only** cuando el contacto se sincronice con Salesforce. En otras palabras, si utiliza el paso de flujo **[Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketo creará un posible cliente duplicado en Salesforce y lo asignará a la cola de posibles clientes.
      >
      >
   1. Si intenta utilizar el paso de flujo **Cambiar propietario** en un contacto, no se creará ningún duplicado en Salesforce.


   >[!NOTE]
   >
   >Si el registro aún no existe en su cuenta de Salesforce, lo sincronizaremos de nuevo y lo asignaremos al usuario seleccionado.
