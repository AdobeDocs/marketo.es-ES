---
unique-page-id: 10095429
description: Corrección de problemas de sincronización de validación de Dynamics - Documentos de Marketo - Documentación del producto
title: Corregir problemas de sincronización de validación de Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Solucionar problemas de sincronización de validación de Dynamics {#fix-dynamics-validation-sync-issues}

## Validar resultados de la herramienta de sincronización {#validate-sync-tool-results}

Cuando ejecuta Dynamics Validate Sync, genera este informe. Si hay un ![delete](assets/delete.png) junto a un paso, consulte a continuación para identificar y solucionar el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado muestre únicamente marcas de verificación.

![](assets/image2015-9-22-15-3a58-3a12.png)

## La dirección URL es válida {#url-is-valid}

Si tiene una ![delete](assets/delete.png) aquí, compruebe que la dirección URL sea válida. Lo encontrará aquí en Recursos para desarrolladores y consulte el servicio de organización. La dirección URL puede no ser válida por varios motivos.

1. Inicie sesión en Dynamics. Haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en Configuración y seleccione **Personalizaciones**.

   ![](assets/two.png)

1. Haga clic en **Developer Resources**.

   ![](assets/three.png)

1. La URL del servicio de organización se encuentra en Puntos de conexión de servicio.

   ![](assets/four.png)

## El nombre de usuario y la contraseña son válidos {#username-and-password-are-valid}

Si tiene un ![—](assets/delete.png) aquí, compruebe que su nombre de usuario y contraseña de Microsoft Dynamics son válidos.

## El usuario de sincronización está asignado a la función de usuario de sincronización de Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si tiene un ![—](assets/delete.png) aquí, debe comprobar que la función de usuario de sincronización de Marketo está marcada en Microsoft Dynamics. Consulte el paso 2 de la documentación de instalación de Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Settings** y seleccione **Security**.

   ![](assets/six.png)

1. Haga clic en **Usuarios.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Haga clic en el vínculo del usuario de sincronización.

   ![](assets/seven.png)

1. Haga clic en **Administrar funciones**.

   ![](assets/eight.png)

1. Compruebe que la función de usuario de sincronización de Marketo esté marcada. Si no es así, compruébelo y haga clic en **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## La solución Marketo está instalada correctamente {#marketo-solution-is-properly-installed}

Si tiene un ![—](assets/delete.png) aquí, vaya a Microsoft Dynamics para comprobar que la instalación de Marketo está allí. Consulte el paso 1 de la documentación de configuración de Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Configuración** y seleccione **Soluciones.**

   ![](assets/eleven.png)

1. Compruebe que la solución esté incluida en la lista.

   ![](assets/twelve.png)

## Todos los pasos de la solución están habilitados {#all-steps-in-the-solution-are-enabled}

Si tiene un ![—](assets/delete.png) aquí, compruebe que no se haya desactivado ninguno de los pasos predeterminados. Todos los pasos se activan automáticamente en la instalación, pero se pueden desactivar durante una personalización.

## El usuario de sincronización está asignado a la solución de Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Si tiene un ![—](assets/delete.png) aquí, asegúrese de que el usuario de sincronización esté asignado en la página predeterminada de Marketo en Microsoft Dynamics.

1. En Dynamics, haga clic en el icono Configuración y seleccione **Configuración avanzada**.

   ![](assets/one.png)

1. Haga clic en **Settings** y seleccione **Marketo Config**.

   ![](assets/thirteen.png)

1. Compruebe que el usuario de sincronización está asignado como predeterminado.

   ![](assets/fourteen.png)

## El usuario de sincronización coincide con el nombre de usuario y la contraseña {#sync-user-matches-username-and-password}

Si tiene un ![—](assets/delete.png) aquí, asegúrese de asignar el usuario de sincronización adecuado en el campo Usuario de Marketo en el paso Configuración predeterminada de Marketo en Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Validar Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
