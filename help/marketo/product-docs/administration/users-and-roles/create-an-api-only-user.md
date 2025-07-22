---
unique-page-id: 2360207
description: 'Creación de un usuario solo de API: documentos de Marketo, documentación del producto'
title: Crear un usuario solo de API
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Crear un usuario solo de API {#create-an-api-only-user}

Si desea integrarse con Marketo a través de la [API REST](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}, deberá crear un usuario solo de API. Así es como.

>[!IMPORTANT]
>
>Si va a crear usuarios con solo API en una suscripción que se ha incorporado a Adobe Identity, los pasos son diferentes y [se pueden encontrar aquí](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Crear un rol de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-an-api-only-user-1.png)

1. Haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/create-an-api-only-user-2.png)

1. Haga clic en **[!UICONTROL Invitar nuevo usuario]**.

   ![](assets/create-an-api-only-user-3.png)

1. Introduzca un correo electrónico, un nombre y un apellido para el usuario solo de API. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Agregue un [!UICONTROL Motivo] opcional o una fecha de [!UICONTROL caducidad del acceso]. Las fechas de caducidad del acceso son útiles para los empleados a corto plazo.

1. Seleccione el rol **[!UICONTROL Solo API]** y marque la casilla **[!UICONTROL Solo API]**. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/create-an-api-only-user-5.png)

1. Haga clic en **[!UICONTROL Enviar]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>La ventana emergente dice: &quot;No se requiere una invitación solo para la API&quot;, pero eso no significa que haya hecho algo mal. Solo significa que crearemos la función sin tener que enviar un correo electrónico de invitación.

Muy bien, entonces! Ahora sigamos adelante y creemos el servicio personalizado.

>[!MORELIKETHIS]
>
>[Crear un servicio personalizado para utilizarlo con la API de REST](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
