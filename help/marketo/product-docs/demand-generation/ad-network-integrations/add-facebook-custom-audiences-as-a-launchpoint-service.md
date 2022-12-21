---
unique-page-id: 4720257
description: 'Añadir Audiencias personalizadas de Facebook como un servicio de LaunchPoint: Documentos de Marketo: Documentación del producto'
title: Añadir Audiencias personalizadas de Facebook como un servicio de LaunchPoint
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Añadir Audiencias personalizadas de Facebook como un servicio de LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Con esta integración, puede enviar datos de audiencia desde listas estáticas e inteligentes de Marketo a Facebook para que se utilicen como audiencias personalizadas en campañas de anuncios de Facebook. Así es como configurarlo.

1. Vaya a Marketo **Administrador**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vaya a **LaunchPoint**, haga clic en **Nuevo** y seleccione **Nuevo servicio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Escriba un **Nombre para mostrar** para su servicio y seleccione la **Audiencias personalizadas de facebook** del **Servicio** lista desplegable.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Abra una nueva pestaña en el mismo explorador y vaya a [facebook.com](https://www.facebook.com/). Inicie sesión en Facebook con la cuenta que desee utilizar para la integración.

   >[!CAUTION]
   >
   >Para que Marketo envíe audiencias en varias cuentas de Administrador de anuncios, el usuario de Facebook que autorice en los pasos siguientes debe tener acceso a *all* de estas cuentas.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Una vez que haya iniciado sesión en Facebook, vuelva a Marketo. Haga clic en **Autorizar**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >You _must_ utilice una cuenta de Facebook Business Manager para que funcione la integración de Audiencias personalizadas. Para obtener información sobre cómo configurar una cuenta de Business Manager, consulte [Ayuda de facebook](https://www.facebook.com/business/help/1710077379203657).

1. Si se le solicita, haga clic en **OK** para aceptar la instalación de la aplicación de Marketo en Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. ¡Ya estás autorizado! Seleccione un modo coincidente y haga clic en **Crear**.

   >[!NOTE]
   >
   >**Coincidencia básica** solo utiliza direcciones de correo electrónico. **Coincidencia avanzada** utiliza siete campos adicionales, lo que aumenta la tasa de coincidencia, para obtener más conversión. Sin embargo, si la política de privacidad de su empresa no permite compartir campos adicionales o si los datos no los incluyen, seleccione Coincidencia básica.

   ![](assets/fb-custom-adv-matching-hands.png)

   ¡bueno trabajo! Ahora puede pasar a cualquier lista estática o inteligente de Marketo y enviar datos de audiencia a Facebook.

   >[!CAUTION]
   >
   >Oh, antes de ir, asegúrese de [Aceptar términos de audiencias personalizadas de Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) en su cuenta de Facebook Sin ello, las actualizaciones de audiencia fallarán.

>[!MORELIKETHIS]
>
>* [Crear una audiencia personalizada en Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configuración de anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

