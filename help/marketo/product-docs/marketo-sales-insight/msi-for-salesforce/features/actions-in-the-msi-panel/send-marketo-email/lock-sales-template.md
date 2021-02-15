---
unique-page-id: 12981050
description: Bloquear plantilla de ventas - Documentos de marketing - Documentación del producto
title: Bloquear plantilla de ventas
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Bloquear plantilla de ventas {#lock-sales-template}

Para evitar que los usuarios de CRM editen plantillas de ventas, los administradores pueden habilitar la posibilidad de bloquear plantillas, lo que permite a los usuarios bloquear plantillas individualmente desde el editor de correo electrónico.

>[!CAUTION]
>
>Esta función solo funciona para Salesforce y no es compatible con Microsoft Dynamics u otros CRM. Las plantillas a las que se accede desde los complementos de Outlook o Gmail no se bloquearán, ya que el editor no está controlado por Marketing.

## Habilitar plantilla de bloqueo {#enable-lock-template}

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya a **Administración** y haga clic en **Perspectiva de ventas**.

   ![](assets/1.png)

1. En **Configuración**, haga clic en **Editar**.

   ![](assets/2.png)

1. Marque **Habilitar la capacidad de bloquear plantillas**. Haga clic en **Guardar**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>De forma predeterminada, esta casilla está activada y la capacidad de bloquear plantillas está activada. Al desmarcarla, se desactivará la función de plantilla de bloqueo en el editor de correo electrónico.

>[!NOTE]
>
>Si se cambia esta configuración como administrador, **no** afectará retroactivamente a las plantillas existentes; es decir, no los bloqueará automáticamente.

## Bloquear plantilla en el Editor de correo electrónico {#lock-template-in-the-email-editor}

1. Seleccione el correo electrónico que desee bloquear y haga clic en **Editar borrador**.

   ![](assets/5.png)

1. En el editor de correo electrónico, haga clic en **Configuración de correo electrónico**.

   ![](assets/6.png)

1. Marque **Publicar en Marketingto Sales Insight** si no está marcado. Ahora puede desactivar **Permitir que el usuario de CRM edite el correo electrónico** para bloquear la plantilla. Haga clic en **Guardar**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >De forma predeterminada, esta casilla está activada y los usuarios de CRM pueden editar correos electrónicos.
