---
unique-page-id: 30081815
description: Configuración de la integración de Adobe Experience Manager - Documentos de marketing - Documentación del producto
title: Configuración de la integración de Adobe Experience Manager
translation-type: tm+mt
source-git-commit: e5050328cbddaf072dd60ddd8d7363a704e720b5
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Configuración de la integración de Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure AEM para que pueda acceder, seleccionar e importar AEM recursos en el estudio de diseño de Marketing Cloud.

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!CAUTION]
>
>Actualmente, esta función solo es totalmente compatible con Firefox. No es compatible con Safari y es posible que no funcione en la versión más reciente de Chrome (v. 80), según la configuración de la cookie SameSite.

1. Vaya al Adobe Experience Manager (la dirección URL es específica de su compañía).

   ![](assets/one.png)

1. Puede iniciar sesión con Adobe o localmente. En este ejemplo iniciaremos sesión localmente.

   ![](assets/two.png)

1. En **Herramientas**, haga clic en **Operaciones** y seleccione **Consola Web**.

   ![](assets/2a.png)

1. En el navegador, busque &quot;Política de uso compartido de recursos de Adobe Granite Cross-Origen&quot; (ctrl+f en Windows, cmd+f en Mac).

   ![](assets/three.png)

1. Haga clic en el signo **+** de la derecha.

   ![](assets/four.png)

1. En el cuadro de texto **Orígenes permitidos (Regexp)**, escriba `https://.*\.marketo\.com` y haga clic en **Guardar**.

   ![](assets/five-psd.png)

1. En el encabezado de la parte superior de la página, haga clic en **Consola web** y seleccione **Información del sistema**.

   ![](assets/six.png)

1. En Información del servidor, haga clic en el botón **Reiniciar**.

   ![](assets/seven.png)

1. Haga clic en **Aceptar** para confirmar.

   ![](assets/eight.png)

1. En Marketing Classic, haga clic en **Administración**.

   ![](assets/nine.png)

1. En Integración, seleccione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Haga clic en **Editar**.

   ![](assets/eleven.png)

1. Introduzca la dirección URL de AEM y haga clic en **Aceptar**.

   ![](assets/twelve.png)

   ¡Estás listo! Ahora puede [importar recursos de AEM en Design Studio en Marketo Sky](https://help.marketo.com/hc/en-us/articles/360036765993).
