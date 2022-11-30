---
unique-page-id: 11382122
description: Habilitar pista de auditoría - Documentos de Marketo - Documentación del producto
title: Habilitar pista de auditoría
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
source-git-commit: 73d41904ca74ae265648c3ed91805be7c4d24fe0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Habilitar pista de auditoría {#enable-audit-trail}

La pista de auditoría está disponible para todos los clientes y está controlada por dos permisos de administrador.

>[!NOTE]
>
>De forma predeterminada, todos los roles de administrador del sistema tienen ambos permisos habilitados.

## Habilitar pista de auditoría para una función {#enable-audit-trail-for-a-role}

1. Haga clic en **Administrador**.

   ![](assets/enable-audit-trail-1.png)

1. Select **Usuarios y funciones** y haga clic en **Funciones**.

   ![](assets/enable-audit-trail-2.png)

1. Seleccione la función para la que desea habilitar la pista de auditoría y haga clic en **Editar función**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >También tiene la opción aquí para crear una nueva función y otorgarle acceso a Pista de auditoría.

1. Expanda el **Administrador de acceso** permiso. Select **Acceso a pista de auditoría** y/o **Acceso al historial de inicio de sesión**, según sus necesidades. Haga clic en **Guardar**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >**Acceso a pista de auditoría:** Permite a los usuarios acceder tanto a la pista de auditoría de recursos como a la pista de auditoría de administración.
   >
   >**Acceso al historial de inicio de sesión:** Concede a los usuarios acceso a [Historial de inicio de sesión del usuario](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Asignar función de pista de auditoría a un usuario {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Crear](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) o [enable](#enable-audit-trail) una función existente que le otorga permisos de pista de auditoría.

1. En **Usuarios y funciones**, haga clic en **Usuarios**.

   ![](assets/enable-audit-trail-5.png)

1. Seleccione el usuario al que desea conceder acceso a la pista de auditoría y haga clic en **Editar usuario**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Este proceso también se aplica cuando se crea un nuevo usuario.

1. Seleccione las funciones de pista de auditoría que ha creado. En este ejemplo creamos &quot;Pista de auditoría - Activo y administrador&quot; y &quot;Pista de auditoría - Con historial de inicio de sesión&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Si tiene espacios de trabajo habilitados, asegúrese de marcar la casilla de verificación de la función, que selecciona todos los espacios de trabajo. Al anular la selección de un espacio de trabajo individual, se ocultará la pista de auditoría. Esto significa que verá los datos de pista de auditoría de cada espacio de trabajo. Tiene la opción de ocultar espacios de trabajo cuando [filtrado](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Haga clic en **Guardar**.

   ![](assets/enable-audit-trail-8.png)
