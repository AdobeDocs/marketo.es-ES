---
unique-page-id: 12983390
description: 'Registre una aplicación con Azure para adquirir su ID de cliente o ID de aplicación: documentos de Marketo, documentación del producto'
title: Registre una aplicación con Azure para adquirir su ID de cliente o ID de aplicación
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Registre una aplicación con Azure para adquirir su ID de cliente o ID de aplicación {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory amplía los directorios locales en la nube y proporciona compatibilidad con MS Dynamics 365 CRM con autenticación ADFS local.

## Registro de una aplicación nueva {#registering-a-new-app}

1. [Iniciar sesión](https://login.microsoftonline.com/){target="_blank"} al portal de administración de Microsoft Azure con una cuenta con permisos de administrador. También puede acceder al portal de Microsoft Azure a través del Centro de administración de Office 365 si expande el **[!UICONTROL Administrador]** en el panel de navegación izquierdo y seleccione **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >Debe utilizar una cuenta con la misma suscripción de Office 365 con la que desea registrar la aplicación.

   >[!NOTE]
   >
   >Si no tiene una cuenta de Azure, puede [apuntarse](https://azure.microsoft.com/en-us/free/){target="_blank"} para empezar. Consulte la documentación de Microsoft o póngase en contacto con su representante de Microsoft para obtener más información. Una vez creada una cuenta de Azure, puede registrar una o más aplicaciones mediante el procedimiento que se describe a continuación.
   >
   >
   >Si tiene una cuenta de Azure pero su suscripción de Office 365 con Microsoft Dynamics 365 no está disponible en su suscripción de Azure, siga [estas instrucciones](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} para asociar las dos cuentas.

1. Busque y haga clic en **[!UICONTROL Azure Active Directory]** en el panel de navegación izquierdo.

   ![](assets/two.png)

1. En Administrar, haga clic en **[!UICONTROL Registros de aplicaciones]**.

   ![](assets/three.png)

1. Clic **[!UICONTROL Nuevo registro]** en la parte superior de la página.

   ![](assets/four.png)

1. Escriba un nombre para la aplicación, elija el tipo de cuenta aplicable e introduzca una URL de redireccionamiento. Luego haga clic en **[!UICONTROL Registrar]** en la parte inferior de la página.

   ![](assets/five.png)

1. Ahora debería ver su aplicación en la **[!UICONTROL Registros de aplicaciones]** pestaña.

   ![](assets/six.png)

## Configuración de permisos de aplicaciones {#configuring-app-permissions}

1. En el **[!UICONTROL Registros de aplicaciones]** en su Active Directory, haga clic en la aplicación para la que desee configurar permisos.

   ![](assets/seven.png)

1. En Administrar, haga clic en **[!UICONTROL Permisos de API]**.

   ![](assets/eight.png)

1. Haga clic en **[!UICONTROL Añadir un permiso]** botón.

   ![](assets/nine.png)

1. Elegir **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Compruebe la **[!UICONTROL Acceso al servicio común de datos como usuarios de la organización]** y haga clic en **[!UICONTROL Añadir permisos]**.

   ![](assets/eleven.png)

1. Una vez que los permisos se hayan agregado correctamente, espere al menos 10 segundos.

   ![](assets/twelve.png)

1. Haga clic en **[!UICONTROL Conceder consentimiento de administrador]** botón.

   ![](assets/thirteen.png)

1. Clic **[!UICONTROL Sí]** para confirmar.

   ![](assets/fourteen.png)

   ¡Y has terminado!

   ![](assets/fifteen.png)
