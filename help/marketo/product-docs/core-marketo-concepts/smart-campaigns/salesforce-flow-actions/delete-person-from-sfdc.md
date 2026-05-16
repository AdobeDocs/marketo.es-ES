---
unique-page-id: 1147031
description: Obtenga información sobre cómo eliminar una persona de Salesforce con un paso de flujo. Elimine el posible cliente o contacto de SFDC cuando entre en el flujo.
title: Eliminar persona de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
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
