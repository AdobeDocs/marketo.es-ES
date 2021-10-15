---
description: 'Creación de una emisión: Marketo Docs: Documentación del producto'
title: Creación de un flujo
hide: true
hidefromtoc: true
source-git-commit: 1434d2a1cbf5575cea60ccc0c655313003b1452c
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Creación de un flujo {#create-a-stream}

Puede crear _muchas_ combinaciones de flujo. A continuación se muestra un ejemplo en el que el especialista en marketing pregunta al visitante del sitio si tiene alguna pregunta sobre el producto. Si es así, el visitante puede programar una cita. En caso negativo, se da al visitante la opción de unirse a una lista de correo para correspondencia futura. El objetivo es programar una cita o recopilar el correo electrónico del visitante.

1. Después de [crear el cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue), haga clic en la pestaña **Diseñador de flujo**.

   ![](assets/create-a-stream-1.png)

1. Arrastre y suelte la tarjeta Pregunta .

   ![](assets/create-a-stream-2.png)

1. En Respuesta de bots de chat, responda a su pregunta como le gustaría.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >El valor de Poke se establece en activado de forma predeterminada, lo que muestra la pregunta de apertura junto al icono de chat sin que el visitante tenga que hacer clic en él para verlo.

1. Introduzca sus respuestas de usuario y haga clic en **Save**.

   ![](assets/create-a-stream-4.png)

1. Para &quot;Sí&quot; queremos programar una cita, así que debajo de esa opción, arrastre la tarjeta Programador de citas.

   ![](assets/create-a-stream-5.png)

1. En la columna de la derecha, haga clic en **Save**.

   ![](assets/create-a-stream-6.png)

1. Dado que es un objetivo, arrastre la tarjeta Goal debajo del Programador de citas.

   ![](assets/create-a-stream-7.png)

1. Asigne un nombre al objetivo (o elija uno existente) y haga clic en **Guardar**.

   ![](assets/create-a-stream-8.png)

1. Para &quot;No&quot; queremos ver si se unirán a la lista de correo, así que debajo de esa opción, arrastre sobre otra tarjeta de Pregunta.

   ![](assets/create-a-stream-9.png)

1. Introduzca su respuesta y añada opciones de respuesta para el visitante. Haga clic en **Guardar** cuando termine.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Para agregar más respuestas, haga clic en **Agregar respuesta**.

1. Debajo de la respuesta &quot;Sí&quot;, arrastre la tarjeta Captura de información para poder recopilar el correo electrónico del visitante.

   ![](assets/create-a-stream-11.png)

1. Haga clic en la lista desplegable **Type** y seleccione **Email**.

   ![](assets/create-a-stream-12.png)

1. Introduzca un mensaje de bots de chat y un marcador de posición. Asegúrese de que el atributo esté asignado al campo correspondiente en Marketo y haga clic en **Guardar**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Tipo</strong></td>
     <td>El tipo de información que desea capturar: Teléfono, Texto, Correo electrónico.</td>
    </tr>
    <tr>
     <td><strong>Mensaje de bots de chat</strong></td>
     <td>El mensaje que el visitante ve solicitándole que proporcione la información.</td>
    </tr>
    <tr>
     <td><strong>Marcador de posición</strong></td>
     <td>Texto de muestra que ayuda al visitante a ver qué introducir.</td>
    </tr>
    <tr>
     <td><strong>Asignar respuesta al atributo</strong></td>
     <td>Permite sincronizar la respuesta del visitante con el campo correspondiente de su registro de persona en la suscripción a Marketo.</td>
    </tr>
   </table>

1. Dado que la recopilación de su correo electrónico es un objetivo, arrastre la tarjeta de objetivo debajo de Captura de información.

   ![](assets/create-a-stream-14.png)

1. Asigne un nombre al objetivo (o elija uno existente) y haga clic en **Guardar**.

   ![](assets/create-a-stream-15.png)

1. Recuerde añadir una respuesta si dicen &quot;No&quot;. Arrastre una tarjeta Mensaje debajo de esa opción.

   ![](assets/create-a-stream-16.png)

1. Introduzca el mensaje y haga clic en **Save**.

   ![](assets/create-a-stream-17.png)

1. Cuando desee activar el cuadro de diálogo, haga clic en **Publicar**.

   ![](assets/create-a-stream-18.png)

>[!NOTE]
>
>Antes de hacer clic en Publicar, recuerde asegurarse de que ha [introducido las URL de destino](help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[Cuadros de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
