---
unique-page-id: 2360245
description: 'Eliminar el texto de cancelación de suscripción de la sección de correo electrónico del administrador: Documentos de Marketo: documentación del producto'
title: Eliminar el texto de cancelación de suscripción de la sección Correo electrónico del administrador
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Eliminar el texto de cancelación de suscripción de la sección Correo electrónico del administrador {#remove-unsubscribe-text-from-the-admin-email-section}

La única razón por la que debería eliminar por completo el contenido de cancelación de suscripción del área &quot;Administración > Correo electrónico&quot; es si decide crear el vínculo de cancelación de suscripción en las propias plantillas de correo electrónico. El cuadro de texto tiene una validación que no permite guardar sin contenido. Puede evitarlo añadiendo un pequeño comentario HTML. El comentario del HTML no se mostrará en el cliente de correo electrónico, ya que está procesando el correo electrónico en HTML y los comentarios se omiten. Así es como hacerlo.

1. Vaya a la **Administrador** .

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Haga clic en **Correo electrónico**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Seleccione todo el texto y presione la tecla **Eliminar** clave.

   >[!CAUTION]
   >
   >Antes de eliminarlo, copie o pegue esto en un documento de texto como copia de seguridad.

1. Escriba en `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Haga clic en **Guardar cambios**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Para la variable **Cancelar suscripción de texto** tiene que añadir un solo carácter. Utilice un guión o un punto.
