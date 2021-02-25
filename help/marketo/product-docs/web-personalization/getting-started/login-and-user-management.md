---
unique-page-id: 7513771
description: Inicio de sesión y administración de usuarios - Documentos de marketing - Documentación del producto
title: Inicio de sesión y administración de usuarios
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Inicio de sesión y administración de usuarios {#login-and-user-management}

## Crear una función de usuario de personalización web {#create-a-web-personalization-user-role}

1. Vaya a la sección **Administración** y haga clic en **Usuarios y roles**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Haga clic en **Roles**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Si la función de usuario de Personalización web (WP) ya existe, asegúrese de que está configurada como se muestra en el paso 4.

1. Haga clic en **Nueva función**.

   ![](assets/three-1.png)

1. Introduzca un nombre de rol y seleccione Permisos. Haga clic en **Crear** (esta función debe [aplicarse a todos los espacios de trabajo](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Para otorgar a los usuarios permiso para acceder a todo lo que se encuentra en Segmentación y personalización, asegúrese de seleccionar _todo_ las casillas de verificación.

## Permisos de usuario de contenido predictivo y personalización de Web {#web-personalization-and-predictive-content-user-permissions}

**Segmentación y personalización**: El usuario solo tiene permisos de vista si este permiso solo está seleccionado.

**Administración Personalización Web + Predictiva**: El usuario solo tiene acceso a la configuración de cuenta y a la configuración de contenido de la aplicación de personalización web y contenido predictivo. Los usuarios pueden realizar vistas de páginas en la aplicación, pero no tienen permisos de creación, edición, eliminación ni inicio.

**Editor** de contenido predictivo: El usuario tiene acceso de editor a la aplicación de contenido predictivo. El permiso permite crear, editar y eliminar fragmentos de contenido. No permite habilitar el contenido para el uso predictivo en la Web o en el correo electrónico.

**Iniciador** de contenido predictivo: El usuario tiene acceso a todas las funciones de contenido predictivo, excepto a la configuración de contenido y cuenta. El permiso permite crear, editar, eliminar y activar fragmentos de contenido.

**Editor** de Campañas web: El usuario tiene acceso de editor a todas las funciones de personalización web para crear, editar y eliminar, pero no iniciar campañas web.

**Iniciador** de Campaña web: El usuario tiene acceso a todas las funciones de la aplicación de personalización web, excepto a la configuración de la cuenta y el contenido. El permiso permite crear, editar, eliminar e iniciar campañas web.

## Asignar la función de WP al usuario {#assign-wp-role-to-user}

1. Vaya a **Usuarios**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Seleccione el usuario al que desea otorgar acceso WP y haga clic en **Editar usuario**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Seleccione la función de usuario de WP para todos los espacios de trabajo.

   ![](assets/seven.png)

1. Los usuarios recién habilitados verán el mosaico **Personalización web** en Mi marketing la próxima vez que inicien sesión.

   ![](assets/eight.png)
