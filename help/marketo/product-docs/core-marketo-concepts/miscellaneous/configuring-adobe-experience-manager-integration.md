---
unique-page-id: 30081815
description: Configuración de la integración de Adobe Experience Manager - Marketo Docs - Documentación del producto
title: Configuración de la integración de Adobe Experience Manager
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Configuración de la integración de Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure AEM para que pueda acceder, seleccionar e importar AEM recursos en Design Studio de Marketo.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!CAUTION]
>
>Actualmente, esta función solo es totalmente compatible con Firefox. No es compatible con Safari y es posible que no funcione en la última versión de Chrome (v. 80), según la configuración de las cookies de SameSite.

1. Vaya a Adobe Experience Manager (la dirección URL es específica de su empresa).

   ![](assets/one.png)

1. Puede iniciar sesión con Adobe o con inicio de sesión local. En este ejemplo iniciaremos sesión localmente.

   ![](assets/two.png)

1. En **Tools**, haga clic en **Operations** y seleccione **Web Console**.

   ![](assets/2a.png)

1. En el navegador, busque &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot; (ctrl+f en Windows, cmd+f en Mac).

   ![](assets/three.png)

1. Haga clic en el signo **+** de la derecha.

   ![](assets/four.png)

1. En el cuadro de texto **Orígenes permitidos (Regexp)**, escriba `https://.*\.marketo\.com` y haga clic en **Guardar**.

   ![](assets/five-psd.png)

1. En el encabezado de la parte superior de la página, haga clic en **Consola Web** y seleccione **Información del sistema**.

   ![](assets/six.png)

1. En Información del servidor, haga clic en el botón **Restart**.

   ![](assets/seven.png)

1. Haga clic en **OK** para confirmar.

   ![](assets/eight.png)

1. En Marketo Classic, haga clic en **Admin**.

   ![](assets/nine.png)

1. En Integración, seleccione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Haga clic en **Editar**.

   ![](assets/eleven.png)

1. Introduzca la dirección URL de AEM y haga clic en **OK**.

   ![](assets/twelve.png)

   ¡Estás listo! Ahora puede [importar AEM recursos en Design Studio en Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
