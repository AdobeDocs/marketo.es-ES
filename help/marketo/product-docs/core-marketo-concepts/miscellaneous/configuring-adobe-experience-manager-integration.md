---
unique-page-id: 30081815
description: Configuración de la integración de Adobe Experience Manager - Documentos de Marketo - Documentación del producto
title: Configuración de la integración con Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configuración de la integración con Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure Adobe Experience Manager AEM AEM () para poder acceder a los recursos, seleccionarlos e importarlos en el estudio de diseño de Marketo Engage.

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!IMPORTANT]
>
>* AEM Esta integración solo funciona con implementaciones locales de y no es compatible con implementaciones de AEM Cloud Service.
>
>* Actualmente, esta función solo es totalmente compatible con Firefox. Safari no lo admite y es posible que no funcione en la versión más reciente de Chrome, según la configuración de la cookie de SameSite.

1. Vaya a Adobe Experience Manager (la dirección URL es específica de su empresa).

   ![](assets/one.png)

1. Puede iniciar sesión con el Adobe o localmente. En este ejemplo, iniciaremos sesión localmente.

   ![](assets/two.png)

1. Entrada **Herramientas**, haga clic en **Operaciones** y seleccione **Consola web**.

   ![](assets/2a.png)

1. En su navegador, busque (ctrl+f en Windows, cmd+f en Mac) &quot;Política de uso compartido de recursos de origen cruzado de Adobe Granite&quot;.

   ![](assets/three.png)

1. Haga clic en **+** Firme a la derecha.

   ![](assets/four.png)

1. En el **Orígenes permitidos (Regexp)** cuadro de texto, escriba `https://.*\.marketo\.com` y haga clic en **Guardar**.

   ![](assets/five-psd.png)

1. En el encabezado situado en la parte superior de la página, haga clic en **Consola web** y seleccione **Información del sistema**.

   ![](assets/six.png)

1. En Información del servidor, haga clic en **Restart** botón.

   ![](assets/seven.png)

1. Clic **OK** para confirmar.

   ![](assets/eight.png)

1. En Marketo Engage, haga clic en **Administrador**.

   ![](assets/nine.png)

1. En Integración, seleccione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Clic **Editar**.

   ![](assets/eleven.png)

1. AEM Introduzca la dirección URL de la y haga clic en **OK**.

   ![](assets/twelve.png)
