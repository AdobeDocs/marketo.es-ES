---
unique-page-id: 1900577
description: 'Creación de un token de script de correo electrónico: documentos de Marketo: documentación del producto'
title: Crear un token de script de correo electrónico
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Crear un token de script de correo electrónico {#create-an-email-script-token}

Para desarrolladores avanzados, puedes usar [Scripts de Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) en tus correos electrónicos. Así es como se hace.

1. Vaya a **Actividades de marketing**.

   ![](assets/ma.png)

1. Busque y seleccione cualquier programa (Evento, Predeterminado o Participación, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. En la ficha **Mis tokens**, arrastre un token de **correo electrónico**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Asigne un nombre al token del script de correo electrónico y **haga clic para editar** su contenido.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilice el árbol de la derecha para arrastrar **tokens de persona, oportunidad** u **objeto personalizado**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Al acceder a una matriz (oportunidad u objeto personalizado), se limita a los 10 elementos asociados más recientemente a la persona.

1. Observe que el token se activa o se marca después de arrastrarlo al editor de scripts.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Si está escribiendo tokens de forma libre, asegúrese de comprobar/activar todos los tokens correspondientes en el árbol o se tratarán como texto sin formato y no funcionarán.

1. Escriba el script en Velocity. Estos son algunos recursos útiles:

   * [Documentación de scripts de correo electrónico para desarrolladores de Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Guía del usuario de Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guía de referencia de Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Herramientas Javadoc De Velocity](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Una vez completado el script, haz clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Haz clic en **Guardar** una vez más.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Ahora puede utilizar este token en sus correos electrónicos. Ejecutará el script cada vez que se envíe un correo electrónico.

>[!MORELIKETHIS]
>
>[Agregue un token de script de correo electrónico a su correo electrónico](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
