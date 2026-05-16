---
unique-page-id: 1147154
description: Obtenga información sobre cómo sincronizar una campaña de Salesforce con un programa de Marketo. Mantener el estado de miembro sincronizado entre SFDC y Marketo.
title: Sincronización de una campaña de SFDC con un programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
TQID: https://experienceleague.adobe.com/WUVAKa2NMKLuT0t-Z-VJLqsnJBa7x7bYir8ORqUnmpU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 11%

---

# Sincronización de una campaña de SFDC con un programa {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage le permite sincronizar sus programas con [!DNL Salesforce] campañas para mantener la misma lista de personas en ambos sistemas, incluidos sus estados. ¡Empecemos!

>[!PREREQUISITES]
>
>Primero tendrá que [habilitar [!DNL Salesforce] la sincronización de campaña](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.

>[!CAUTION]
>
>Al sincronizar una campaña de SFDC con un programa de Marketo Engage, las acciones de SFDC implícitas (por ejemplo, agregar a SFDC Campaign, Sincronizar con SFDC) se desactivan para las campañas secundarias del programa.

1. Vaya a **[!UICONTROL Actividades de marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione el programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Haga clic en **[!UICONTROL Acciones del programa]** y, a continuación, seleccione **[!UICONTROL Sincronización de Salesforce Campaign]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleccione **[!UICONTROL Crear nuevo]** o elija una campaña [!DNL Salesforce] existente.

   >[!TIP]
   >
   >Si selecciona una campaña [!DNL Salesforce] existente, asegúrese de [coincidir con los estados de programa de la  [!DNL Salesforce] campaña y el programa de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. Escriba un nombre para la nueva campaña y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ahora puede verificar los detalles de sincronización de campañas en la página de resumen del programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Los cambios de estado del programa en Marketo ahora se sincronizan con la campaña de SFDC y viceversa.
