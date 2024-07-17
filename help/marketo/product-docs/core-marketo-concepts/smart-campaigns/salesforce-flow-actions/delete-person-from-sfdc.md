---
unique-page-id: 1147031
description: Eliminar persona de SFDC - Documentos de Marketo - Documentación del producto
title: Eliminar persona de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Eliminar persona de SFDC {#delete-person-from-sfdc}

Si necesita eliminar un conjunto específico de posibles clientes de Salesforce pero dejarlos como personas en Marketo Engage, puede utilizar la acción de flujo Eliminar persona del SFDC.

>[!NOTE]
>
>Solo está disponible cuando se integra con Salesforce.

1. En la base de datos, haga clic en la persona que desee eliminar de Salesforce. Luego haga clic en **[!UICONTROL Acciones de persona]** y seleccione **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Seleccione **[!UICONTROL Eliminar persona del SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Asegúrese de que la opción **[!UICONTROL Eliminar en Marketo]** sea **[!UICONTROL false]** y, a continuación, haga clic en **[!UICONTROL Ejecutar ahora]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Una vez que se ejecute el paso de flujo, su persona ya no será un posible cliente en Salesforce, pero permanecerá en Marketo.

   >[!CAUTION]
   >
   >Si establece **[!UICONTROL Delete en Marketo]** en **[!UICONTROL true]** y elimina a las personas de Marketo y a los posibles clientes de Salesforce, se irán para siempre. Esto no se puede deshacer.
