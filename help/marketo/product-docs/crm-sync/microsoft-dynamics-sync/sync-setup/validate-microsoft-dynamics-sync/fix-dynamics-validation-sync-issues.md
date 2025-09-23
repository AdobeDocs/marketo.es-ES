---
unique-page-id: 10095429
description: Corregir problemas de sincronización de validación de Dynamics - Documentos de Marketo - Documentación del producto
title: Corregir problemas de sincronización de validación de Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 9%

---

# Corregir problemas de sincronización de validación de Dynamics {#fix-dynamics-validation-sync-issues}

## Validar resultados de la herramienta de sincronización {#validate-sync-tool-results}

Al ejecutar la sincronización de validación de Dynamics, se genera un informe. Si hay un ![x](assets/delete.png) junto a un paso, consulta las siguientes opciones para identificar y solucionar el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado muestre únicamente marcas de verificación verdes.

![](assets/image2015-9-22-15-3a58-3a12.png)

## La URL es válida {#url-is-valid}

Si tiene un ![x](assets/delete.png) aquí, compruebe que la dirección URL sea válida. Encuéntralo aquí en Recursos para desarrolladores y consulte el Servicio de organización. La URL podría no ser válida por varios motivos.

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en Configuración y seleccione **Personalizaciones**.

   ![](assets/two.png)

1. Haga clic en **Recursos para desarrolladores**.

   ![](assets/three.png)

1. La URL del servicio de organización se encuentra en Extremos de servicio.

   ![](assets/four.png)

## El nombre de usuario y la contraseña son válidos {#username-and-password-are-valid}

Si tiene un ![x](assets/delete.png) aquí, verifique que sus credenciales de Microsoft Dynamics sean válidas. Para la autenticación S2S de la API web, el nombre de usuario en Marketo debe coincidir con la [dirección de correo electrónico](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) del usuario de la aplicación en CRM. Para otros tipos, debe coincidir con el nombre de usuario del usuario de sincronización.

## El usuario de sincronización se ha asignado a la función de usuario de sincronización de Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si tiene un ![x](assets/delete.png) aquí, podría ser uno de los tres problemas siguientes.

**Opción uno: compruebe que la función de usuario de sincronización de Marketo esté marcada en Microsoft Dynamics**:

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración** y seleccione **Seguridad**.

   ![](assets/six.png)

1. Haga clic en **Usuarios.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Haga clic en el vínculo del usuario de sincronización.

   ![](assets/seven.png)

1. Haga clic en **Administrar roles**.

   ![](assets/eight.png)

1. Compruebe que la función de usuario de sincronización de Marketo esté seleccionada. Si no, compruébelo y haga clic en **Aceptar.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Opción dos - Confirmar consentimiento de concesión**:

1. Revise [Conceder consentimiento para el ID de cliente y el registro de la aplicación](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) para confirmar que la aplicación tiene consentimiento de administrador para llamar a las API.

**Opción tres - Sincronizar usuario**:

1. Compruebe que el usuario de sincronización se ha agregado a la configuración de Marketo.

## La solución de Marketo está correctamente instalada {#marketo-solution-is-properly-installed}

Si tiene un ![x](assets/delete.png) aquí, vaya a Microsoft Dynamics para comprobar que la instalación de Marketo esté allí. Consulte el paso 1 de la documentación de configuración de Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración** y seleccione **Soluciones.**

   ![](assets/eleven.png)

1. Compruebe que la solución aparece en la lista.

   ![](assets/twelve.png)

## Todos los pasos de la solución están habilitados {#all-steps-in-the-solution-are-enabled}

Si tiene un ![x](assets/delete.png) aquí, compruebe que no se haya desactivado ninguno de los pasos predeterminados. Todos los pasos se activan automáticamente durante la instalación, pero podrían desactivarse durante una personalización.

## El usuario de sincronización está asignado a la solución de Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Si tiene un ![x](assets/delete.png) aquí, asegúrese de que el usuario de sincronización esté asignado en la página predeterminada de Marketo en Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración** y seleccione **Configuración de Marketo**.

   ![](assets/thirteen.png)

1. Compruebe que el usuario de sincronización está asignado como predeterminado.

   ![](assets/fourteen.png)

## El usuario de sincronización coincide con el nombre de usuario y la contraseña {#sync-user-matches-username-and-password}

Si tiene un ![x](assets/delete.png) aquí, asegúrese de asignar el usuario de sincronización adecuado en el campo Usuario de Marketo en el paso Configuración predeterminada de Marketo en Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Validar sincronización de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
