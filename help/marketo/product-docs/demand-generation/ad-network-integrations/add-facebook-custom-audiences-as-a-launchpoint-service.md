---
unique-page-id: 4720257
description: 'Añadir audiencias personalizadas de Facebook as a LaunchPoint Service: documentos de Marketo: documentación del producto'
title: Añadir audiencias personalizadas de Facebook como servicio de LaunchPoint
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Añadir audiencias personalizadas de Facebook como servicio de LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Permisos de administración necesarios**

Con esta integración, puede enviar datos de audiencia de listas estáticas e inteligentes de Marketo a Facebook para utilizarlos como audiencias personalizadas en campañas de publicidad de Facebook. A continuación se muestra cómo configurarlo.

1. Ir a Marketo **Administrador**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Ir a **LaunchPoint**, haga clic en **Nuevo** y seleccione **Nuevo servicio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Introduzca una **Nombre para mostrar** para el servicio y seleccione la **Audiencias personalizadas de facebook** servicio desde el **Servicio** menú desplegable.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Abra una pestaña nueva en el mismo explorador y vaya a [facebook.com](https://www.facebook.com/). Inicie sesión en Facebook con la cuenta que desee utilizar para la integración.

   >[!CAUTION]
   >
   >Para que Marketo envíe audiencias a través de varias cuentas de Ad Manager, el usuario de Facebook que autorice en los siguientes pasos debe tener acceso a *todo* de estas cuentas.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Una vez que haya iniciado sesión en Facebook, vuelva a Marketo. Clic **Autorizar**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Usted _debe_ use una cuenta de Facebook Business Manager para que funcione la integración de Audiencias personalizadas. Para aprender a configurar una cuenta de Business Manager, consulte [Ayuda de facebook](https://www.facebook.com/business/help/1710077379203657).

1. Si se le solicita, haga clic en **OK** para aceptar la instalación de la aplicación de Marketo en Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. ¡Ya está autorizado! Seleccione un modo coincidente y haga clic en **Crear**.

   >[!NOTE]
   >
   >**Coincidencia básica** solo utiliza direcciones de correo electrónico. **Coincidencia avanzada** utiliza siete campos adicionales, lo que aumenta la tasa de coincidencia, para obtener más conversión. Sin embargo, si la política de privacidad de su empresa no permite compartir campos adicionales o si los datos no los incluyen, seleccione Coincidencia básica.

   ![](assets/fb-custom-adv-matching-hands.png)

   ¡bueno trabajo! Ahora puede pasar a cualquier lista estática o inteligente en Marketo y enviar datos de audiencia a Facebook.

   >[!CAUTION]
   >
   >Antes de que te vayas, asegúrate de [Acepte los términos de audiencias personalizadas de Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) en su cuenta de Facebook. Sin hacerlo, las actualizaciones de audiencia fallarán.

>[!MORELIKETHIS]
>
>* [Crear una audiencia personalizada en Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurar anuncios de posibles clientes de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
