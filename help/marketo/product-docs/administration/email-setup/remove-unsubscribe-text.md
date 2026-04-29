---
unique-page-id: 2360245
description: Elimine el contenido predeterminado para cancelar la suscripción del correo electrónico del administrador mediante un comentario de HTML al crear el vínculo en las plantillas.
title: Quitar texto de cancelación de suscripción
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 9c4f0d0a43d3ef06132d827b605b9e42de712e22
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 7%

---

# Quitar texto de cancelación de suscripción {#remove-unsubscribe-text}

La única razón por la que deberías eliminar por completo el contenido de cancelación de suscripción del área de **[!UICONTROL Administración]** > **[!UICONTROL Correo electrónico]** es si eliges crear el vínculo de cancelación de suscripción en las propias plantillas de correo electrónico. El cuadro de texto tiene una validación que no permite guardar sin contenido. Puede evitar esto añadiendo un pequeño comentario en HTML. El comentario de HTML no aparecerá en el cliente de correo electrónico, porque está procesando el correo electrónico en HTML y los comentarios se omiten.

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
