---
unique-page-id: 12981050
description: Bloquear plantilla de ventas - Documentos de Marketo - Documentación del producto
title: Bloquear plantilla de ventas
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 4%

---

# Bloquear plantilla de ventas {#lock-sales-template}

Para evitar que los usuarios de CRM editen plantillas de ventas, los administradores pueden habilitar la capacidad de bloquear plantillas, lo que permite a los usuarios bloquear plantillas individualmente desde el editor de correo electrónico.

>[!CAUTION]
>
>Esta característica solo funciona para [!DNL Salesforce] y no es compatible con [!DNL Microsoft Dynamics] u otros CRM. Las plantillas a las que se accede desde los complementos de [!DNL Outlook] o Gmail no se bloquearán, ya que Marketo no controla el editor.

## Habilitar plantilla de bloqueo {#enable-lock-template}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya a **[!UICONTROL Administrador]** y, a continuación, haga clic en **[!UICONTROL Ventas Insight]**.

   ![](assets/1.png)

1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Editar]**.

   ![](assets/2.png)

1. Marque **[!UICONTROL Habilitar la capacidad para bloquear plantillas]**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>De forma predeterminada, esta casilla está activada y la capacidad de bloquear plantillas está activada. Si la desmarca, se desactivará la función de plantilla de bloqueo en el editor de correo electrónico.

>[!NOTE]
>
>Si se cambia esta configuración como administrador **no**, las plantillas existentes se verán afectadas de forma retroactiva; es decir, no se bloquearán automáticamente.

## Bloquear plantilla en el editor de correo electrónico {#lock-template-in-the-email-editor}

1. Seleccione el correo electrónico que desee bloquear y, a continuación, haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/5.png)

1. En el editor de correo electrónico, haga clic en **[!UICONTROL Configuración de correo electrónico]**.

   ![](assets/6.png)

1. Marque **[!UICONTROL Publicar en Marketo Sales Insight]** si aún no lo está. Ahora puede desmarcar **[!UICONTROL Permitir que el usuario de CRM edite el correo electrónico]** para bloquear la plantilla. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >De forma predeterminada, esta casilla está marcada y los usuarios de CRM pueden editar correos electrónicos.
