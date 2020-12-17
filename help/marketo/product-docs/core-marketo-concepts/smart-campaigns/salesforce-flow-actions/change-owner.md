---
unique-page-id: 1147021
description: Cambiar propietario - Documentos de marketing - Documentación del producto
title: Cambiar propietario
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Cambiar propietario {#change-owner}

Si ya tiene personas asignadas a un propietario, puede utilizar este paso de flujo para volver a asignarlas a otro propietario.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Uso**

1. Simplemente elija el propietario o la cola de posibles clientes a la que desea cambiar y vaya.

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce no permite que los contactos se asignen a colas de posibles clientes. Para un registro que es un contacto SFDC:
   >
   >1. Marketing creará un posible cliente de duplicado **solamente** cuando el contacto se sincronice con Salesforce. En otras palabras, si utiliza el paso de flujo **[Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** con `AssignTo=<a lead queue>`, Marketing creará un lead de duplicado en Salesforce y lo asignará a la cola de posibles clientes.
      >
      >
   2. Si intenta utilizar el paso de flujo **Cambiar propietario** en un contacto, no se creará ningún duplicado en Salesforce.


   >[!NOTE]
   >
   >Si el registro aún no existe en su cuenta de Salesforce, lo sincronizaremos de nuevo y lo asignaremos al usuario seleccionado.
