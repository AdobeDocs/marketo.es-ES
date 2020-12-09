---
unique-page-id: 8783322
description: Validar Microsoft Dynamics Sync - Documentos de marketing - Documentación del producto
title: Validar Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Validar Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Si tiene Multi-Factor Authentication (MFA) habilitado para Dynamics Sync, debe deshabilitarlo para que Dynamics se sincronice correctamente con Marketing. Para obtener más información, póngase en contacto con la asistencia técnica [de marketing](http://nation.marketo.com/community/support_solutions).

## Ejecutar Validar sincronización en Marketing {#run-validate-sync-in-marketo}

Es muy importante ejecutar la herramienta Validar sincronización para asegurarse de que Microsoft Dynamics Sync con Marketing está correctamente configurado antes de establecer la conexión final entre ellos. El proceso genera una lista de siete pasos de configuración que señalan dónde se producen problemas. La verificación de que se han realizado correctamente puede ahorrar mucho tiempo más tarde.

1. Haga clic en la ficha **Administración** y, a continuación, en el vínculo **Microsoft Dynamics** del área Integración.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Seleccione **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Haga clic en la ficha **Validar configuración** de sincronización.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Introduzca el nombre de usuario, la contraseña y la dirección URL (el ID de cliente y el secreto de cliente son opcionales). Haga clic en **Siguiente** cuando termine.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Si se ha sincronizado antes, **CRM** en el árbol izquierdo leerá **Microsoft Dynamics** y los datos del formulario anterior pueden rellenarse previamente.

1. Si todo está bien, Validar sincronización genera una lista de comprobación llena de marcas de verificación verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Si ve un ![—](assets/delete.png), ese paso tiene un problema. Consulte [Corregir problemas](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) de sincronización de validación de Dynamics para identificar y corregir el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado sea como la imagen anterior.

   >[!CAUTION]
   >
   >Actualmente no se admite la actualización del entorno limitado para Marketing Dynamics Sync. Si necesita actualizar el simulador para pruebas de Dynamics CRM, se necesitará un nuevo simulador para pruebas de Marketing. Póngase en contacto con el administrador de éxito del cliente para obtener más detalles.

>[!MORELIKETHIS]
>
>[Corregir problemas de sincronización de validación de Dynamics](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

