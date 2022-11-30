---
unique-page-id: 2360350
description: 'Creación de un servicio personalizado para su uso con la API de ReST: Marketo Docs: documentación del producto'
title: Crear un servicio personalizado para utilizarlo con la API de ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Crear un servicio personalizado para utilizarlo con la API de ReST {#create-a-custom-service-for-use-with-rest-api}

Si desea integrarse con Marketo a través de la API de ReST, debe crear un servicio personalizado. Así es como.

>[!PREREQUISITES]
>
>* [Crear una función de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Crear un usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>


>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!TIP]
>
>Consulte la documentación de nuestros desarrolladores para obtener más información sobre [API de ReST](https://developers.marketo.com/documentation/rest/). También tenemos el [API SOAP](https://developers.marketo.com/documentation/soap/) si eso es lo que necesitas.

## Crear servicio personalizado {#create-custom-service}

1. Vaya a la **Administrador** .

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Haga clic en **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Select **Nuevo** y luego **Nuevo servicio**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Escriba un **Nombre para mostrar** para el servicio. Seleccione el **Usuario solo de API** [creado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Tenga en cuenta que ya tenemos integración nativa para los servicios de seminarios web más populares.

1. Haga clic en **Crear**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   ¡Oh sí! El servicio se ha creado, sigamos adelante y obtengamos todas las credenciales para proporcionar acceso.

## Credenciales para el acceso a la API {#credentials-for-api-access}

1. Vaya a la **Administrador** .

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Haga clic en **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Haga clic en **Ver detalles** para el servicio personalizado de LaunchPoint creado anteriormente.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Haga clic en **Obtener token**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Proporcione la variable **ID de cliente**, **Secreto del cliente**, **Usuario autorizado** y **Token** a la persona responsable de establecer la conexión.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>No comparta esta información; es la puerta trasera de sus datos. ¡Mantenlo a salvo!
