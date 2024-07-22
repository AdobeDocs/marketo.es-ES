---
unique-page-id: 2359909
description: 'Administración de funciones y permisos de usuario: documentos de Marketo, documentación del producto'
title: Administración de roles y permisos de usuario
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Administración de roles y permisos de usuario {#managing-user-roles-and-permissions}

Establezca, cree y edite funciones de usuario y asígnelas a usuarios. Esto le permite controlar las áreas y la funcionalidad a las que cada usuario de Marketo tiene acceso.

Por ejemplo: un usuario de marketing suele necesitar un acceso amplio en toda la aplicación para crear, modificar e implementar correos electrónicos, páginas de aterrizaje y programas. Un diseñador web, por otro lado, pasa casi todo su tiempo en el Design Studio, creando recursos para usarlos en correos electrónicos y páginas de aterrizaje. Y aunque los líderes de la compañía hacen un uso extensivo de los informes de Marketo en el área de Analytics, es posible que no necesiten crear ni dirigir los recursos o programas ellos mismos.

>[!NOTE]
>
>**Se requieren permisos de administración**

Marketo proporciona varias funciones integradas, con diferentes niveles de acceso:

* **Administrador**: todas las partes de la aplicación, incluida la sección Administración
* **Usuario estándar**: todas las partes de la aplicación, excepto la sección Administración
* **Usuario de marketing**: todas las partes de la aplicación, excepto la sección Administración
* **Web Designer**: solo Design Studio
* **Usuario de Analytics**: solo la sección Analytics

No puede editar las funciones Administrador y Usuario estándar, pero puede editar las demás. También puede crear nuevas funciones personalizadas para que coincidan con las estructuras organizativas particulares de su compañía.

## Marketo con identidad de Adobe {#marketo-with-adobe-identity}

Si usa Marketo con identidad de Adobe, la lista de descripciones de perfiles [se puede encontrar aquí](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Asignar funciones a un usuario {#assign-roles-to-a-user}

Puede asignar funciones a un usuario cuando [cree usuarios por primera vez](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) o cuando [edite un usuario existente](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. En la lista, seleccione el usuario que desee editar y haga clic en **[!UICONTROL Editar usuario]**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. En **[!UICONTROL Roles]**, seleccione los roles que desee asignar al usuario según los permisos que necesite y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Para obtener más información sobre cada rol, consulte [Descripciones de los permisos de roles](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md).

## Crear una función nueva {#create-a-new-role}

A veces, su organización tiene empleados con funciones muy específicas que requieren una combinación personalizada de permisos.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Haga clic en la ficha **[!UICONTROL Roles]**.

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Haga clic en **[!UICONTROL Nuevo rol]**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Escriba un **[!UICONTROL Nombre de función]**, una **[!UICONTROL Descripción]** (opcional) y seleccione los permisos que los usuarios de esta función necesitarán.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Editar un rol {#edit-a-role}

Si necesita cambiar los permisos asociados a una función existente, puede editar la función.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Haga clic en la ficha **[!UICONTROL Roles]**.

   ![](assets/managing-user-roles-and-permissions-12.png)

1. En la lista, seleccione la función que desee modificar y haga clic en **[!UICONTROL Editar función]**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Cambie **[!UICONTROL Role Name]** y **[!UICONTROL Description]** si es necesario y, a continuación, cambie la selección de **[!UICONTROL Permisos]** asociados.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Los usuarios que tengan la función que ha editado recibirán los permisos modificados después de cerrar la sesión y volver a iniciarla.

## Eliminar un rol {#delete-a-role}

Si una función se vuelve innecesaria, puede eliminarla.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Haga clic en la ficha **[!UICONTROL Roles]**.

   ![](assets/managing-user-roles-and-permissions-17.png)

1. En la lista, seleccione la función que desee eliminar y haga clic en **[!UICONTROL Eliminar función]**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Haga clic en **[!UICONTROL Eliminar]** para confirmar.

   ![](assets/managing-user-roles-and-permissions-19.png)
