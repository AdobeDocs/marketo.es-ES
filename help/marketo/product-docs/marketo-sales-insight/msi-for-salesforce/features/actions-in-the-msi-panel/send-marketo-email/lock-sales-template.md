---
unique-page-id: 12981050
description: Bloquear plantilla de ventas - Documentos de Marketo - Documentación del producto
title: Bloquear plantilla de ventas
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Bloquear plantilla de ventas {#lock-sales-template}

Para evitar que los usuarios de CRM editen plantillas de ventas, los administradores pueden habilitar la posibilidad de bloquear plantillas, lo que permite a los usuarios bloquear plantillas individualmente desde el editor de correo electrónico.

>[!CAUTION]
>
>Esta función solo funciona para Salesforce y no es compatible con Microsoft Dynamics u otros CRM. Las plantillas a las que se accede desde los complementos de Outlook o Gmail no se bloquearán, ya que el editor no está controlado por Marketo.

## Activar Bloquear plantilla {#enable-lock-template}

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Vaya a **Administrador** y haga clic en **Perspectiva de ventas**.

   ![](assets/1.png)

1. En **Configuración**, haga clic en **Editar**.

   ![](assets/2.png)

1. Marque **Habilitar la capacidad de bloquear plantillas**. Haga clic en **Guardar**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>De forma predeterminada, esta casilla está marcada y la capacidad de bloquear plantillas está habilitada. Al desmarcarlo, se deshabilitará la función de plantilla de bloqueo en el editor de correo electrónico.

>[!NOTE]
>
>Si se cambia esta configuración como administrador, **not** afectar retroactivamente a las plantillas existentes; es decir, no los bloqueará automáticamente.

## Bloquear plantilla en el editor de correo electrónico {#lock-template-in-the-email-editor}

1. Seleccione el correo electrónico que desea bloquear y haga clic en **Editar borrador**.

   ![](assets/5.png)

1. En el editor de correo electrónico, haga clic en **Configuración de correo electrónico**.

   ![](assets/6.png)

1. Marque **Publicar en Marketo Sales Insight** si no está marcada. Ahora puede desactivar **Permitir que el usuario de CRM edite el correo electrónico** para bloquear la plantilla. Haga clic en **Guardar**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >De forma predeterminada, esta casilla está marcada y los usuarios de CRM pueden editar correos electrónicos.
