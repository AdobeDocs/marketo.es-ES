---
unique-page-id: 2360207
description: 'Creación de un usuario solo de API: documentos de Marketo, documentación del producto'
title: Crear un usuario solo de API
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Crear un usuario solo de API {#create-an-api-only-user}

Si desea integrar con Marketo a través de la [API DE REST](https://developers.marketo.com/documentation/rest/){target="_blank"}, deberá crear un usuario solo de API. Así es como.

>[!IMPORTANT]
>
>Si crea usuarios de solo API en una suscripción que se ha incorporado a Adobe Identity, los pasos son diferentes y [se puede encontrar aquí](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Crear un rol de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/create-an-api-only-user-1.png)

1. Clic **[!UICONTROL Usuarios y funciones]**.

   ![](assets/create-an-api-only-user-2.png)

1. Clic **[!UICONTROL Invitar nuevo usuario]**.

   ![](assets/create-an-api-only-user-3.png)

1. Introduzca un correo electrónico, un nombre y un apellido para el usuario solo de API. Clic **[!UICONTROL Siguiente]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Añada un motivo opcional o una fecha de caducidad para el acceso. Las fechas de caducidad del acceso son útiles para los empleados a corto plazo.

1. Seleccione el **[!UICONTROL Solo API]** función y marque la **[!UICONTROL Solo API]** casilla de verificación Clic **[!UICONTROL Siguiente]**.

   ![](assets/create-an-api-only-user-5.png)

1. Clic **[!UICONTROL Enviar]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>La ventana emergente dice: &quot;No se requiere una invitación solo para la API&quot;, pero eso no significa que haya hecho algo mal. Solo significa que crearemos la función sin tener que enviar un correo electrónico de invitación.

Muy bien, entonces! Ahora sigamos adelante y creemos el servicio personalizado.

>[!MORELIKETHIS]
>
>[Crear un servicio personalizado para utilizarlo con la API de REST](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
