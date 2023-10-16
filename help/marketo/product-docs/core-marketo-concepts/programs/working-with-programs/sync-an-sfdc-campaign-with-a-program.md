---
unique-page-id: 1147154
description: 'Sincronización de una campaña de SFDC con un programa: documentos de Marketo, documentación del producto'
title: Sincronización de una campaña de SFDC con un programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Sincronización de una campaña de SFDC con un programa {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage le permite sincronizar sus programas con [!DNL Salesforce] campañas para mantener la misma lista de personas en ambos sistemas, incluidos sus estados. Comencemos!

>[!PREREQUISITES]
>
>Deberá hacer lo siguiente [habilitar [!DNL Salesforce] sincronización de campaña](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) primero.

>[!CAUTION]
>
>Al sincronizar una campaña de SFDC con un programa de Marketo Engage, las acciones de SFDC implícitas (por ejemplo, agregar a la campaña de SFDC o Sincronizar con SFDC) se desactivarán para las campañas secundarias del programa.

1. Ir a **[!UICONTROL Actividades de marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione el programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clic **[!UICONTROL Acciones de programa]**, luego seleccione **[!UICONTROL Sincronización de campaña de Salesforce]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleccionar **[!UICONTROL Crear nuevo]** o elija una campaña de Salesforce existente.

   >[!TIP]
   >
   >Si selecciona una campaña de Salesforce existente, asegúrese de lo siguiente [hacer coincidir los estados de programa de la campaña de Salesforce y del programa de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Introduzca un nombre para la nueva campaña y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ahora puede verificar los detalles de sincronización de campañas en la página de resumen del programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   ¡Excelente! Ahora, cualquier cambio de estado de programa en Marketo se sincroniza con la campaña de SFDC y viceversa.
