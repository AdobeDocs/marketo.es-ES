---
unique-page-id: 42762511
description: Configuración de la asignación de organizaciones de Adobe - Documentos de Marketo - Documentación del producto
title: Configuración de la asignación de organización de Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: 22f46fedc90d064bd7fbe6f7d5e4621de0b83718
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Configuración de la asignación de organización de Adobe {#set-up-adobe-organization-mapping}

Para sincronizar con aplicaciones de Adobe, como el Audience Manager, el conector Marketo B2B CDP, Dynamic Chat, etc., primero debe introducir sus credenciales de organización de Adobe IMS en Marketo.

>[!NOTE]
>
>Una implementación lista para HIPAA de una instancia de Marketo no puede utilizar esta integración.

>[!CAUTION]
>
>Para los clientes incorporados a Adobe Business Platform y Identity Management System, el ID de organización asociado con la suscripción ya se rellenará y es un campo de solo lectura.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. En Integración, haga clic en **Asignación de organización de Adobe**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Haga clic en **Editar**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Introduzca su ID de organización de Adobe IMS (Aprenda a encontrar que [here](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) y haga clic en **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Haga clic en **Confirmar**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Haga clic en **Cerrar**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Por motivos de seguridad, debe ser administrador de organización de la organización de Adobe a la que desee asignar. Si no lo está, la acción fallará. Además, el usuario de Adobe y el usuario de Marketo deben utilizar la misma dirección de correo electrónico al iniciar sesión.

1. Si _not_ ya ha iniciado sesión, aparecerá una ventana emergente en una nueva pestaña o ventana. Inicie sesión en la organización de Adobe (esta acción valida el acceso a la organización).

¡Y eso es todo! Ahora puede [compartir datos de audiencia](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;} para o [sincronizar una audiencia](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target=&quot;_blank&quot;} de Adobe Experience Cloud.
