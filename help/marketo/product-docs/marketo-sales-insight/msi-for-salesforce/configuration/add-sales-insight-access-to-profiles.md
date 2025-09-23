---
description: Añadir el acceso de Insight de ventas a los perfiles - Documentos de Marketo - Documentación del producto
title: Añadir el acceso de Sales Insight a los perfiles
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 5%

---

# Agregar acceso de [!DNL Sales Insight] a perfiles {#add-sales-insight-access-to-profiles}

A continuación se indica cómo crear un perfil con acceso a [!DNL Sales Insight] mientras se elimina el acceso a los demás perfiles. Esto es para usuarios que ya han instalado el [[!DNL Sales Insight] paquete de AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Si anteriormente dio acceso a [!DNL Sales Insight] a todos los perfiles, debe [quitar el acceso de nivel de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} para usar este conjunto de permisos.

## Crear nuevo perfil para [!DNL Sales Insight] {#create-a-new-profile-for-sales-insight}

Si tiene un perfil dedicado para los usuarios de [!DNL Sales Insight], puede omitir este paso.

1. En [!DNL Salesforce], vaya a la página de instalación.

1. Busque perfiles en Búsqueda rápida y seleccione la opción **[!UICONTROL Perfil]**.

1. Haga clic en el botón **[!UICONTROL Nuevo perfil]** en la parte superior de la página.

1. Elija un perfil para clonar y asígnele un nombre (por ejemplo: Usuario de Insight de ventas).

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.

## Agregar permisos de [!DNL Sales Insight] {#add-sales-insight-permissions}

1. Vuelva a la lista de perfiles.

1. Haga clic en el vínculo **[!UICONTROL Editar]** del nuevo perfil que acaba de crear (o de cualquier otro perfil existente al que desee conceder acceso a [!DNL Sales Insight]).

1. En la página de edición, deberá cambiar algunas opciones de configuración.

   **Para perfiles con acceso permitido a[!DNL Sales Insight]**:

   * En Configuración de pestaña, cambie las pestañas de Marketo a Predeterminado activado
   * En Permisos de objetos personalizados, marque Leer, Crear, Editar y Eliminar en la configuración de [!DNL Marketo Sales Insight] (si el usuario debe tener acceso a la configuración, generalmente utilizada por los administradores)

   **Para perfiles a los que no se les permite el acceso a[!DNL Sales Insight]**:

   * En Configuración de pestaña, cambie las pestañas de Marketo a Pestaña oculta
   * En Permisos de objetos personalizados, desactive Leer, Crear, Editar y Eliminar en la configuración [!DNL Marketo Sales Insight]

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.

## Crear diseño para [!DNL Sales Insight] {#create-layout-for-sales-insight}

1. Vaya a la página Configuración y, a continuación, haga clic en **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Personalizar]** > **[!UICONTROL Posibles clientes]** > **[!UICONTROL Diseños de página]**. Luego haga clic en el botón **[!UICONTROL Nuevo]**.

1. Clone el diseño que desee y asígnele un nombre apropiado (p. ej.: Diseño de Insight de ventas).

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.

1. Repita estos pasos para los diseños de página de [!UICONTROL Contactos], [!UICONTROL Oportunidades] y [!UICONTROL Cuentas].

## Asignar perfil al diseño {#assign-profile-to-layout}

1. Vuelva a la sección Diseños de página y haga clic en el botón **[!UICONTROL Asignación de diseño de página]**.

1. Seleccione **[!UICONTROL Editar asignación]**.

1. Seleccione el perfil [!DNL Sales Insight] de la lista y, a continuación, seleccione el diseño [!DNL Sales insight] en la lista desplegable [!UICONTROL Seleccionar diseño de página]&quot;.

1. Haga clic en **[!UICONTROL Guardar]** cuando termine.

1. Repita estos pasos para los diseños de página de [!UICONTROL Contactos], [!UICONTROL Oportunidades] y [!UICONTROL Cuentas].

## Otros cambios {#other-changes}

Estos son otros lugares donde podrían aparecer [!DNL Sales Insight] elementos. Tendrá que eliminarlos directamente, ya que no puede utilizar Perfiles para limitar su acceso:

* Quitar los botones [!DNL Sales Insight] de los diseños de búsqueda de [!UICONTROL Contactos], [!UICONTROL Posibles clientes] y [!UICONTROL Cuentas]
* Quitar [!DNL Sales Insight] columnas de las listas de contactos y posibles clientes
