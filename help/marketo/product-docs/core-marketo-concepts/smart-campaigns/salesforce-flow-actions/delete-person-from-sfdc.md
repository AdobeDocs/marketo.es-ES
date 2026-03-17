---
unique-page-id: 1147031
description: Obtenga información sobre cómo eliminar una persona de Salesforce con un paso de flujo. Elimine el posible cliente o contacto de SFDC cuando entre en el flujo.
title: Eliminar persona de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 5%

---

# Eliminar persona de SFDC {#delete-person-from-sfdc}

Si necesita eliminar un conjunto específico de posibles clientes de Salesforce pero dejarlos como personas en Marketo Engage, puede utilizar la acción de flujo Eliminar persona de SFDC.

>[!NOTE]
>
>Solo está disponible cuando se integra con [!DNL Salesforce].

1. En la base de datos, haga clic en la persona que desee eliminar de Salesforce. Luego haga clic en **[!UICONTROL Acciones de persona]** y seleccione **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Seleccionar **[!UICONTROL Eliminar persona de SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Asegúrese de que la opción **[!UICONTROL Eliminar en Marketo]** sea **[!UICONTROL false]** y, a continuación, haga clic en **[!UICONTROL Ejecutar ahora]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Una vez que se ejecute el paso de flujo, su persona ya no será un posible cliente en [!DNL Salesforce], pero permanecerá en Marketo.

   >[!CAUTION]
   >
   >Si establece **[!UICONTROL Delete en Marketo]** en **[!UICONTROL true]** y elimina a las personas de Marketo y a los posibles clientes de Salesforce, se irán para siempre. Esto no se puede deshacer.
