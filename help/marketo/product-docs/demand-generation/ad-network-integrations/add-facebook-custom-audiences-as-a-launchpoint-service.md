---
unique-page-id: 4720257
description: Aprenda a añadir audiencias personalizadas de Facebook como servicio de LaunchPoint. Envíe listas de Marketo a Facebook para usarlas como audiencias personalizadas en campañas publicitarias.
title: Agregar  [!DNL Facebook] audiencias personalizadas como [!DNL LaunchPoint] servicio
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
TQID: https://experienceleague.adobe.com/oqtZ6Dbnnj8FgpPOLwZbLrmTmmex5spooX0VuJeugT0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 0%

---

# Agregar [!DNL Facebook] audiencias personalizadas como servicio de [!DNL LaunchPoint] {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Con esta integración, puede enviar datos de audiencia desde listas estáticas e inteligentes de Marketo a [!DNL Facebook] para que se utilicen como audiencias personalizadas en [!DNL Facebook] campañas de publicidad. Siga estos pasos para configurarlo.

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
   >Usted *debe* usar una cuenta de [!DNL Facebook] Business Manager para que funcione su integración de audiencias personalizadas. Para aprender a configurar una cuenta de Business Manager, consulte [[!DNL Facebook] Ayuda](https://www.facebook.com/business/help/1710077379203657).

1. Si se le solicita, haga clic en **[!UICONTROL Aceptar]** para aceptar la instalación de la aplicación Marketo en [!DNL Facebook].

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. ¡Ya está autorizado! Seleccione un modo que coincida y haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >**[!UICONTROL Coincidencia básica]** solo usa direcciones de correo electrónico. **[!UICONTROL Coincidencia avanzada]** usa siete campos adicionales, lo que aumenta la tasa de coincidencia, para obtener más conversión. Sin embargo, si la directiva de privacidad de la compañía no permite compartir campos adicionales o si los datos no los incluyen, seleccione [!UICONTROL Coincidencia básica].

   ![](assets/fb-custom-adv-matching-hands.png)

   Ahora puede ir a cualquier lista estática o inteligente en Marketo y enviar datos de audiencia a [!DNL Facebook].

   >[!CAUTION]
   >
   >Antes de usar la integración, [Acepte los términos de audiencias personalizadas de  [!DNL Facebook]](https://www.facebook.com/ads/manage/customaudiences/tos.php) en su cuenta de [!DNL Facebook]. Sin hacerlo, las actualizaciones de audiencia fallarán.

>[!MORELIKETHIS]
>
>* [Crear una audiencia personalizada en [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurar [!DNL Facebook] Anuncios Posibles Clientes](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
