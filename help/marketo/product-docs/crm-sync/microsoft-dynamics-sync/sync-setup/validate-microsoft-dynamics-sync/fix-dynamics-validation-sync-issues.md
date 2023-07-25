---
unique-page-id: 10095429
description: Corregir problemas de sincronización de validación de Dynamics - Documentos de Marketo - Documentación del producto
title: Corregir problemas de sincronización de validación de Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Corregir problemas de sincronización de validación de Dynamics {#fix-dynamics-validation-sync-issues}

## Validar resultados de la herramienta de sincronización {#validate-sync-tool-results}

Al ejecutar la sincronización de validación de Dynamics, se genera un informe. Si hay un... ![x](assets/delete.png) al lado del paso, consulte las siguientes opciones para identificar y corregir el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado muestre únicamente marcas de verificación verdes.

![](assets/image2015-9-22-15-3a58-3a12.png)

## La URL es válida {#url-is-valid}

Si tiene un ![x](assets/delete.png) En este caso, compruebe que la dirección URL sea válida. Encuéntralo aquí en Recursos para desarrolladores y consulte el Servicio de organización. La URL podría no ser válida por varios motivos.

1. Inicie sesión en Dynamics. Haga clic en el icono Settings y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en Configuración y seleccione **Personalizaciones**.

   ![](assets/two.png)

1. Clic **Recursos para desarrolladores**.

   ![](assets/three.png)

1. La URL del servicio de organización se encuentra en Extremos de servicio.

   ![](assets/four.png)

## El nombre de usuario y la contraseña son válidos {#username-and-password-are-valid}

Si tiene un ![x](assets/delete.png) En este caso, compruebe que sus credenciales de Microsoft Dynamics son válidas. Para la autenticación S2S de la API web, el nombre de usuario en Marketo debe coincidir con el de [dirección de email](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) del usuario de la aplicación en CRM. Para otros tipos, debe coincidir con el nombre de usuario del usuario de sincronización.

## El usuario de sincronización se ha asignado a la función de usuario de sincronización de Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si tiene un ![x](assets/delete.png) en este caso, podría ser una de las tres cuestiones siguientes.

**Opción uno: compruebe que la función de usuario de sincronización de Marketo esté marcada en Microsoft Dynamics**:

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Clic **Configuración** y seleccione **Seguridad**.

   ![](assets/six.png)

1. Clic **Usuarios.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Haga clic en el vínculo del usuario de sincronización.

   ![](assets/seven.png)

1. Clic **Administrar funciones**.

   ![](assets/eight.png)

1. Compruebe que la función de usuario de sincronización de Marketo esté seleccionada. Si no es así, márquelo y haga clic en **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Opción dos: Confirmar consentimiento de concesión**:

1. Revise la [Conceder consentimiento para el ID de cliente y el registro de aplicaciones](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) para confirmar que la aplicación tiene consentimiento de administrador para llamar a las API de.

**Opción tres: Sincronizar usuario**:

1. Compruebe que el usuario de sincronización se ha agregado a la configuración de Marketo.

## La solución Marketo está correctamente instalada {#marketo-solution-is-properly-installed}

Si tiene un ![x](assets/delete.png) En este caso, vaya a Microsoft Dynamics para comprobar que la instalación de Marketo está allí. Consulte el paso 1 de la documentación de configuración de Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Clic **Configuración** y seleccione **Soluciones.**

   ![](assets/eleven.png)

1. Compruebe que la solución aparece en la lista.

   ![](assets/twelve.png)

## Todos los pasos de la solución están activados {#all-steps-in-the-solution-are-enabled}

Si tiene un ![x](assets/delete.png) en este caso, compruebe que no se ha desactivado ninguno de los pasos predeterminados. Todos los pasos se activan automáticamente durante la instalación, pero podrían desactivarse durante una personalización.

## El usuario de sincronización está asignado a la solución de Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Si tiene un ![x](assets/delete.png) Aquí, asegúrese de que el usuario de sincronización está asignado en la página predeterminada de Marketo en Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Clic **Configuración** y seleccione **Configuración de Marketo**.

   ![](assets/thirteen.png)

1. Compruebe que el usuario de sincronización está asignado como predeterminado.

   ![](assets/fourteen.png)

## El usuario de sincronización coincide con el nombre de usuario y contraseña {#sync-user-matches-username-and-password}

Si tiene un ![x](assets/delete.png) Aquí, asegúrese de asignar el usuario de sincronización adecuado en el campo Usuario de Marketo en el paso Configuración predeterminada de Marketo en Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
