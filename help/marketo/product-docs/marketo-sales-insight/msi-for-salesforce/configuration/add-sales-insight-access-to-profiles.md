---
description: 'Agregar acceso a perspectivas de ventas a perfiles: documentos de Marketo: documentación del producto'
title: Agregar el acceso a la perspectiva de ventas a los perfiles
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Agregar el acceso a la perspectiva de ventas a los perfiles {#add-sales-insight-access-to-profiles}

A continuación se explica cómo crear un perfil con acceso a la perspectiva de ventas al eliminar el acceso para los demás perfiles. Esto es para usuarios que ya han instalado el [Paquete de AppExchange de Insight de ventas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}.

>[!IMPORTANT]
>
>Si anteriormente ha concedido acceso a Sales Insight a todos los perfiles, debe [quitar acceso a nivel de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;} para usar este conjunto de permisos.

## Crear un nuevo perfil para la perspectiva de ventas {#create-a-new-profile-for-sales-insight}

Si tiene un perfil dedicado para sus usuarios de Perspectiva de ventas, puede omitir este paso.

1. En Salesforce, vaya a la página Configuración .

1. Busque perfiles en Búsqueda rápida y seleccione la opción **Perfil** .

1. Haga clic en el **Nuevo perfil** en la parte superior de la página.

1. Elija un perfil para clonar y asígnele un nombre (por ejemplo: usuario de perspectiva de ventas).

1. Haga clic en **Guardar** cuando haya terminado.

## Agregar permisos de perspectiva de ventas {#add-sales-insight-permissions}

1. Vuelva a la lista Perfiles.

1. Haga clic en el **Editar** vínculo para el nuevo perfil que acaba de crear (o cualquier otro perfil existente al que desee otorgar acceso a la perspectiva de ventas).

1. En la página de edición, tendrá que cambiar algunas opciones de configuración.

   **Para perfiles a los que se permite acceder a la perspectiva de ventas**:

   * En Configuración de pestañas, cambie las pestañas de Marketo a Predeterminado activado
   * En Permisos de objeto personalizados, marque Leer, Crear, Editar y Eliminar en la Configuración de perspectiva de ventas de Marketo (si el usuario debe tener acceso a la configuración de configuración, que normalmente se utiliza para los administradores)

   **Para perfiles a los que no se permite el acceso a la perspectiva de ventas**:

   * En Configuración de pestañas, cambie las pestañas de Marketo a Oculto de tabulación
   * En Permisos de objeto personalizados, desmarque Leer, Crear, Editar y Eliminar en la configuración de perspectiva de ventas de Marketo


1. Haga clic en **Guardar** cuando haya terminado.

## Crear diseño para la perspectiva de ventas {#create-layout-for-sales-insight}

1. Vaya a la página Configuración y, a continuación, haga clic en **Configuración de la aplicación** > **Personalizar** > **Posibles clientes** > **Diseños de página**. A continuación, haga clic en el **Nuevo** botón.

1. Clone el diseño que desee y asígnele un nombre adecuado (por ejemplo: Diseño de perspectiva de ventas).

1. Haga clic en **Guardar** cuando haya terminado.

1. Repita estos pasos para los diseños de página de Contactos, Oportunidades y Cuentas.

## Asignar perfil al diseño {#assign-profile-to-layout}

1. Vuelva a la sección Diseños de página y haga clic en el botón **Asignación de diseño de página** botón.

1. Select **Editar asignación**.

1. Seleccione su perfil de perspectiva de ventas en la lista y, a continuación, seleccione el diseño de perspectiva de ventas en la lista desplegable &quot;Seleccionar diseño de página&quot;.

1. Haga clic en **Guardar** cuando haya terminado.

1. Repita estos pasos para los diseños de página de Contactos, Oportunidades y Cuentas.

## Otros cambios {#other-changes}

Aquí hay otros lugares donde podrían aparecer artículos de perspectivas de ventas. Tendrá que eliminarlos directamente, ya que no puede usar Perfiles para limitar su acceso:

* Eliminar los botones de perspectiva de ventas de Buscar diseños para contactos, posibles clientes y cuentas
* Eliminar las columnas de perspectivas de ventas de las listas de contactos y posibles clientes
