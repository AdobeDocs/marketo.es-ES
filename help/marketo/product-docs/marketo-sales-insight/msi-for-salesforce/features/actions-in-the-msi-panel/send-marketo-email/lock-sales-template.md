---
unique-page-id: 12981050
description: Bloquear plantilla de ventas - Documentos de Marketo - Documentación del producto
title: Bloquear plantilla de ventas
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Bloquear plantilla de ventas {#lock-sales-template}

Para evitar que los usuarios de CRM editen plantillas de ventas, los administradores pueden habilitar la capacidad de bloquear plantillas, lo que permite a los usuarios bloquear plantillas individualmente desde el editor de correo electrónico.

>[!CAUTION]
>
>Esta función solo funciona para Salesforce y no es compatible con Microsoft Dynamics u otros CRM. Las plantillas a las que se accede desde los complementos de Outlook o Gmail no se bloquearán, ya que el editor no está controlado por Marketo.

## Habilitar plantilla de bloqueo {#enable-lock-template}

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Ir a **Administrador**, luego haga clic en **Perspectiva de ventas**.

   ![](assets/1.png)

1. En **Configuración**, haga clic en **Editar**.

   ![](assets/2.png)

1. Marque **Habilitar la capacidad de bloquear plantillas**. Clic **Guardar**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>De forma predeterminada, esta casilla está activada y la capacidad de bloquear plantillas está activada. Si la desmarca, se desactivará la función de plantilla de bloqueo en el editor de correo electrónico.

>[!NOTE]
>
>Si cambia esta configuración como administrador, **no** afectar de forma retroactiva a las plantillas existentes; es decir, no las bloqueará automáticamente.

## Bloquear plantilla en el editor de correo electrónico {#lock-template-in-the-email-editor}

1. Seleccione el correo electrónico que desea bloquear y haga clic en **Editar borrador**.

   ![](assets/5.png)

1. En el editor de correo electrónico, haga clic en **Configuración de correo electrónico**.

   ![](assets/6.png)

1. Marque **Publicar en Marketo Sales Insight** si aún no está marcada. Ahora puede desmarcar **Permitir al usuario de CRM editar el correo electrónico** para bloquear la plantilla. Clic **Guardar**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >De forma predeterminada, esta casilla está marcada y los usuarios de CRM pueden editar correos electrónicos.
