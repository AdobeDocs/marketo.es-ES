---
unique-page-id: 8783322
description: 'Validación de Microsoft Dynamics Sync: Documentos de Marketo: Documentación del producto'
title: Validar Microsoft Dynamics Sync
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Validar Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Si tiene Multi-Factor Authentication (MFA) habilitado para Dynamics Sync, debe deshabilitarlo para que Dynamics se sincronice correctamente con Marketo. Para obtener más información, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

## Ejecutar Validar sincronización en Marketo {#run-validate-sync-in-marketo}

Es muy importante ejecutar la herramienta Validar sincronización para asegurarse de que la sincronización de Microsoft Dynamics con Marketo esté correctamente configurada antes de establecer la conexión final entre ellas. El proceso genera una lista de comprobación de siete pasos de configuración que señalan dónde existen problemas. Verificar que se hayan realizado correctamente puede ahorrar mucho tiempo después.

1. Haga clic en el **Administrador** y, a continuación, **Microsoft Dynamics** en el área Integración.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Select **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Haga clic en el **Validar la configuración de sincronización** pestaña .

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Introduzca su nombre de usuario, contraseña y dirección URL (el ID de cliente y el Secreto de cliente son opcionales). Haga clic en **Siguiente** cuando haya terminado.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Si ha sincronizado antes, **CRM** en el árbol de la izquierda se leerá **Microsoft Dynamics**, y los datos del formulario anterior pueden rellenarse previamente.

1. Si todo está bien, Validar sincronización genera una lista de comprobación llena de marcas de verificación verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Si ve una ![—](assets/delete.png), entonces ese paso tiene un problema. Consulte [Corregir problemas de sincronización de validación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para identificar y solucionar el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado se asemeje a la imagen anterior.

   >[!CAUTION]
   >
   >Actualmente no se admite la actualización de entornos limitados para Marketo Dynamics Sync. Si necesita actualizar el simulador para pruebas de Dynamics CRM, se necesitará un nuevo simulador para pruebas de Marketo. Póngase en contacto con el equipo de cuentas de Adobe (su administrador de cuentas) para obtener más información.

>[!MORELIKETHIS]
>
>[Corregir problemas de sincronización de validación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
