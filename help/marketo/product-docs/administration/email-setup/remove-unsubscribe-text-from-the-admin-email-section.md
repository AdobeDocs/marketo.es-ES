---
unique-page-id: 2360245
description: Eliminar el texto de cancelación de suscripción de la sección de correo electrónico del administrador - Documentos de Marketo - Documentación del producto
title: Eliminar texto de cancelación de suscripción de la sección Correo electrónico del administrador
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Elimine el texto de cancelación de suscripción de la sección Administración > Correo electrónico {#remove-unsubscribe-text-from-the-admin-email-section}

La única razón por la que deberías eliminar por completo el contenido de cancelación de suscripción del área de **[!UICONTROL Administración]** > **[!UICONTROL Correo electrónico]** es si eliges crear el vínculo de cancelación de suscripción en las propias plantillas de correo electrónico. El cuadro de texto tiene una validación que no permite guardar sin contenido. Puede evitar esto añadiendo un pequeño comentario del HTML. El comentario del HTML no aparecerá en el cliente de correo electrónico, ya que está procesando el correo electrónico en HTML y los comentarios se omiten. Así es como se hace.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Haga clic en **[!UICONTROL Correo electrónico]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Seleccione todo el texto y presione la tecla **[!UICONTROL Delete]**.

   >[!CAUTION]
   >
   >Antes de eliminarlo, copie/pegue esto en un documento de texto como copia de seguridad.

1. Escriba `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Haga clic en **[!UICONTROL Guardar cambios]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Para el **texto para cancelar la suscripción**, debe agregar un solo carácter. Utilice un guión o un punto.
