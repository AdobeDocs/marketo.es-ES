---
unique-page-id: 1147154
description: Sincronización de una campaña SFDC con un programa - Marketo Docs - Documentación del producto
title: Sincronización de una campaña SFDC con un programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Sincronización de una campaña SFDC con un programa {#sync-an-sfdc-campaign-with-a-program}

Marketo le permite sincronizar sus programas con campañas de Salesforce para mantener la misma lista de personas en ambos sistemas, incluidos sus estados. ¡Empecemos!

>[!PREREQUISITES]
>
>Primero deberá [habilitar la sincronización de campañas de Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).

>[!CAUTION]
>
>Al sincronizar una campaña de SFDC con un programa de Marketo, las acciones de SFDC implícitas (por ejemplo, agregar a la campaña de SFDC, Sincronizar con SFDC) se desactivarán para las campañas secundarias del programa.

1. Vaya a **Marketing Activities**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione el programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Haga clic en **Acciones de programa** y, a continuación, seleccione **Salesforce Campaign Sync**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleccione **Crear nuevo** o elija una campaña de Salesforce existente.

   >[!TIP]
   >
   >Si selecciona una campaña de Salesforce existente, asegúrese de [coincidir con los estados de programa de la campaña de Salesforce y del programa de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Introduzca un nombre para la nueva campaña y haga clic en **Save**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ahora puede verificar los detalles de sincronización de campañas en la página de resumen del programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   ¡Excelente! Ahora, cualquier cambio de estado del programa en Marketo se sincroniza con la campaña de SFDC y viceversa.
