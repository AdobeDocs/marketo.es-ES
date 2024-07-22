---
unique-page-id: 8783322
description: 'Validar la sincronización de Microsoft Dynamics: documentos de Marketo, documentación del producto'
title: Validar sincronización de Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Validar sincronización de Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Si tiene habilitada la Autenticación de varios factores (MFA) para la sincronización de Dynamics, debe deshabilitarla para que Dynamics se sincronice correctamente con Marketo. Para obtener más información, comuníquese con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

## Ejecutar Validar sincronización en Marketo {#run-validate-sync-in-marketo}

Es muy importante ejecutar la herramienta Validar sincronización para asegurarse de que la sincronización de Microsoft Dynamics con Marketo esté configurada correctamente antes de establecer la conexión final entre ellas. El proceso genera una lista de comprobación de siete pasos de configuración que indican dónde existen problemas. Verificar que se hayan realizado correctamente puede ahorrar mucho tiempo más tarde.

1. Haga clic en la ficha **[!UICONTROL Admin]** y, a continuación, en el vínculo **[!DNL Microsoft Dynamics]** del área de integración.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Seleccione **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Haga clic en la ficha **[!UICONTROL Validar configuración de sincronización]**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Introduzca su nombre de usuario, contraseña y URL (el ID de cliente y el Secreto de cliente son opcionales). Haga clic en **[!UICONTROL Siguiente]** cuando haya terminado.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Si ha realizado la sincronización anteriormente, **[!UICONTROL CRM]** en el árbol izquierdo leerá **[!DNL Microsoft Dynamics]**, y es posible que los datos del formulario anterior se hayan rellenado previamente.

1. Si todo está bien, Validate Sync genera una lista de comprobación llena de marcas de verificación verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Si ve un(a) ![—](assets/delete.png), entonces ese paso tiene un problema. Consulte [Corregir problemas de sincronización de validación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} para identificar y corregir el problema. A continuación, vuelva a ejecutar los pasos de validación de sincronización hasta que el resultado se parezca a la imagen anterior.

   >[!CAUTION]
   >
   >Actualmente no se admite la actualización de la zona protegida para la sincronización de Marketo Dynamics. Si necesita actualizar la zona protegida de Dynamics CRM, se necesitará una nueva zona protegida de Marketo. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

>[!MORELIKETHIS]
>
>[Corregir problemas de sincronización de validación de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}
