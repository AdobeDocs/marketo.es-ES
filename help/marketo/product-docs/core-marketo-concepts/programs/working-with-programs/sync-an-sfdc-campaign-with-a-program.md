---
unique-page-id: 1147154
description: Sincronizar una Campaña SFDC con un Programa - Documentos de marketing - Documentación del producto
title: Sincronizar una Campaña SFDC con un Programa
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Sincronizar una Campaña SFDC con un Programa {#sync-an-sfdc-campaign-with-a-program}

Marketing le permite sincronizar sus programas con campañas de Salesforce para mantener la misma lista de personas en ambos sistemas, incluidos sus estados. ¡Empecemos!

>[!NOTE]
>
>**Requisitos previos**
>
>Tendrá que [activar primero la sincronización](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) de campañas de Salesforce.

>[!CAUTION]
>
>Al sincronizar una campaña SFDC con un programa de marketing, las acciones SFDC implícitas (por ejemplo, agregar a la Campaña SFDC, Sincronizar con SFDC) se desactivarán para las campañas secundarias del programa.

1. Vaya a Actividades **de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione su programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Haga clic en Acciones **de** Programa y, a continuación, seleccione **Sincronización** de Campaña de Salesforce.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleccione **Crear nuevo **o elija una campaña de Salesforce existente.

   >[!TIP]
   >
   >Si selecciona una campaña existente de Salesforce, asegúrese de [coincidir con los estados de programa de la campaña de Salesforce y el programa](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)de Marketing.

1. Escriba un nombre para la nueva campaña y haga clic en **Guardar**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ahora puede comprobar los detalles de sincronización de campañas en la página de resumen de programas.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   ¡Excelente! Ahora cualquier cambio de estado de programa en Marketing se sincroniza con la campaña SFDC y viceversa.

