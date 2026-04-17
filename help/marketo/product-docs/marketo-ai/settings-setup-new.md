---
description: Obtenga información sobre cómo habilitar permisos de IA de Marketo, configurar reglas organizativas y administrar configuraciones como integraciones y notificaciones.
title: Configuración y configuración
hide: true
hidefromtoc: true
source-git-commit: 47389ec9d7974d5f75a68bfbb0e32e8147d8eaaa
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 4%

---

# Configuración y configuración {#settings-setup}

Obtenga información sobre cómo habilitar permisos y utilizar el área Configuración para ver los detalles de conexión, definir reglas organizativas y configurar integraciones y notificaciones.

## Permisos y funciones {#permission-and-role}

Hay una compilación de _Access con permiso de AI_ y una compilación con rol de _AI_, lo que proporciona a los administradores un mayor control sobre los usuarios que pueden acceder a la característica **Build with AI**. El permiso se asigna en el nivel de rol. La función _Build with AI_ viene con el permiso _Access Build with AI_ habilitado de forma predeterminada.

>[!IMPORTANT]
>
>El permiso _Generar acceso con IA_ no está habilitado de manera predeterminada para todas las funciones. Consulte la tabla siguiente para obtener más información.

<table><thead>
  <tr>
    <th>Función</th>
    <th>Estado predeterminado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Administrador</td>
    <td>Habilitado</td>
  </tr>
  <tr>
    <td>Administrador de productos de Adobe</td>
    <td>Habilitado</td>
  </tr>
  <tr>
    <td>Usuario de marketing</td>
    <td>Desactivado</td>
  </tr>
  <tr>
    <td>Usuario estándar</td>
    <td>No disponible</td>
  </tr>
  <tr>
    <td>Generar con usuario de IA</td>
    <td>Habilitado</td>
  </tr>
  <tr>
    <td>Funciones personalizadas</td>
    <td>Desactivado</td>
  </tr>
</tbody>
</table>

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
