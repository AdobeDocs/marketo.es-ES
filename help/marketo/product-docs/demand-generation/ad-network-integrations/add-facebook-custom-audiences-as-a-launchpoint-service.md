---
unique-page-id: 4720257
description: Agregar  [!DNL Facebook] audiencias personalizadas como servicio [!DNL LaunchPoint] Documentos de Marketo - Documentación del producto
title: Agregar  [!DNL Facebook] audiencias personalizadas como [!DNL LaunchPoint] servicio
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Agregar [!DNL Facebook] audiencias personalizadas como servicio de [!DNL LaunchPoint] {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Se requieren permisos de administración**

Con esta integración, puede enviar datos de audiencia desde listas estáticas e inteligentes de Marketo a [!DNL Facebook] para que se utilicen como audiencias personalizadas en [!DNL Facebook] campañas de publicidad. A continuación se muestra cómo configurarlo.

1. Vaya a Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vaya a **[!UICONTROL LaunchPoint]**, haga clic en **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo servicio]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Escriba un **[!UICONTROL Nombre para mostrar]** para su servicio y seleccione el servicio **[!UICONTROL Audiencias personalizadas de Facebook]** de la lista desplegable **[!UICONTROL Servicio]**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Abra una ficha nueva en el mismo explorador y vaya a [facebook.com](https://www.facebook.com/). Inicie sesión en [!DNL Facebook] con la cuenta que desee usar para la integración.

   >[!CAUTION]
   >
   >Para que Marketo envíe audiencias a través de varias cuentas de Ad Manager, el usuario [!DNL Facebook] que autorizó en los siguientes pasos necesita tener acceso a *todas* estas cuentas.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Una vez que haya iniciado sesión en [!DNL Facebook], vuelva a Marketo. Haga clic en **[!UICONTROL Autorizar]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Usted _debe_ usar una cuenta de [!DNL Facebook] Business Manager para que funcione su integración de audiencias personalizadas. Para aprender a configurar una cuenta de Business Manager, consulte [[!DNL Facebook] Ayuda](https://www.facebook.com/business/help/1710077379203657).

1. Si se le solicita, haga clic en **[!UICONTROL Aceptar]** para aceptar la instalación de la aplicación Marketo en [!DNL Facebook].

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. ¡Ya está autorizado! Seleccione un modo que coincida y haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >**[!UICONTROL Coincidencia básica]** solo usa direcciones de correo electrónico. **[!UICONTROL Coincidencia avanzada]** usa siete campos adicionales, lo que aumenta la tasa de coincidencia, para obtener más conversión. Sin embargo, si la directiva de privacidad de la compañía no permite compartir campos adicionales o si los datos no los incluyen, seleccione [!UICONTROL Coincidencia básica].

   ![](assets/fb-custom-adv-matching-hands.png)

   ¡Buen trabajo! Ahora puede pasar a cualquier lista estática o inteligente en Marketo y enviar datos de audiencia a [!DNL Facebook].

   >[!CAUTION]
   >
   >¡Antes de irte, asegúrate de [aceptar [!DNL Facebook] los términos de audiencias personalizadas](https://www.facebook.com/ads/manage/customaudiences/tos.php) en tu cuenta de [!DNL Facebook]! Sin hacerlo, las actualizaciones de audiencia fallarán.

>[!MORELIKETHIS]
>
>* [Crear una audiencia personalizada en [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurar [!DNL Facebook] Anuncios Posibles Clientes](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
