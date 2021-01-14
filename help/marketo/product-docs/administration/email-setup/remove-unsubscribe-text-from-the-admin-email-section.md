---
unique-page-id: 2360245
description: Eliminar el texto de cancelación de suscripción de la sección Correo electrónico del administrador - Documentos de marketing - Documentación del producto
title: Eliminar el texto de cancelación de suscripción de la sección Correo electrónico del administrador
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Eliminar el texto de cancelación de suscripción de la sección de correo electrónico del administrador {#remove-unsubscribe-text-from-the-admin-email-section}

La única razón por la que debería eliminar por completo el contenido de cancelación de suscripción del área &quot;Administración > Correo electrónico&quot; es si decide crear el vínculo de cancelación de suscripción en las plantillas de correo electrónico. El cuadro de texto tiene una validación que no le permite guardar sin contenido. Puede evitarlo agregando un pequeño comentario HTML. El comentario HTML no se mostrará en el cliente de correo electrónico porque está representando el correo electrónico en HTML y los comentarios se omiten. Así es como hacerlo.

1. Vaya a **Administración** y haga clic en **Correo electrónico**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Seleccione todo el texto y pulse la tecla **Eliminar**.

   >[!CAUTION]
   >
   >Antes de eliminar, copie/pegue esto en un documento de texto como copia de seguridad.

1. Escriba `<!--This is a comment -->`.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Haga clic en **Guardar cambios**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Para el **Cancelar suscripción de texto** debe agregar un solo carácter. Utilice un guión o un punto.
