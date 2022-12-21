---
unique-page-id: 1900577
description: 'Creación de un token de script de correo electrónico: documentos de Marketo: documentación del producto'
title: Creación de un token de script de correo electrónico
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Creación de un token de script de correo electrónico {#create-an-email-script-token}

Para desarrolladores avanzados, puede usar [Secuencias de comandos de Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) en sus correos electrónicos. Así es como hacerlo.

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Busque y seleccione cualquier programa (Evento, Predeterminado, Participación, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. En el **Mis tokens** , arrastre **Script de correo electrónico** token.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Asigne un nombre al token de script de correo electrónico y **haga clic para editar** su contenido.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilice el árbol de la derecha para arrastrar **Persona, oportunidad** o **Objeto personalizado** tokens.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Al acceder a una matriz (oportunidad u objeto personalizado), está limitado a los últimos 10 elementos asociados a la persona.

1. Observe que el token se activa o marca después de arrastrarlo al editor de secuencias de comandos.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Si está escribiendo en tokens de forma libre, asegúrese de comprobar/activar todos los tokens correspondientes en el árbol; de lo contrario, se tratarán como texto sin formato y no funcionarán.

1. Escriba el script en Velocity. Estos son algunos recursos útiles:

   * [Documentación de secuencias de comandos de correo electrónico para desarrolladores de Marketo](https://developers.marketo.com/email-scripting/)
   * [Guía del usuario de Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guía de referencia de Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Herramientas de Velocity Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Una vez completada la secuencia de comandos, haga clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Haga clic en **Guardar** una vez más.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ahora puede utilizar este token en sus correos electrónicos. Ejecutará la secuencia de comandos cada vez que se envíe un correo electrónico.

>[!MORELIKETHIS]
>
>[Añadir un token de script de correo electrónico al correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
