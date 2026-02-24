---
unique-page-id: 2360350
description: 'Creación de un servicio personalizado para su uso con la API de ReST: documentos de Marketo: documentación del producto'
title: Creación de un servicio personalizado para utilizarlo con la API de ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 7f8968210659ed2c51640966115f22da47e42ebf
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 12%

---

# Creación de un servicio personalizado para utilizarlo con la API de ReST {#create-a-custom-service-for-use-with-rest-api}

Si desea integrarse con Marketo a través de la API de ReST, debe crear un servicio personalizado. Así es cómo se hace.

>[!PREREQUISITES]
>
>* [Crear un rol de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Crear un usuario solo de API](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md)
>

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!TIP]
>
>Consulte nuestra documentación para desarrolladores para obtener más información sobre la [API de REST](https://developer.adobe.com/marketo-apis/). También tenemos la [API de SOAP](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/soap/soap-api) si es lo que necesita.

## Crear servicio personalizado {#create-custom-service}

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Haga clic en **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Seleccione **[!UICONTROL Nuevo]** y después **[!UICONTROL Nuevo servicio]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Escriba un **[!UICONTROL Nombre para mostrar]** para el servicio. Seleccione el **[!UICONTROL usuario solo de API]** [creado anteriormente](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Tenga en cuenta que ya tenemos la integración nativa para los servicios de seminarios web populares.

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   ¡Ah, sí! El servicio ya se ha creado. Vamos a obtener todas las credenciales para proporcionar el acceso.

## Credenciales para el acceso a API {#credentials-for-api-access}

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Haga clic en **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Haga clic en **[!UICONTROL Ver detalles]** para el servicio [!UICONTROL LaunchPoint] personalizado creado anteriormente.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Haga clic en **[!UICONTROL Obtener token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Proporcione el **[!UICONTROL ID de cliente]**, **[!UICONTROL Secreto de cliente]**, **[!UICONTROL Usuario autorizado]** y **[!UICONTROL Token]** a la persona responsable de establecer la conexión.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>No comparta esta información; es la puerta trasera de sus datos. ¡Mantenlo a salvo!
