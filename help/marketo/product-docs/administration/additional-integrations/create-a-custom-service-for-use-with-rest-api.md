---
unique-page-id: 2360350
description: 'Creación de un servicio personalizado para su uso con la API de ReST: Marketo Docs: documentación del producto'
title: Crear un servicio personalizado para utilizarlo con la API de ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Crear un servicio personalizado para usar con la API de ReST {#create-a-custom-service-for-use-with-rest-api}

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
>Consulte la documentación de nuestros desarrolladores para obtener más información sobre la [API de ReST](https://developers.marketo.com/documentation/rest/). También tenemos la [API SOAP](https://developers.marketo.com/documentation/soap/) si es lo que necesita.

>[!NOTE]
>
>No puede crear un servicio personalizado si tiene el nivel Spark de Marketo.

## Crear servicio personalizado {#create-custom-service}

1. Vaya a **Admin** y haga clic en **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. En **Nuevo**, haga clic en **Nuevo servicio**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Introduzca un **Display Name** para el servicio. Seleccione **API Only User** [creado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >Tenga en cuenta que ya tenemos integración nativa para los servicios de seminarios web más populares.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Haga clic en **Crear**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   ¡Oh sí! El servicio se ha creado, sigamos adelante y obtengamos todas las credenciales para proporcionar acceso.

## Credenciales de acceso a API {#credentials-for-api-access}

1. Vaya a **Admin** y haga clic en **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Haga clic en **Ver detalles** para el servicio personalizado de LaunchPoint creado anteriormente.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Haga clic en **Obtener token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Proporcione el **Client Id**, **Client Secret**, **Authorized User** y el **Token** a la persona responsable del establecimiento de la conexión.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>No comparta esta información; es la puerta trasera de sus datos. ¡Mantenlo a salvo!
