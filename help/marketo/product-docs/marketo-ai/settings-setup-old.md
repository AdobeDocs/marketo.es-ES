---
description: Obtenga información sobre cómo habilitar permisos de IA de Marketo, configurar reglas organizativas y administrar configuraciones como integraciones y notificaciones.
title: Configuración y configuración
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: c0854d574b4fc995f249783aebcd15ed7d224851
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Configuración y configuración {#settings-setup}

Obtenga información sobre cómo habilitar permisos y utilizar el área Configuración para ver los detalles de conexión, definir reglas organizativas y configurar integraciones y notificaciones.

## Permisos {#permissions}

>[!IMPORTANT]
>
>En la fase de Alpha de Marketo AI, el acceso de _está habilitado de forma predeterminada_ para los siguientes roles: Administrador, Administrador de productos de Adobe, Usuario de marketing y Usuario estándar. Por lo tanto, en lugar de activarlo para las funciones a las que desea tener acceso, debe desactivarlo para las funciones a las que no tenga acceso.

### Acceso para todos {#access-for-all}

Si desea habilitar la IA de Marketo para todas las funciones enumeradas anteriormente, no tiene que hacer nada.

### Acceso para algunos {#access-for-some}

Si desea quitar el acceso a cualquier función, siga los pasos a continuación.

1. En Mi Marketo, haz clic en **Administrador**, luego en **Usuarios y roles**.

   ![](assets/settings-setup-1.png)

1. En la ficha _Roles_, seleccione el rol que desee y haga clic en **Editar rol**.

   ![](assets/settings-setup-2.png)

1. Desplácese hacia abajo y _desmarque_ la casilla de verificación **Generar acceso con IA** y haga clic en **Guardar**.

   ![](assets/settings-setup-3.png)

Repita estos pasos para cualquier otra función que desee.

### Función personalizada {#custom-role}

También tiene la opción de [crear una nueva función](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} y personalizar sus permisos, agregando _Generar acceso con IA_, junto con cualquier otra cosa que desee, y [asignando esa función](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a usuarios específicos.

<!-- 
## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

## Configuración {#settings}

1. En Mi Marketo, haga clic en el mosaico **Generar con IA**.

   ![](assets/settings-setup-4.png)

1. Haga clic en el icono de engranaje.

   ![](assets/settings-setup-5.png)

### Conexión {#connection}

Esta pestaña no contiene campos editables. Muestra información de la cuenta, como su Munchkin ID y su organización IMS.

![](assets/settings-setup-6.png)

### Reglas organizativas {#organizational-rules}

Defina las directrices y restricciones organizativas que sigue la IA de Marketo al crear o modificar recursos de Marketo Engage.

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Las reglas utilizan el formato Markdown con YAML frontmatter. Las reglas globales se aplican a todos los espacios de trabajo. Las reglas de Workspace anulan la configuración global.

### Integraciones (próximamente) {#integrations}

Configure conexiones a servicios externos y API.

_Esta ficha puede aparecer en la interfaz de usuario, pero aún no está disponible para su uso. Vuelva a buscar actualizaciones_.

### Notificaciones (próximamente) {#notifications}

Administrar las preferencias de alerta y los canales de notificación.

_Esta ficha puede aparecer en la interfaz de usuario, pero aún no está disponible para su uso. Vuelva a buscar actualizaciones_.
