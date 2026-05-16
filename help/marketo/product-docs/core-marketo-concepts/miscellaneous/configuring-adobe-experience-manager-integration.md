---
unique-page-id: 30081815
description: Obtenga información sobre cómo configurar la integración de Adobe Experience Manager con Marketo. Configure AEM para poder acceder a los recursos e importarlos en Design Studio.
title: Configuración de la integración de Adobe Experience Manager
hide: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
TQID: https://experienceleague.adobe.com/nJBydVi8mRwVf1vAIFuI1S3nEuX0FGiztp8fhRHq6RM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 8%

---

# Configuración de la integración de Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure Adobe Experience Manager (AEM) para poder acceder, seleccionar e importar recursos de AEM en Marketo Engage Design Studio.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!IMPORTANT]
>
>* Esta integración solo funciona con implementaciones locales de AEM y no es compatible con implementaciones de AEM Cloud Service.
>
>* Actualmente, esta función solo es totalmente compatible con Firefox. Safari no lo admite y es posible que no funcione en la versión más reciente de Chrome, según la configuración de la cookie de SameSite.

1. Vaya a Adobe Experience Manager (la dirección URL es específica de su empresa).

   ![](assets/one.png)

1. Puede iniciar sesión con Adobe o localmente. Este ejemplo utiliza el inicio de sesión local.

   ![](assets/two.png)

1. En **[!UICONTROL Herramientas]**, haga clic en **[!UICONTROL Operaciones]** y seleccione **[!UICONTROL Consola web]**.

   ![](assets/2a.png)

1. En su explorador, busque (ctrl+f en Windows, cmd+f en Mac) &quot;[!UICONTROL Política de uso compartido de recursos de origen cruzado de Adobe Granite]&quot;.

   ![](assets/three.png)

1. Haga clic en el signo **+** de la derecha.

   ![](assets/four.png)

1. En el cuadro de texto **[!UICONTROL Orígenes permitidos (Regexp)]**, escriba `https://.*\.marketo\.com` y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/five-psd.png)

1. En el encabezado de la parte superior de la página, haz clic en **[!UICONTROL Consola web]** y selecciona **[!UICONTROL Información del sistema]**.

   ![](assets/six.png)

1. En Información del servidor, haga clic en el botón **[!UICONTROL Reiniciar]**.

   ![](assets/seven.png)

1. Haga clic en **[!UICONTROL Aceptar]** para confirmar.

   ![](assets/eight.png)

1. En Marketo Engage, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/nine.png)

1. En Integración, seleccione **[!UICONTROL Adobe Experience Manager]**.

   ![](assets/ten.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/eleven.png)

1. Escriba la dirección URL de AEM y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/twelve.png)
