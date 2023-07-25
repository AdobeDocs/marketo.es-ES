---
unique-page-id: 1147154
description: 'Sincronización de una campaña de SFDC con un programa: documentos de Marketo, documentación del producto'
title: Sincronización de una campaña de SFDC con un programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Sincronización de una campaña de SFDC con un programa {#sync-an-sfdc-campaign-with-a-program}

Marketo le permite sincronizar sus programas con campañas de Salesforce para mantener la misma lista de personas en ambos sistemas, incluidos sus estados. Comencemos!

>[!PREREQUISITES]
>
>Deberá hacer lo siguiente [habilitar sincronización de campaña de Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) primero.

>[!CAUTION]
>
>Al sincronizar una campaña de SFDC con un programa de Marketo, las acciones de SFDC implícitas (por ejemplo, agregar a la campaña de SFDC o Sincronizar con SFDC) se desactivarán para las campañas secundarias del programa.

1. Ir a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione el programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clic **Acciones de programa**, luego seleccione **Sincronización de campaña de Salesforce**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Seleccionar **Crear nuevo** o elija una campaña de Salesforce existente.

   >[!TIP]
   >
   >Si selecciona una campaña de Salesforce existente, asegúrese de lo siguiente [hacer coincidir los estados de programa de la campaña de Salesforce y del programa de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Introduzca un nombre para la nueva campaña y haga clic en **Guardar**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Ahora puede verificar los detalles de sincronización de campañas en la página de resumen del programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   ¡Excelente! Ahora, cualquier cambio de estado de programa en Marketo se sincroniza con la campaña de SFDC y viceversa.
