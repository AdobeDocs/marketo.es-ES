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

La única razón por la que debería eliminar por completo el contenido de cancelación de suscripción de la **[!UICONTROL Administrador]** > **[!UICONTROL Correo electrónico]** es si elige incorporar el vínculo &quot;Cancelar la suscripción&quot; en las propias plantillas de correo electrónico. El cuadro de texto tiene una validación que no permite guardar sin contenido. Puede evitar esto añadiendo un pequeño comentario del HTML. El comentario del HTML no aparecerá en el cliente de correo electrónico, ya que está procesando el correo electrónico en HTML y los comentarios se omiten. Así es como se hace.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Clic **[!UICONTROL Correo electrónico]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Seleccione todo el texto y pulse la tecla **[!UICONTROL Eliminar]** clave.

   >[!CAUTION]
   >
   >Antes de eliminarlo, copie/pegue esto en un documento de texto como copia de seguridad.

1. Escribir en `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Clic **[!UICONTROL Guardar cambios]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Para el **Cancelar suscripción a texto** tiene que añadir un solo carácter. Utilice un guión o un punto.
