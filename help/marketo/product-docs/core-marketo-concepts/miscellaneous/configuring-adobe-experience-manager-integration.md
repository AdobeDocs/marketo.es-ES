---
unique-page-id: 30081815
description: Configuración de la integración de Adobe Experience Manager - Documentos de Marketo - Documentación del producto
title: Configuración de la integración con Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configuración de la integración con Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure Adobe Experience Manager AEM AEM () para poder acceder a los recursos, seleccionarlos e importarlos en el estudio de diseño de Marketo Engage.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!IMPORTANT]
>
>* AEM Esta integración solo funciona con implementaciones locales de y no es compatible con implementaciones de AEM Cloud Service.
>
>* Actualmente, esta función solo es totalmente compatible con Firefox. Safari no lo admite y es posible que no funcione en la versión más reciente de Chrome, según la configuración de la cookie de SameSite.

1. Vaya a Adobe Experience Manager (la dirección URL es específica de su empresa).

   ![](assets/one.png)

1. Puede iniciar sesión con el Adobe o localmente. En este ejemplo, iniciaremos sesión localmente.

   ![](assets/two.png)

1. En **[!UICONTROL Herramientas]**, haga clic en **[!UICONTROL Operaciones]** y seleccione **[!UICONTROL Consola web]**.

   ![](assets/2a.png)

1. En su navegador, busque (ctrl+f en Windows, cmd+f en Mac) &quot;Política de uso compartido de recursos de origen cruzado de Adobe Granite&quot;.

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

1. AEM Escriba la dirección URL de la y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/twelve.png)
