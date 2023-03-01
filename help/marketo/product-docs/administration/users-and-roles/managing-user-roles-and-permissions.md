---
unique-page-id: 2359909
description: 'Administración de funciones y permisos de usuario: documentos de Marketo, documentación del producto'
title: Administración de roles y permisos de usuario
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: 4fa7e733a824af8d2fc0e3ba824b25f9bb985ccf
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Administración de roles y permisos de usuario {#managing-user-roles-and-permissions}

Establezca, cree y edite funciones de usuario y asígnelas a usuarios. Esto le permite controlar las áreas y la funcionalidad a las que cada usuario de Marketo tiene acceso.

Por ejemplo: un usuario de marketing suele necesitar un acceso amplio en toda la aplicación para crear, modificar e implementar correos electrónicos, páginas de aterrizaje y programas. Un diseñador web, por otro lado, pasa casi todo su tiempo en el Design Studio, creando recursos para usarlos en correos electrónicos y páginas de aterrizaje. Y aunque los líderes de la compañía hacen un uso extensivo de los informes de Marketo en el área de Analytics, es posible que no necesiten crear ni dirigir los recursos o programas ellos mismos.

>[!NOTE]
>
>**Permisos de administración necesarios**

Marketo proporciona varias funciones integradas, con diferentes niveles de acceso:

* **Administrador** - todas las partes de la aplicación, incluida la sección Admin
* **Usuario estándar** - todas las partes de la aplicación, excepto la sección Admin
* **Usuario de marketing** - todas las partes de la aplicación, excepto la sección Admin
* **Diseñador web** - sólo el Design Studio
* **Usuario de Analytics** - solo la sección Analytics

No puede editar las funciones Administrador y Usuario estándar, pero puede editar las demás. También puede crear nuevas funciones personalizadas para que coincidan con las estructuras organizativas particulares de su compañía.

## Marketo con identidad de Adobe {#marketo-with-adobe-identity}

Si utiliza Marketo con identidad de Adobe, consulte la lista de descripciones de perfiles [se puede encontrar aquí](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Asignar funciones a un usuario {#assign-roles-to-a-user}

Puede asignar funciones a un usuario cuando [creación de usuarios por primera vez](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) o por [edición de un usuario existente](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Vaya a la **Administrador** área.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Clic **Usuarios y funciones**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. En la lista, seleccione el usuario que desea editar y haga clic en **Editar usuario**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. En **Funciones**, seleccione las funciones que desee asignar al usuario según los permisos que necesite y haga clic en **Guardar**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Para obtener más información sobre cada función, consulte [Descripciones de los permisos de funciones](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md).

## Crear una función nueva {#create-a-new-role}

A veces, su organización tiene empleados con funciones muy específicas que requieren una combinación personalizada de permisos.

1. Vaya a la **Administrador** área.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Clic **Usuarios y funciones**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Haga clic en **Funciones** pestaña.

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Clic **Nuevo rol**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Introduzca una **Nombre de rol**, a **Descripción** (opcional) y seleccione los permisos que necesitarán los usuarios de esta función.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Editar un rol {#edit-a-role}

Si necesita cambiar los permisos asociados a una función existente, puede editar la función.

1. Vaya a la **Administrador** área.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Clic **Usuarios y funciones**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Haga clic en **Funciones** pestaña.

   ![](assets/managing-user-roles-and-permissions-12.png)

1. En la lista, seleccione el rol que desea modificar y haga clic en **Editar rol**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Cambie el **Nombre de rol** y **Descripción** si es necesario, y cambie la selección de asociado **Permisos**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Los usuarios que tengan la función que ha editado recibirán los permisos modificados después de cerrar la sesión y volver a iniciarla.

## Eliminar un rol {#delete-a-role}

Si una función se vuelve innecesaria, puede eliminarla.

1. Vaya a la **Administrador** área.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Clic **Usuarios y funciones**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Haga clic en **Funciones** pestaña.

   ![](assets/managing-user-roles-and-permissions-17.png)

1. En la lista, seleccione la función que desee eliminar y haga clic en **Eliminar función**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Clic **Eliminar** para confirmar.

   ![](assets/managing-user-roles-and-permissions-19.png)
