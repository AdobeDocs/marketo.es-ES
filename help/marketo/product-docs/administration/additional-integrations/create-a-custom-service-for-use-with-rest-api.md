---
unique-page-id: 2360350
description: Cree un servicio de LaunchPoint personalizado vinculado a un usuario solo de API para la integración de API de ReST.
title: Creación de un servicio personalizado para utilizarlo con la API de ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 15%

---

# Creación de un servicio personalizado para utilizarlo con la API de ReST {#create-a-custom-service-for-use-with-rest-api}

Si desea integrarse con Marketo mediante la API de ReST, cree un servicio personalizado.

>[!PREREQUISITES]
>
>* [Crear un rol de usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Crear un usuario solo de API](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!TIP]
>
>Consulte la documentación para desarrolladores para obtener más información sobre la [API de REST](https://developer.adobe.com/marketo-apis/).

## Crear servicio personalizado {#create-custom-service}

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Haga clic en **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Seleccione **[!UICONTROL Nuevo]** y después **[!UICONTROL Nuevo servicio]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Escriba un **[!UICONTROL Nombre para mostrar]** para el servicio. Seleccione el **[!UICONTROL usuario solo de API]** [creado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   El servicio se ha creado. Recupere las credenciales para proporcionar acceso.

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
>No comparta esta información, ya que proporciona acceso a sus datos.
