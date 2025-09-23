---
unique-page-id: 12983390
description: 'Registre una aplicación con Azure para adquirir su ID de cliente o ID de aplicación: documentos de Marketo, documentación del producto'
title: Registrar una aplicación con Azure para adquirir su ID de cliente o ID de aplicación
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 7%

---

# Registrar una aplicación con Azure para adquirir su ID de cliente o ID de aplicación {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory extiende sus directorios locales a la nube, lo que proporciona compatibilidad con [!DNL MS Dynamics 365] CRM con autenticación ADFS local.

## Registro de una aplicación nueva {#registering-a-new-app}

1. [Inicie sesión](https://login.microsoftonline.com/){target="_blank"} en el portal de administración de Microsoft Azure con una cuenta con permisos de administrador. También puede obtener acceso al portal de Microsoft Azure a través del Centro de administración de Office 365. Para ello, expanda el elemento **[!UICONTROL Admin]** en el panel de navegación izquierdo y seleccione **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >Debe utilizar una cuenta con la misma suscripción [!DNL Office 365] con la que desea registrar la aplicación.

   >[!NOTE]
   >
   >Si no tiene una cuenta de Azure, puede [registrarse](https://azure.microsoft.com/en-us/free/){target="_blank"} para obtener una. Consulte la documentación de Microsoft o póngase en contacto con su representante de Microsoft para obtener más información. Una vez creada una cuenta de Azure, puede registrar una o más aplicaciones mediante el procedimiento que se describe a continuación.
   >
   >
   >Si tiene una cuenta de Azure pero su suscripción de [!DNL Office 365] con [!DNL Microsoft Dynamics 365] no está disponible en su suscripción de Azure, siga [estas instrucciones](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} para asociar las dos cuentas.

1. Busque **[!UICONTROL Azure Active Directory]** y haga clic en él en el panel de navegación izquierdo.

   ![](assets/two.png)

1. En [!UICONTROL Administrar], haga clic en **[!UICONTROL Registros de aplicaciones]**.

   ![](assets/three.png)

1. Haga clic en **[!UICONTROL Nuevo registro]** en la parte superior de la página.

   ![](assets/four.png)

1. Escriba un nombre para la aplicación, elija el tipo de cuenta aplicable e introduzca una URL de redireccionamiento. Luego haz clic en **[!UICONTROL Registrar]** en la parte inferior de la página.

   ![](assets/five.png)

1. Ahora debería ver su aplicación en la ficha **[!UICONTROL Registros de aplicaciones]**.

   ![](assets/six.png)

## Configuración de permisos de aplicaciones {#configuring-app-permissions}

1. En la ficha **[!UICONTROL Registros de aplicaciones]** de Active Directory, haga clic en la aplicación para la que desee configurar permisos.

   ![](assets/seven.png)

1. En [!UICONTROL Administrar], haga clic en **[!UICONTROL Permisos de API]**.

   ![](assets/eight.png)

1. Haga clic en el botón **[!UICONTROL Agregar un permiso]**.

   ![](assets/nine.png)

1. Elija **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Marque la casilla **[!UICONTROL Acceder al servicio de datos comunes como usuarios de la organización]** y luego haga clic en **[!UICONTROL Agregar permisos].**

   ![](assets/eleven.png)

1. Una vez que los permisos se hayan agregado correctamente, espere al menos 10 segundos.

   ![](assets/twelve.png)

1. Haga clic en el botón **[!UICONTROL Conceder consentimiento de administrador]**.

   ![](assets/thirteen.png)

1. Haga clic en **[!UICONTROL Sí]** para confirmar.

   ![](assets/fourteen.png)

   ¡Y has terminado!

   ![](assets/fifteen.png)
