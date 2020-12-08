---
unique-page-id: 10095429
description: Corregir problemas de sincronización de validación de Dynamics - Documentos de marketing - Documentación del producto
title: Corregir problemas de sincronización de validación de Dynamics
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Corregir problemas de sincronización de validación de Dynamics {#fix-dynamics-validation-sync-issues}

## Validar los resultados de la herramienta de sincronización {#validate-sync-tool-results}

Al ejecutar la sincronización de validación dinámica, se genera este informe. Si hay una ![eliminación](assets/delete.png) al lado de un paso, consulte a continuación para identificar y solucionar el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado no muestre más que marcas de verificación.

![](assets/image2015-9-22-15-3a58-3a12.png)

## La dirección URL es válida {#url-is-valid}

Si tiene una ![eliminación](assets/delete.png) aquí, compruebe que la dirección URL sea válida. Encuéntralo aquí en Recursos para desarrolladores y consulte el servicio de organización. La dirección URL puede no ser válida por varios motivos.

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione Configuración **avanzada**.

   ![](assets/one.png)

1. Haga clic en Configuración y seleccione **Personalizaciones**.

   ![](assets/two.png)

1. Haga clic en Recursos **para desarrolladores**.

   ![](assets/three.png)

1. La dirección URL del servicio de organización se encuentra en Extremos de servicio.

   ![](assets/four.png)

## El nombre de usuario y la contraseña son válidos {#username-and-password-are-valid}

Si tiene un ![—](assets/delete.png) aquí, compruebe que el nombre de usuario y la contraseña de Microsoft Dynamics son válidos.

## El usuario de sincronización está asignado a la función de usuario de sincronización de marketing {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si tiene un ![—](assets/delete.png) aquí, debe comprobar que la función Usuario de sincronización de marketing está marcada en Microsoft Dynamics. Consulte el paso 2 de la documentación de instalación de MIcrosoft Dynamics.

1. En Dinámica, haga clic en el icono Configuración y seleccione Configuración **avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración** y seleccione **Seguridad**.

   ![](assets/six.png)

1. Haga clic en **Usuarios.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Haga clic en el vínculo del usuario de sincronización.

   ![](assets/seven.png)

1. Haga clic en **Administrar funciones**.

   ![](assets/eight.png)

1. Compruebe que la función de usuario de sincronización de marketing está activada. Si no es así, márquelo y haga clic en **Aceptar.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## La solución de marketing está correctamente instalada {#marketo-solution-is-properly-installed}

Si tiene un ![—](assets/delete.png) aquí, vaya a Microsoft Dynamics para comprobar que la instalación de Marketing está allí. Consulte el paso 1 de la documentación de configuración de MIcrosoft Dynamics.

1. En Dinámica, haga clic en el icono Configuración y seleccione Configuración **avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración **y seleccione **Soluciones.**

   ![](assets/eleven.png)

1. Verifique que la solución esté enumerada.

   ![](assets/twelve.png)

## Todos los pasos de la solución están activados {#all-steps-in-the-solution-are-enabled}

Si tiene un ![—](assets/delete.png) aquí, compruebe que no se haya desactivado ninguno de los pasos predeterminados. Todos los pasos se activan automáticamente durante la instalación, pero se pueden desactivar durante una personalización.

## El usuario de sincronización está asignado a la solución de marketing {#sync-user-is-assigned-to-the-marketo-solution}

Si tiene un ![—](assets/delete.png) aquí, asegúrese de que el usuario de sincronización está asignado en la página predeterminada de marketing de Microsoft Dynamics.

1. En Dinámica, haga clic en el icono Configuración y seleccione Configuración **avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración **y seleccione **Configuración** de marketing.

   ![](assets/thirteen.png)

1. Compruebe que el usuario de sincronización está asignado como predeterminado.

   ![](assets/fourteen.png)

## El usuario de sincronización coincide con el nombre de usuario y la contraseña {#sync-user-matches-username-and-password}

Si tiene un ![—](assets/delete.png) aquí, asegúrese de asignar el usuario de sincronización adecuado en el campo Usuario de marketing en el paso Configuración predeterminada de marketing en Microsoft Dynamics.

>[!NOTE]
>
>**Artículos relacionados**
>
>[Validar Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

