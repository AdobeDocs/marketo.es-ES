---
unique-page-id: 1147031
description: Eliminar persona de SFDC - Documentos de Marketo - Documentación del producto
title: Eliminar persona de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Eliminar persona de SFDC {#delete-person-from-sfdc}

Si necesita eliminar un conjunto específico de posibles clientes de Salesforce pero dejarlos como personas en Marketo, puede utilizar la acción de flujo Eliminar persona del SFDC.

>[!NOTE]
>
>Solo está disponible cuando se integra con Salesforce.

1. En la base de datos, haga clic en la persona que desee eliminar de Salesforce. Luego haga clic en **Acciones de persona** y seleccione **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Seleccionar **Eliminar persona del SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Asegúrese de que la **Eliminar en Marketo** la configuración es **false**, luego haga clic en **Ejecutar ahora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Una vez que se ejecute el paso de flujo, su persona ya no será un posible cliente en Salesforce, pero permanecerá en Marketo.

   >[!CAUTION]
   >
   >Si establece **Eliminar en Marketo** hasta **true** y eliminar a las personas de Marketo y a los posibles clientes de Salesforce, se han ido para siempre. Esto no se puede deshacer.
