---
unique-page-id: 42762511
description: Configuración de la asignación de organizaciones de Adobe - Documentos de Marketo - Documentación del producto
title: Configurar asignación de organización de Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: dd4fb7dfc92580c58da70d603b6d92bd8f64493c
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Configurar asignación de organización de Adobe {#set-up-adobe-organization-mapping}

Para sincronizarse con aplicaciones de Adobe, como Audience Manager, el conector de Marketo B2B CDP, [!DNL Dynamic Chat], etc., primero debe introducir las credenciales de la organización IMS de Adobe en Marketo.

>[!NOTE]
>
>Una implementación compatible con HIPAA de una instancia de Marketo no puede utilizar esta integración.

>[!CAUTION]
>
>Para los clientes incorporados a Adobe Business Platform y Identity Management System, el ID de organización asociado con la suscripción ya se rellenará y es un campo de solo lectura.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. En Integración, haga clic en **[!UICONTROL Asignación de organización de Adobe]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Clic **[!UICONTROL Editar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Introduzca su ID de organización de Adobe IMS (aprenda a encontrar eso) [aquí](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) y haga clic en **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Clic **[!UICONTROL Confirmar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Haga clic en **[!UICONTROL Cerrar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Por motivos de seguridad, debe ser administrador de organización de la organización de Adobe a la que desee asignar. Si no lo está, la acción fallará. Además, el usuario de Adobe y el usuario de Marketo deben utilizar la misma dirección de correo electrónico al iniciar sesión.

1. Si usted es _no_ ya ha iniciado sesión, aparecerá un elemento emergente en una nueva pestaña o ventana. Inicie sesión en la organización de Adobe (esta acción valida el acceso a la organización).

¡Y eso es todo! Ahora puede [compartir datos de audiencia](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} to, or [sync an audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} de Adobe Experience Cloud.
