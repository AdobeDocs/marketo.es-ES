---
description: Volver a configurar el método de autenticación de Dynamics - Documentos de Marketo - Documentación del producto
title: Reconfiguración del método de autenticación de Dynamics
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
source-git-commit: 8d401eeba46dc1b21983ea03c8ecd823046a5479
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Reconfiguración del método de autenticación de Dynamics {#reconfigure-dynamics-authentication-method}

Siga los pasos a continuación para actualizar su método de autenticación de Dynamics.

>[!PREREQUISITES]
>
>Configure la aplicación en Microsoft Dynamics y el directorio activo (Azure AD/ADFS) utilizando el método de autenticación deseado desde cualquiera de los siguientes artículos:
>* [Paso 2 de 3: Configurar la solución de Marketo con conexión de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [Paso 2 de 4: Configurar la solución de Marketo con la conexión de control de contraseña del propietario del recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. En Marketo, haga clic en **Administrador**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Haga clic en **Microsoft Dynamics**, luego **Desactivar sincronización**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Debe desactivar la sincronización global temporalmente para actualizar el método de autenticación.

1. Haga clic en el **Reconfigurar nuevo método de autenticación** pestaña .

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Seleccione el nuevo método de autenticación deseado (en este ejemplo elegimos la API web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Introduzca las credenciales necesarias para el nuevo método de autenticación y haga clic en **Validar**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* Los campos específicos variarán según el método de autenticación elegido y el formulario se actualizará automáticamente según el método de autenticación anterior.
   >* Si ha sincronizado antes, es posible que los datos del formulario anterior se rellenen previamente. Vuelva a introducir todas las credenciales para asegurarse de que los valores son correctos.


1. Si todo está bien, Validar sincronización generará todas las marcas de verificación verdes ![](assets/green-check.png). Revise el mensaje y haga clic en **Conmutador** para actualizar el método de autenticación.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Si ve una ![](assets/red-x.png), ese paso tiene un problema. Consulte [Corregir problemas de sincronización de validación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para identificar y solucionar los problemas. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado se asemeje a la imagen anterior.

1. Haga clic en **Confirmar** para continuar.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Haga clic en **Confirmar** de nuevo.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Haga clic en **OK**.

   >[!IMPORTANT]
   >
   >El sistema tarda 15 minutos en aceptar el nuevo modo de autenticación. Espere 15 minutos desde la hora del conmutador antes de volver a activar la sincronización.
