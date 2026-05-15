---
description: Obtenga información sobre cómo habilitar permisos de IA de Marketo, configurar reglas organizativas y administrar configuraciones como integraciones y notificaciones.
title: Configuración y configuración
badge: Beta
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---

# Configuración y configuración {#settings-setup}

Obtenga información sobre cómo habilitar permisos y utilizar el área Configuración para ver los detalles de conexión, definir reglas organizativas y configurar integraciones y notificaciones.

>[!PREREQUISITES]
>
>Para usar esta característica, primero debe aceptar los términos de [Core Gen-AI y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!NOTE]
>
>Esta función está en versión beta cerrada y se está implementando por fases en los próximos meses. Sabrás cuándo se ha habilitado para tu suscripción cuando veas un mosaico de _Generar con IA_ en la pantalla de Mi Marketo.

## Permisos y funciones {#permission-and-role}

Hay una compilación de _Access con permiso de AI_ y una función de _Build with AI User_, que proporciona a los administradores un mayor control sobre los usuarios que pueden acceder a la función **Build with AI**. El permiso se asigna en el nivel de rol. La función _Generar con usuario de IA_ viene con el permiso _Generar acceso con IA_ habilitado de forma predeterminada.

>[!IMPORTANT]
>
>El permiso _Generar acceso con IA_ no está habilitado de manera predeterminada para todas las funciones. Consulte la tabla siguiente para obtener más información.

| Función | Estado predeterminado |
| --- | --- |
| Administrador | Habilitado |
| Administrador de productos de Adobe | Habilitado |
| Usuario de marketing | Desactivado |
| Usuario estándar | No disponible |
| Generar con usuario de IA | Habilitado |
| Funciones personalizadas | Desactivado |

### Acceso a la versión con permiso de IA {#access-build-with-ai-permission}

Siga los pasos a continuación para habilitar _Access Build con IA_ para roles calificadores que aún no lo tienen habilitado.

1. En Mi Marketo, haz clic en **Administrador**, luego en **Usuarios y roles**.

   ![](assets/settings-setup-1.png)

1. En la ficha _Roles_, seleccione el rol que desee y haga clic en **Editar rol**.

   ![](assets/settings-setup-2.png)

1. Desplácese hacia abajo y marque la casilla de verificación _Generar acceso con IA_ y haga clic en **Guardar**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Puede seguir estos mismos pasos para quitar el permiso **un** marcando la casilla de verificación _Generar acceso con IA_.

### Generar con función de usuario de IA {#build-with-ai-user-role}

Sigue estos pasos para asignar un usuario específico al rol _Generar con usuario de IA_.

>[!NOTE]
>
>Este rol **solamente** contiene la compilación de acceso _con permiso de IA_.

1. En Mi Marketo, haz clic en **Administrador**, luego en **Usuarios y roles**.

   ![](assets/settings-setup-1.png)

1. Seleccione el usuario que desee y haga clic en **Editar usuario**.

   ![](assets/settings-setup-5b.png)

1. En _Roles y espacios de trabajo_, active la casilla de verificación _Generar con usuario de IA_. Si tiene más de un área de trabajo, puede especificar cuáles recibirán acceso en la lista desplegable de signo **+**. Haga clic en **Guardar** cuando termine.

   ![](assets/settings-setup-6b.png)

### Función personalizada {#custom-role}

También tiene la opción de [crear una nueva función](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} y personalizar sus permisos, agregando _Generar acceso con IA_, junto con cualquier otra cosa que desee, y [asignando esa función](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a usuarios específicos.

## Configuración {#settings}

1. En Mi Marketo, haga clic en el mosaico **Generar con IA**.

   ![](assets/settings-setup-4.png)

1. Haga clic en el icono de engranaje.

   ![](assets/settings-setup-5.png)

### Connection {#connection}

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
