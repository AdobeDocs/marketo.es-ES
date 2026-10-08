---
description: Aprenda a reconfigurar el método de autenticación de Dynamics en Marketo. Deshabilite la sincronización, utilice Volver a configurar nuevo método de autenticación y valide las credenciales para la API web o ROPC.
title: Volver a configurar el método de autenticación [!DNL Dynamics]
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/wRcBTP-m1VtKDg6L4zrH6zzPIvrFuMEPQd5QoSrrm3I'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%
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

1. Seleccione el nuevo Método de autenticación que desee (en este ejemplo, se selecciona API web).

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
