---
unique-page-id: 1147031
description: Obtenga información sobre cómo eliminar una persona de Salesforce con un paso de flujo. Elimine el posible cliente o contacto de SFDC cuando entre en el flujo.
title: Eliminar persona de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: 'https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
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
