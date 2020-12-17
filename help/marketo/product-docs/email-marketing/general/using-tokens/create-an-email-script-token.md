---
unique-page-id: 1900577
description: Creación de un token de script de correo electrónico - Documentos de marketing - Documentación del producto
title: Creación de un token de script de correo electrónico
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# Crear un token de script de correo electrónico {#create-an-email-script-token}

Para desarrolladores avanzados, puede utilizar [scripts de Velocity](http://velocity.apache.org/engine/1.7/user-guide.html) en sus correos electrónicos. Así es como hacerlo.

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Busque y seleccione cualquier programa (Evento, Predeterminado o Participación, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. En la ficha **Mis tokens**, arrastre un distintivo **Script de correo electrónico**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Asigne un nombre al token de script de correo electrónico y **haga clic para editar** su contenido.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilice el árbol de la derecha para arrastrar los tokens **Persona, Oportunidad** o **Objeto personalizado**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Al acceder a una matriz (oportunidad u objeto personalizado), se limita a los 10 elementos más recientes asociados a la persona.

1. Observe que el token se marca o se activa después de arrastrarlo al editor de secuencias de comandos.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Si está escribiendo tokens de forma libre, asegúrese de comprobar/activar todos los tokens correspondientes en el árbol o se tratarán como texto sin formato y no funcionarán.

1. Escriba el script en Velocity. Estos son algunos recursos útiles:

   * [Documentación de secuencias de comandos de correo electrónico para desarrolladores de Marketing to](http://developers.marketo.com/email-scripting/)
   * [Guía del usuario de Velocity](http://velocity.apache.org/engine/devel/user-guide.html)
   * [Guía de referencia de Velocity](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Una vez completada la secuencia de comandos, haga clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Haga clic en **Guardar** una vez más.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ahora puede usar este token en sus correos electrónicos. Ejecutará la secuencia de comandos cada vez que se envíe un correo electrónico.

>[!MORELIKETHIS]
>
>* [Añadir un token de script de correo electrónico a su correo electrónico](add-an-email-script-token-to-your-email.md)

>



