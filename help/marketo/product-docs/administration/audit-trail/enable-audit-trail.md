---
unique-page-id: 11382122
description: Habilitar pista de auditoría - Documentos de marketing - Documentación del producto
title: Habilitar pista de auditoría
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Habilitar pista de auditoría {#enable-audit-trail}

La pista de auditoría está disponible para todos los clientes y está controlada por dos permisos de administración.

>[!NOTE]
>
>De forma predeterminada, todas las funciones de administración del sistema tienen ambos permisos activados.

## Habilitar pista de auditoría para una función {#enable-audit-trail-for-a-role}

1. Haga clic en **Administración**.

   ![](assets/one-2.png)

1. Seleccione **Usuarios y roles** y haga clic en **Roles**.

   ![](assets/two-2.png)

1. Seleccione la función para la que desea habilitar la pista de auditoría y haga clic en **Editar función**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >También tiene la opción de crear una nueva función y otorgarle acceso a la pista de auditoría.

1. Expanda el permiso **Administración de acceso**. Seleccione **Ruta de auditoría de acceso** y/o **Historial de inicio de sesión de acceso**, según sus necesidades. Haga clic en **Guardar**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >
   >**Acceso a pista de auditoría:** proporciona a los usuarios acceso a la pista de auditoría de recursos y a la pista de auditoría de administración.
   >
   >
   >**Acceso al historial de inicio de sesión:** otorga a los usuarios acceso al historial [ de inicio de sesión ](user-login-history.md)del usuario.

## Asignar la función de pista de auditoría a un usuario {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[](http://docs.marketo.com/display/DOCS/Create,+Delete,+Edit+and+Change+a+User+Role#Create,Delete,EditandChangeaUserRole-CreateaRole) Cree o  [](#Enable) habilite una función existente, otorgándole permisos de pista de auditoría.

1. En **Usuarios y roles**, haga clic en **Usuarios**.

   ![](assets/five-1.png)

1. Seleccione el usuario al que desea otorgar acceso a la pista de auditoría y haga clic en **Editar usuario**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Este proceso también se aplica al crear un nuevo usuario.

1. Seleccione las funciones de pista de auditoría que ha creado. En este ejemplo creamos &quot;Pista de auditoría: recurso y administrador&quot; y &quot;Pista de auditoría: con historial de inicio de sesión&quot;.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Si tiene habilitadas las áreas de trabajo, asegúrese de marcar la casilla de verificación de la función, que selecciona todas las áreas de trabajo. Si se anula la selección de un espacio de trabajo individual, se ocultará la pista de auditoría. Esto significa que verá los datos de la pista de auditoría de cada espacio de trabajo. Tiene la opción de ocultar espacios de trabajo cuando [filtra](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail).

1. Haga clic en **Guardar**.

   ![](assets/eight-1.png)

