---
unique-page-id: 1147031
description: Eliminar persona de SFDC - Marketo Docs - Documentación del producto
title: Eliminar persona de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Eliminar persona de SFDC {#delete-person-from-sfdc}

Si necesita eliminar un conjunto específico de posibles clientes de Salesforce pero déjelos como personas en Marketo, puede utilizar la acción de flujo Eliminar persona de SFDC .

>[!NOTE]
>
>Solo disponible cuando se integra con Salesforce.

1. En la base de datos, haga clic en la persona que desee eliminar de Salesforce. A continuación, haga clic en **Acciones de persona** y seleccione **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Select **Eliminar persona de SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Asegúrese de que la variable **Eliminar en Marketo** configurar es **false** y haga clic en **Ejecutar ahora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Una vez que se ejecute el paso de flujo, su persona ya no será líder en Salesforce, pero permanecerá en Marketo.

   >[!CAUTION]
   >
   >Si configura **Eliminar en Marketo** a **true** y borran a las personas de Marketo y a los posibles clientes de Salesforce, se han ido para siempre. Esto no se puede deshacer.
