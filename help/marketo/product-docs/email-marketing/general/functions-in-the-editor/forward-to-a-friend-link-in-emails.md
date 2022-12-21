---
unique-page-id: 1900581
description: 'Reenviar a un vínculo de amigo en correos electrónicos: Marketo Docs: documentación del producto'
title: Enviar a un vínculo de amigo en correos electrónicos
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Enviar a un vínculo de amigo en correos electrónicos {#forward-to-a-friend-link-in-emails}

Añadir el vínculo &quot;Reenviar a amigo&quot; a sus correos electrónicos le permite hacer un seguimiento de las personas que han recibido un correo electrónico reenviado a través de este vínculo y añadirlo automáticamente como una nueva persona si no están ya en la base de datos.

Por ejemplo, supongamos que Keith utiliza el vínculo &quot;Reenviar a amigo&quot; para reenviar el correo electrónico a una persona desconocida, Mark. Mark se añade automáticamente como una persona nueva, se le asigna su propia cookie y cualquier actividad de correo electrónico y web está vinculada a él. Sin embargo, si Keith utiliza el botón de reenvío en su cliente de correo electrónico, Mark recibe una cookie incorrecta como Keith y su actividad se registra como de Keith.

## Agregar el vínculo a una plantilla de correo electrónico {#add-the-link-to-an-email-template}

1. Vaya a la **Design Studio**.

   ![](assets/one-8.png)

1. Busque y seleccione la plantilla de correo electrónico a la que desea agregar el vínculo. Haga clic en **Editar borrador**.

   ![](assets/two-7.png)

1. Pegue el siguiente código de HTML donde desee que aparezca el vínculo &quot;Reenviar a amigo&quot; (si necesita ayuda con esta parte, consulte con su desarrollador web):

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Puede agregar estilo al vínculo para que tenga un aspecto más agradable. Por ejemplo:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >No se recomienda utilizar el estilo **posición:relativo** en la plantilla de correo electrónico. Puede crear problemas con la posición y visualización del cuadro &quot;De reenvío a amigo&quot;.

1. Haga clic en **Previsualizar borrador** para asegurarse de que la plantilla tenga el aspecto que desea.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Recuerde aprobar el borrador de la plantilla para aplicar los cambios.

   Ahora, todos los correos electrónicos que utilicen esa plantilla tendrán el vínculo &quot;Reenviar a amigo&quot;. Cuando el destinatario del correo electrónico haga clic en él, se le llevará a una versión web del correo electrónico con el cuadro &quot;Reenviar a un amigo&quot;:

   ![](assets/f2afbox.png)

## Añadir el vínculo a un correo electrónico individual {#add-the-link-to-an-individual-email}

También puede añadir el vínculo &quot;Reenviar a amigo&quot; directamente a un correo electrónico.

1. Abra el correo electrónico en el que desee incluir el vínculo y haga doble clic en el área editable.

   ![](assets/five-4.png)

1. Sitúe el cursor donde desee que aparezca el vínculo y haga clic en el botón **Insertar token** botón.

   ![](assets/six-2.png)

1. Seleccione el **`{{system.forwardToFriendLink}}`** token.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Este token es la URL de la versión web del correo electrónico con un cuadro &quot;Reenviar a amigo&quot;.

1. Escriba el texto que desea que muestre el vínculo (por ejemplo, &quot;Reenviar a un amigo&quot;).

   ![](assets/seven-1.png)

1. Corte la variable **`{{system.forwardToFriendLink}}`** token utilizando Ctrl+X (Windows) o Cmd+X (Mac). Resalte &quot;Enviar a un amigo&quot; y haga clic en el botón **Insertar/Editar vínculo** botón.

   ![](assets/eight-1.png)

1. Pegue el **`{{system.forwardToFriendLink}}`** en el **URL** en el cuadro con Ctrl/Cmd+V y, a continuación, haga clic en **Insertar**.

   ![](assets/nine.png)

1. Guarde la edición y previsualice el nuevo vínculo.

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Las personas nuevas que se agregan recibiendo un correo electrónico de &quot;Reenviar a un amigo&quot; se cancelan de forma predeterminada a los correos electrónicos de marketing.

## Ver actividad de reenvío {#view-forwarding-activity}

Puede ver quién reenvió y recibió los correos electrónicos en el registro de actividades de la persona.

1. Vaya a la **`Database`**.

   ![](assets/db.png)

1. Haga doble clic en la persona para la que desee ver la actividad.

   ![](assets/fourteen.png)

1. Vaya a la **Registro de actividades** pestaña . Hacer doble clic **Correo electrónico de reenvío a amigo recibido** o **Enviar correo electrónico de reenvío a amigo** para ver los detalles.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definición**
   >
   >En el caso de Recibido reenvío a correo electrónico de amigo, el ID de persona es la persona que reenvió el correo electrónico.
   >
   >Para Enviar a correo electrónico de amigo, el ID de persona es la persona que recibió el correo electrónico.

   ![](assets/sixteen.png)

1. Para ver una persona por ID, copie y pegue el **ID de persona** al final de la dirección URL (el principio de dicha dirección URL dependerá de la instancia de Marketo):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >Haremos que el **ID de persona** Haga clic en y vincule directamente a la persona en un parche próximo.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Si el amigo que recibe el reenvío es una persona desconocida, se crea una nueva persona con la marca &quot;De reenviar a un amigo&quot; como la de la persona **Fuente**.
   >Si el correo electrónico es un recurso local de un programa, el programa se marca como el **Programa de adquisición**.

## Déclencheur o filtro mediante la actividad de reenvío {#trigger-or-filter-using-forwarding-activity}

Hay seis déclencheur/filtros que puede utilizar para las acciones de flujo de déclencheur o para filtrar personas mediante la actividad &quot;Enviar a amigo&quot; enviada y recibida.

En la lista inteligente de una campaña inteligente, si busca &quot;adelante&quot;, encontrará los déclencheur y filtros disponibles.

![](assets/nineteen.png)

## Probar el envío a un amigo {#test-forward-to-friend}

Para probar &quot;Reenviar a un amigo&quot;, envíe un correo electrónico con el enlace de reenvío. Asegúrese de enviarlo a través de la variable **Enviar correo electrónico** paso de flujo, *not* hasta **Enviar mensaje de prueba**.
