---
unique-page-id: 2360350
description: Creación de un servicio personalizado para su uso con la API de ReST - Documentos de marketing - Documentación del producto
title: Crear un servicio personalizado para utilizarlo con la API de ReST
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---


# Crear un servicio personalizado para utilizarlo con la API de ReST {#create-a-custom-service-for-use-with-rest-api}

Si desea realizar la integración con Marketing mediante la API de ReST, deberá crear un servicio personalizado. Así es como.

>[!NOTE]
>
>**Requisitos previos**
>
>* [Crear una función de usuario solo de API](../../../product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Crear un usuario solo de API](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**Se requieren permisos de administración**

>[!NOTE]
>
>**Buceo profundo**
>
>Consulte la documentación de nuestros desarrolladores para obtener más información sobre la API [de](http://developers.marketo.com/documentation/rest/)ReST. También tenemos la API [](http://developers.marketo.com/documentation/soap/) SOAP si es lo que necesita.

>[!NOTE]
>
>No puede crear un servicio personalizado si tiene el nivel de Spark de Marketing.

## Crear servicio personalizado {#create-custom-service}

1. Vaya a **Administración** y haga clic en **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. En **Nuevo**, haga clic en **Nuevo servicio**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Introduzca un **nombre** para mostrar para el servicio. Seleccione el usuario **solo de** API [creado](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)anteriormente.

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >Tenga en cuenta que ya contamos con integración nativa para los servicios de seminarios Web más populares.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Haga clic en **Crear**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   ¡Oh sí! Ahora se ha creado el servicio, sigamos adelante y obtengamos todas las credenciales para proporcionar acceso.

## Credenciales para el acceso a API {#credentials-for-api-access}

1. Vaya a **Administración** y haga clic en **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Haga clic en Detalles **de** Vista para el servicio LaunchPoint personalizado creado anteriormente.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Haga clic en **Obtener token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Proporcione el** ID de cliente**, el secreto **de** cliente, el usuario **** autorizado y el **autentificador** a la persona encargada de establecer la conexión.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>No comparta esta información; es la puerta trasera de tus datos. ¡Mantén la seguridad!

