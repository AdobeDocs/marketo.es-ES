---
description: Volver a configurar  [!DNL Dynamics] método de autenticación - Documentos de Marketo - Documentación del producto
title: Volver a configurar  [!DNL Dynamics] método de autenticación
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Volver a configurar el método de autenticación de Dynamics {#reconfigure-dynamics-authentication-method}

Siga los pasos a continuación para actualizar su método de autenticación [!DNL Dynamics].

>[!PREREQUISITES]
>
>Configure la aplicación en [!DNL Microsoft Dynamics] y Active Directory (Azure AD/ADFS) utilizando el método de autenticación deseado en cualquiera de los siguientes artículos:
>
>* [Paso 2 de 3: Configurar la solución de Marketo con conexión de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
>* [Paso 2 de 4: Configurar la solución Marketo con conexión de control de contraseña de propietario de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. En Marketo, haga clic en **[!UICONTROL Admin]**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Haga clic en **Microsoft Dynamics** y luego en **[!UICONTROL Deshabilitar sincronización]**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Debe deshabilitar la sincronización global temporalmente para actualizar el Método de autenticación.

1. Haga clic en la ficha **[!UICONTROL Volver a configurar nuevo método de autenticación]**.

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Seleccione el nuevo método de autenticación que desee (en este ejemplo, elegimos API web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Escriba las credenciales necesarias para el nuevo método de autenticación y haga clic en **[!UICONTROL Validar]**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* Los campos específicos variarán según el método de autenticación elegido y el formulario se actualizará automáticamente en función del método de autenticación anterior.
   >* Si ha realizado la sincronización anteriormente, es posible que los datos del formulario anterior se rellenen previamente. Vuelva a introducir todas las credenciales para asegurarse de que los valores son correctos.

1. Si todo está bien, Validar sincronización generará todas las marcas de verificación verdes ![](assets/green-check.png). Revise el mensaje y haga clic en **[!UICONTROL Cambiar]** para actualizar el método de autenticación.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Si ve un(a) ![](assets/red-x.png), ese paso presenta un problema. Vea [Corregir [!DNL Dynamics] problemas de sincronización de validación](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para identificar y corregir los problemas. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado se parezca a la imagen anterior.

1. Haga clic en **[!UICONTROL Confirmar]** para continuar.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Vuelva a hacer clic en **[!UICONTROL Confirmar]**.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Haga clic en **[!UICONTROL Aceptar]**.

   >[!IMPORTANT]
   >
   >El sistema tarda 15 minutos en aceptar el nuevo modo de autenticación. Espere 15 minutos desde el momento del cambio antes de volver a activar la sincronización.
