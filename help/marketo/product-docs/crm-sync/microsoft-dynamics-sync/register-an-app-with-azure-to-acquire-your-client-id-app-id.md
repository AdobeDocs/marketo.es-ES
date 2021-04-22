---
unique-page-id: 12983390
description: 'Registre una aplicación con Azure para adquirir su ID de cliente/ID de aplicación: Marketo Docs: documentación del producto'
title: Registre una aplicación con Azure para adquirir su ID de cliente o ID de aplicación
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Registre una aplicación con Azure para adquirir su ID de cliente/ID de aplicación {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory extiende sus directorios locales a la nube, proporcionando compatibilidad con MS Dynamics 365 CRM con autenticación ADFS local.

## Registro de una nueva aplicación {#registering-a-new-app}

1. [Inicie sesión ](https://manage.windowsazure.com/) en el portal de administración de Microsoft Azure mediante una cuenta con permisos de administrador. También puede acceder al portal de Microsoft Azure a través del Centro de administración de Office 365 expandiendo el elemento **Admin** en el panel de navegación izquierdo y seleccionando **Azure AD**.

   >[!CAUTION]
   >
   >Debe utilizar una cuenta en la misma suscripción de Office 365 que la que desea registrar la aplicación.

   >[!NOTE]
   >
   >Si no tiene una cuenta de Azure, puede [registrarse](https://azure.microsoft.com/en-us/free/) para una. Consulte la documentación de Microsoft o póngase en contacto con su representante de Microsoft para obtener más información. Una vez creada una cuenta de Azure, puede registrar una o más aplicaciones mediante el procedimiento que se describe a continuación.
   >
   >
   >Si tiene una cuenta de Azure pero la suscripción de Office 365 con Microsoft Dynamics 365 no está disponible en su suscripción de Azure, siga [estas instrucciones](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) para asociar las dos cuentas.

1. Busque y haga clic en **Azure Active Directory** en el panel de navegación izquierdo.

   ![](assets/two.png)

1. En Administrar, haga clic en **Registros de aplicación**.

   ![](assets/three.png)

1. Haga clic en **New registration** en la parte superior de la página.

   ![](assets/four.png)

1. Introduzca un nombre para la aplicación, elija el tipo de cuenta aplicable e introduzca una URL de redireccionamiento. A continuación, haga clic en **Register** en la parte inferior de la página.

   ![](assets/five.png)

1. Ahora debería ver su aplicación en la pestaña **App records** .

   ![](assets/six.png)

## Configuración de permisos de aplicación {#configuring-app-permissions}

1. En la ficha **Registros de aplicación** de Active Directory, haga clic en la aplicación para la que desea configurar los permisos.

   ![](assets/seven.png)

1. En Administrar, haga clic en **Permisos de API**.

   ![](assets/eight.png)

1. Haga clic en el botón **Add a permission**.

   ![](assets/nine.png)

1. Elija **Dynamics CRM**.

   ![](assets/ten.png)

1. Marque la casilla **Access Common Data Service como usuario de organización****s** y luego haga clic en **Agregar permisos.**

   ![](assets/eleven.png)

1. Una vez agregados correctamente los permisos, espere al menos 10 segundos.

   ![](assets/twelve.png)

1. Haga clic en el botón **Grant admin permission**.

   ![](assets/thirteen.png)

1. Haga clic en **Yes** para confirmar.

   ![](assets/fourteen.png)

   ¡Y ya terminaste!

   ![](assets/fifteen.png)
