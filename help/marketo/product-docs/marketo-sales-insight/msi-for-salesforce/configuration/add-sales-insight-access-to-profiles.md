---
description: Acceso a los perfiles con información sobre ventas - Documentos de Marketo - Documentación del producto
title: Añadir el acceso de Sales Insight a los perfiles
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Añadir el acceso de Sales Insight a los perfiles {#add-sales-insight-access-to-profiles}

A continuación, le explicamos cómo crear un perfil con acceso a Sales Insight mientras elimina el acceso a los demás perfiles. Esto es para los usuarios que ya han instalado [Paquete de AppExchange de Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Si anteriormente ha proporcionado acceso a Sales Insight a todos los perfiles, debe [eliminar acceso de nivel de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} para utilizar este conjunto de permisos.

## Crear un nuevo perfil para la perspectiva de ventas {#create-a-new-profile-for-sales-insight}

Si tiene un perfil dedicado para los usuarios de perspectivas de ventas, puede omitir este paso.

1. En Salesforce, vaya a la página de configuración.

1. Busque perfiles en Búsqueda rápida y seleccione **Perfil** opción.

1. Haga clic en **Nuevo perfil** en la parte superior de la página.

1. Elija un perfil para clonar y asígnele un nombre (por ejemplo: usuario de Sales Insight).

1. Clic **Guardar** cuando termine.

## Añadir permisos de Sales Insight {#add-sales-insight-permissions}

1. Vuelva a la lista de perfiles.

1. Haga clic en **Editar** para el nuevo perfil que acaba de crear (o cualquier otro perfil existente al que desee dar acceso a Sales Insight).

1. En la página de edición, deberá cambiar algunas opciones de configuración.

   **Para perfiles con acceso permitido a Sales Insight**:

   * En Configuración de pestaña, cambie las pestañas de Marketo a Predeterminado activado
   * En Permisos de objetos personalizados, marque Leer, Crear, Editar y Eliminar en Configuración de Marketo Sales Insight (si el usuario debe tener acceso a la configuración, que suele utilizarse para administradores)

   **Para perfiles a los que no se les permite acceder a Sales Insight**:

   * En Configuración de pestaña, cambie las pestañas de Marketo a Pestaña oculta
   * En Permisos de objetos personalizados, desmarque Leer, Crear, Editar y Eliminar en Configuración de Marketo Sales Insight

1. Clic **Guardar** cuando termine.

## Crear diseño para la perspectiva de ventas {#create-layout-for-sales-insight}

1. Vaya a la página de configuración y haga clic en **Configuración de aplicación** > **Personalizar** > **Posibles clientes** > **Diseños de página**. Luego haga clic en **Nuevo** botón.

1. Clone el diseño que desee y asígnele un nombre apropiado (por ejemplo, Diseño de perspectiva de ventas).

1. Clic **Guardar** cuando termine.

1. Repita estos pasos para los diseños de página de Contactos, Oportunidades y Cuentas.

## Asignar perfil al diseño {#assign-profile-to-layout}

1. Vuelva a la sección Diseños de página y haga clic en **Asignación de diseño de página** botón.

1. Seleccionar **Editar asignación**.

1. Seleccione el perfil de perspectiva de ventas de la lista y, a continuación, seleccione el diseño de perspectiva de ventas en la lista desplegable &quot;Seleccionar diseño de página&quot;.

1. Clic **Guardar** cuando termine.

1. Repita estos pasos para los diseños de página de Contactos, Oportunidades y Cuentas.

## Otros cambios {#other-changes}

Estos son otros lugares en los que podrían aparecer artículos de Información de ventas. Tendrá que eliminarlos directamente, ya que no puede utilizar Perfiles para limitar su acceso:

* Eliminar los botones de perspectiva de ventas de los diseños de búsqueda para contactos, posibles clientes y cuentas
* Eliminar columnas de perspectiva de ventas de las listas de contactos y posibles clientes
