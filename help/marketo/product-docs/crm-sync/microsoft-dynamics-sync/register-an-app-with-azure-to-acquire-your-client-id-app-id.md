---
unique-page-id: 12983390
description: Registre una aplicación con Azure para adquirir su ID de cliente/ID de aplicación - Documentos de marketing - Documentación del producto
title: Registrar una aplicación con Azure para adquirir el ID de cliente o de aplicación
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Registre una aplicación con Azure para adquirir el ID de cliente o de aplicación {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory amplía los directorios locales a la nube, lo que proporciona compatibilidad con MS Dynamics 365 CRM con autenticación ADFS local.

## Registro de una nueva aplicación {#registering-a-new-app}

1. [Inicie sesión ](https://manage.windowsazure.com/) en el portal de administración de Microsoft Azure con una cuenta con permisos de administrador. También puede acceder al portal de Microsoft Azure a través del Centro de administración de Office 365 si expande el elemento **Administrador** en el panel de navegación izquierdo y selecciona **Azure AD**.

   >[!CAUTION]
   >
   >Debe usar una cuenta en la misma suscripción de Office 365 que la que desea registrar la aplicación.

   >[!NOTE]
   >
   >Si no tiene una cuenta de Azure, puede [registrarse](https://azure.microsoft.com/en-us/free/) para una. Consulte la documentación de Microsoft o póngase en contacto con su representante de Microsoft para obtener más información. Una vez que haya creado una cuenta de Azure, puede registrar una o varias aplicaciones mediante el procedimiento que se describe a continuación.
   >
   >
   >Si tiene una cuenta de Azure pero la suscripción de Office 365 con Microsoft Dynamics 365 no está disponible en su suscripción de Azure, siga [estas instrucciones](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) para asociar las dos cuentas.

1. Busque y haga clic en **Azure Active Directory** en el panel de navegación izquierdo.

   ![](assets/two.png)

1. En Administrar, haga clic en **Registros de aplicaciones**.

   ![](assets/three.png)

1. Haga clic en **Nuevo registro** en la parte superior de la página.

   ![](assets/four.png)

1. Escriba un nombre para la aplicación, elija el tipo de cuenta que corresponda e introduzca una URL de redirección. A continuación, haga clic en **Registrarse** en la parte inferior de la página.

   ![](assets/five.png)

1. Ahora debería ver su aplicación en la ficha **Registros de la aplicación**.

   ![](assets/six.png)

## Configuración de los permisos de la aplicación {#configuring-app-permissions}

1. En la ficha **Registros de aplicación** de Active Directory, haga clic en la aplicación para la que desee configurar los permisos.

   ![](assets/seven.png)

1. En Administrar, haga clic en **Permisos de API**.

   ![](assets/eight.png)

1. Haga clic en el botón **Añadir un permiso**.

   ![](assets/nine.png)

1. Elija **Dynamics CRM**.

   ![](assets/ten.png)

1. Marque la casilla **Acceso a servicios comunes de datos como usuario de la organización****s** y luego haga clic en **Añadir permisos.**

   ![](assets/eleven.png)

1. Una vez agregados correctamente los permisos, espere al menos 10 segundos.

   ![](assets/twelve.png)

1. Haga clic en el botón **Conceder consentimiento de administrador**.

   ![](assets/thirteen.png)

1. Haga clic en **Sí** para confirmar.

   ![](assets/fourteen.png)

   ¡Y ya terminaste!

   ![](assets/fifteen.png)

