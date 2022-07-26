---
unique-page-id: 30081815
description: 'Configuración de la integración de Adobe Experience Manager: Marketo Docs: documentación del producto'
title: Configuración de la integración de Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 3105fb33fb457d4dfb63081b80d4d1def717ad34
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Configuración de la integración de Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure AEM para que pueda acceder, seleccionar e importar AEM recursos en Marketo Design Studio.

>[!NOTE]
>
>**Se requieren permisos de administrador**

>[!IMPORTANT]
>
>* Esta integración solo funciona con implementaciones locales de AEM y no es compatible con implementaciones de AEM Cloud Service.
>
>* Actualmente, esta función solo es totalmente compatible con Firefox. No es compatible con Safari y es posible que no funcione en la última versión de Chrome, en función de la configuración de cookies de SameSite.


1. Vaya a Adobe Experience Manager (la dirección URL es específica de su empresa).

   ![](assets/one.png)

1. Puede iniciar sesión con Adobe o con inicio de sesión local. En este ejemplo iniciaremos sesión localmente.

   ![](assets/two.png)

1. En **Herramientas**, haga clic en **Operaciones** y seleccione **Consola web**.

   ![](assets/2a.png)

1. En el navegador, busque &quot;Política de uso compartido de recursos de origen cruzado de Adobe Granite&quot; (ctrl+f en Windows, cmd+f en Mac).

   ![](assets/three.png)

1. Haga clic en el **+** a la derecha.

   ![](assets/four.png)

1. En el **Orígenes permitidos (Regexp)** cuadro de texto, escriba `https://.*\.marketo\.com` y haga clic en **Guardar**.

   ![](assets/five-psd.png)

1. En el encabezado de la parte superior de la página, haga clic en **Consola web** y seleccione **Información del sistema**.

   ![](assets/six.png)

1. En Información del servidor, haga clic en la **Restart** botón.

   ![](assets/seven.png)

1. Haga clic en **OK** para confirmar.

   ![](assets/eight.png)

1. En Marketo Classic, haga clic en **Administrador**.

   ![](assets/nine.png)

1. En Integración, seleccione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Haga clic en **Editar**.

   ![](assets/eleven.png)

1. Introduzca la dirección URL de AEM y haga clic en **OK**.

   ![](assets/twelve.png)

   ¡Estás listo! Ahora puede [importar AEM recursos en Design Studio en Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
