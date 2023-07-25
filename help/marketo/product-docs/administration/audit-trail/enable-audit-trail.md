---
unique-page-id: 11382122
description: Habilitar pista de auditoría - Documentos de Marketo - Documentación del producto
title: Habilitar pista de auditoría
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Habilitar pista de auditoría {#enable-audit-trail}

La pista de auditoría está disponible para todos los clientes y controlada por dos permisos de administrador.

>[!NOTE]
>
>De forma predeterminada, todas las funciones de administrador del sistema tienen ambos permisos habilitados.

## Habilitar pista de auditoría para un rol {#enable-audit-trail-for-a-role}

1. Clic **[!UICONTROL Administrador]**.

   ![](assets/enable-audit-trail-1.png)

1. Seleccionar **[!UICONTROL Usuarios y funciones]** y haga clic en **[!UICONTROL Funciones]**.

   ![](assets/enable-audit-trail-2.png)

1. Seleccione la función para la que desea habilitar la pista de auditoría y haga clic en **[!UICONTROL Editar rol]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >También tiene la opción de crear una función nueva y otorgarle acceso a Pista de auditoría.

1. Expanda el **[!UICONTROL Acceso a administrador]** permiso. Seleccionar **[!UICONTROL Registro de auditoría de acceso]** y/o **[!UICONTROL Acceder al historial de inicio]**, según sus necesidades. Clic **[!UICONTROL Guardar]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >**[!UICONTROL Registro de auditoría de acceso]**: otorga a los usuarios acceso a ambos [!UICONTROL Pista de auditoría de activos] y [!UICONTROL Registro de auditoría de administración].
   >
   >**[!UICONTROL Acceder al historial de inicio]**: otorga a los usuarios acceso a [Historial de inicio de sesión del usuario](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Asignar la función de pista de auditoría a un usuario {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Crear](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) o [habilitar](#enable-audit-trail) una función existente, otorgándole permisos de pista de auditoría.

1. Entrada **[!UICONTROL Usuarios y funciones]**, haga clic en **[!UICONTROL Usuarios]**.

   ![](assets/enable-audit-trail-5.png)

1. Seleccione el usuario al que desea otorgar acceso a la pista de auditoría y haga clic en **[!UICONTROL Editar usuario]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Este proceso también se aplica cuando crea un nuevo usuario.

1. Seleccione las funciones de pista de auditoría que ha creado. En este ejemplo creamos &quot;Pista de auditoría: recurso y administración&quot; y &quot;Pista de auditoría: con historial de inicio de sesión&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Si tiene espacios de trabajo activados, asegúrese de marcar la casilla de verificación de la función, que selecciona todos los espacios de trabajo. Al anular la selección de un espacio de trabajo individual, se oculta la pista de auditoría. Esto significa que verá datos de pista de auditoría para cada espacio de trabajo. Tiene la opción de ocultar los espacios de trabajo al [filtrado](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Clic **[!UICONTROL Guardar]**.

   ![](assets/enable-audit-trail-8.png)
