---
unique-page-id: 42762511
description: Obtenga información sobre cómo configurar la asignación de organización de Adobe en Marketo Engage para sincronizarla con Audience Manager y otras aplicaciones de Adobe.
title: Configuración de la asignación de organización de Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
TQID: https://experienceleague.adobe.com/8Pypw9omyxldMxJqHj-KHBRzl-P5ttDhujCwcEVfLwQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 6%

---

# Configuración de la asignación de organización de Adobe {#set-up-adobe-organization-mapping}

Para sincronizar con aplicaciones de Adobe, como Audience Manager, el conector de Marketo B2B CDP, [!DNL Dynamic Chat], etc., primero debe introducir las credenciales de su organización de IMS de Adobe en Marketo Engage.

>[!NOTE]
>
>* Una implementación compatible con HIPAA de una instancia de Marketo no puede utilizar esta integración.
>* Para que la integración funcione, Marketo y las demás aplicaciones de Adobe deben estar en la misma organización.

>[!IMPORTANT]
>
>Para los que se hayan incorporado a Adobe Business Platform y Identity Management System, el ID de organización asociado con la suscripción ya se rellenará y es un campo de solo lectura. Como tal, los pasos de este artículo no se aplicarían.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. En Integración, haga clic en **[!UICONTROL Asignación de organizaciones de Adobe]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Escriba su [ID de organización de Adobe IMS](https://experienceleague.adobe.com/docs/control-panel/using/faq.html?lang=es){target="_blank"}) y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Haga clic en **[!UICONTROL Confirmar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Por motivos de seguridad, debe ser administrador de organización de la organización de Adobe a la que desee asignar. Si no lo está, la acción fallará. Además, el usuario de Adobe y el usuario de Marketo deben utilizar la misma dirección de correo electrónico al iniciar sesión.

1. Si _no_ ha iniciado sesión, aparecerá una ventana emergente en una nueva pestaña o ventana. Inicie sesión en su organización de Adobe (esta acción valida el acceso a la organización).

Ahora puede [compartir datos de audiencia](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} con o [sincronizar una audiencia](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} desde Adobe Experience Cloud.
