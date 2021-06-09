---
description: Configuración de la perspectiva de ventas para su equipo - Marketo Docs - Documentación del producto
title: Configuración de la perspectiva de ventas para su equipo
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: ecceb1a3aff3a2088379f8f4f2ac33e566f90e21
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Configuración de la perspectiva de ventas para su equipo {#setting-up-sales-insight-for-your-team}

A continuación se explica cómo crear un perfil con acceso a la perspectiva de ventas al eliminar el acceso para los demás perfiles. Esto es para usuarios que ya han instalado el [paquete de AppExchange de perspectiva de ventas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).

## Crear un nuevo perfil para la perspectiva de ventas {#create-a-new-profile-for-sales-insight}

Si tiene un perfil dedicado para sus usuarios de Perspectiva de ventas, puede omitir este paso.

1. En Salesforce, vaya a la página Configuración .

1. Busque perfiles en Búsqueda rápida y seleccione la opción **Perfil** .

1. Haga clic en el botón **Nuevo perfil** en la parte superior de la página.

1. Elija un perfil para clonar y asígnele un nombre (por ejemplo: usuario de perspectiva de ventas).

1. Haga clic en **Guardar** cuando termine.

## Agregar permisos de perspectiva de ventas {#add-sales-insight-permissions}

1. Vuelva a la lista Perfiles.

1. Haga clic en el enlace **Edit** del nuevo perfil que acaba de crear (o en cualquier otro perfil existente al que desee otorgar acceso a la perspectiva de ventas).

1. En la página de edición, tendrá que cambiar algunas opciones de configuración.

   **Para perfiles a los que se permite acceder a la perspectiva** de ventas:

   * En Configuración de pestañas, cambie las pestañas de Marketo a Predeterminado activado
   * En Permisos de objeto personalizados, marque Leer, Crear, Editar y Eliminar en la Configuración de perspectiva de ventas de Marketo (si el usuario debe tener acceso a la configuración de configuración, que normalmente se utiliza para los administradores)

   **Para perfiles a los que no se permite el acceso a la perspectiva** de ventas:

   * En Configuración de pestañas, cambie las pestañas de Marketo a Oculto de tabulación
   * En Permisos de objeto personalizados, desmarque Leer, Crear, Editar y Eliminar en la configuración de perspectiva de ventas de Marketo


1. Haga clic en **Guardar** cuando termine.

## Crear diseño para la perspectiva de ventas {#create-layout-for-sales-insight}

1. Vaya a la página Configuración y, a continuación, haga clic en **Configuración de la aplicación** > **Personalizar** > **Posibles clientes** > **Diseños de la página**. A continuación, haga clic en el botón **New**.

1. Clone el diseño que desee y asígnele un nombre adecuado (por ejemplo: Diseño de perspectiva de ventas).

1. Haga clic en **Guardar** cuando termine.

1. Repita estos pasos para los diseños de página de Contactos, Oportunidades y Cuentas.

## Asignar perfil al diseño {#assign-profile-to-layout}

1. Vuelva a la sección Diseños de página y haga clic en el botón **Asignación de diseño de página**.

1. Seleccione **Editar asignación**.

1. Seleccione su perfil de perspectiva de ventas en la lista y, a continuación, seleccione el diseño de perspectiva de ventas en la lista desplegable &quot;Seleccionar diseño de página&quot;.

1. Haga clic en **Guardar** cuando termine.

1. Repita estos pasos para los diseños de página de Contactos, Oportunidades y Cuentas.

## Otros cambios {#other-changes}

Aquí hay otros lugares donde podrían aparecer artículos de perspectivas de ventas. Tendrá que eliminarlos directamente, ya que no puede usar Perfiles para limitar su acceso:

* Eliminar los botones de perspectiva de ventas de Buscar diseños para contactos, posibles clientes y cuentas
* Eliminar las columnas de perspectivas de ventas de las listas de contactos y posibles clientes
