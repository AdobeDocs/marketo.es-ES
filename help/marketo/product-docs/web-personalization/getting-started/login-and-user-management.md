---
unique-page-id: 7513771
description: Inicio de sesión y administración de usuarios - Documentos de Marketo - Documentación del producto
title: Inicio de sesión y administración de usuarios
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 2%

---

# Inicio de sesión y administración de usuarios {#login-and-user-management}

## Crear un rol de usuario de [!UICONTROL Web Personalization] {#create-a-web-personalization-user-role}

1. Vaya a la sección **[!UICONTROL Administrador]** y, a continuación, haga clic en **[!UICONTROL Usuarios y roles]**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Haga clic en **[!UICONTROL Roles]**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Si la función de usuario Web Personalization (WP) ya existe, asegúrese de que está configurada como se muestra en el paso 4.

1. Haga clic en **[!UICONTROL Nuevo rol]**.

   ![](assets/three-1.png)

1. Escriba un [!UICONTROL Nombre de rol] y seleccione [!UICONTROL Permisos]. Haga clic en **[!UICONTROL Crear]** (esta función debe [aplicarse a todos los espacios de trabajo](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Para dar permiso a los usuarios para acceder a todo en Targeting y Personalization, asegúrese de seleccionar _todas_ las casillas de verificación.

## Permisos de usuario de [!UICONTROL Web Personalization] y contenido predictivo {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Segmentación y Personalization]**: el usuario tiene permisos de solo vista, si este permiso solo está seleccionado.

**[!UICONTROL Admin Web Personalization + Predictive]**: el usuario solo tiene acceso a la configuración de la cuenta y a la configuración de contenido para la aplicación Web Personalization y de contenido predictivo. Los usuarios pueden ver las páginas en la aplicación, pero no tienen permisos para crear, editar, eliminar ni iniciar.

**[!UICONTROL Editor de contenido predictivo]**: el usuario tiene acceso de editor a la aplicación de contenido predictivo. El permiso permite crear, editar o eliminar fragmentos de contenido. No permite habilitar contenido para uso predictivo en la web o por correo electrónico.

**[!UICONTROL Iniciador de contenido predictivo]**: el usuario tiene acceso a todas las características de contenido predictivo, excepto a la configuración de la cuenta y el contenido. El permiso permite crear, editar y eliminar y habilitar fragmentos de contenido.

**[!UICONTROL Editor de campañas web]**: el usuario tiene acceso de editor a todas las características de Web Personalization para crear, editar y eliminar, pero no para iniciar campañas web.

**[!UICONTROL Lanzador de campañas web]**: el usuario tiene acceso a todas las características de la aplicación Web Personalization, excepto a la configuración de la cuenta y del contenido. El permiso permite crear, editar, eliminar e iniciar campañas web.

## Asignar rol WP al usuario {#assign-wp-role-to-user}

1. Ir a **[!UICONTROL Usuarios]**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Seleccione el usuario al que desea conceder acceso al WP y haga clic en **[!UICONTROL Editar usuario]**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Seleccione la función de usuario WP para todos los espacios de trabajo.

   ![](assets/seven.png)

1. Los usuarios recién habilitados verán el mosaico **[!UICONTROL Web Personalization]** en Mi Marketo la próxima vez que inicien sesión.

   ![](assets/eight.png)
