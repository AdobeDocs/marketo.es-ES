---
unique-page-id: 2360245
description: 'Eliminar el texto de cancelación de suscripción de la sección de correo electrónico del administrador: Documentos de Marketo: documentación del producto'
title: Eliminar el texto de cancelación de suscripción de la sección Correo electrónico del administrador
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Eliminar el texto de cancelación de suscripción de la sección de correo electrónico del administrador {#remove-unsubscribe-text-from-the-admin-email-section}

La única razón por la que debería eliminar por completo el contenido de cancelación de suscripción del área &quot;Administración > Correo electrónico&quot; es si decide crear el vínculo de cancelación de suscripción en las propias plantillas de correo electrónico. El cuadro de texto tiene una validación que no permite guardar sin contenido. Puede evitarlo añadiendo un pequeño comentario HTML. El comentario HTML no se mostrará en el cliente de correo electrónico, ya que está procesando el correo electrónico en HTML y los comentarios se omiten. Así es como hacerlo.

1. Vaya a **Admin** y haga clic en **Email**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Seleccione todo el texto y pulse la tecla **Delete**.

   >[!CAUTION]
   >
   >Antes de eliminarlo, copie o pegue esto en un documento de texto como copia de seguridad.

1. Escriba `<!--This is a comment -->`.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Haga clic en **Guardar cambios**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Para el **Unsubscribe Text** debe añadir un solo carácter. Utilice un guión o un punto.
