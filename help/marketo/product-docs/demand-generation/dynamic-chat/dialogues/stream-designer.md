---
description: 'Diseñador de secuencias: Documentos de Marketo: Documentación del producto'
title: Diseñador de secuencias
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: adf3a9f156ec5ed823a0647affb87f6c0686d35f
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# Diseñador de secuencias {#stream-designer}

Hay _many_ combinaciones de flujo que puede crear. Este artículo contiene un ejemplo en el que el especialista en marketing pregunta al visitante del sitio si tiene alguna pregunta sobre el producto. Si es así, el visitante puede programar una cita. En caso negativo, se da al visitante la opción de unirse a una lista de correo para correspondencia futura. El objetivo es programar una cita o recopilar el correo electrónico del visitante.

## Tarjetas de Diseñador de secuencias {#stream-designer-cards}

El diseñador de secuencias contiene varias tarjetas que puede agregar para dar forma a la conversación de chat.

<table>
 <tr>
  <td><strong>Mensaje</strong></td>
  <td>Utilícelo cuando desee realizar una instrucción sin necesidad de respuesta (por ejemplo: "¡Hola! Todos los artículos tienen hoy un 25% de descuento con el código SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Pregunta</strong></td>
  <td>Utilícelo cuando desee hacer una pregunta de opción múltiple, de la que proporcione las respuestas disponibles (por ejemplo: ¿Qué tipo de vehículo le interesa? Respuestas = SUV, Compacta, Camión, etc.).</td>
 </tr>
 <tr>
  <td><strong>Captura de información</strong></td>
  <td>Utilícelo cuando desee recopilar información. Los tres campos entre los que elegir son Dirección de correo electrónico, Número de teléfono y Texto (que permite al visitante escribir su propio mensaje).</td>
 </tr>
 <tr>
  <td><strong>Programador de citas</strong></td>
  <td>Proporciona al visitante un calendario de fechas disponibles para programar un seguimiento. La disponibilidad del calendario refleja <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">el siguiente agente en línea</a>.</td>
 </tr>
 <tr>
  <td><strong>Objetivo</strong></td>
  <td>Esta es la única tarjeta que los visitantes no verán. Depende de usted determinar en qué momento se logra un objetivo dentro del chat específico (por ejemplo: si su objetivo es recopilar el correo electrónico del visitante, coloque la tarjeta Goal inmediatamente después de Captura de información en el flujo).</td>
 </tr>
</table>

## Creación de un flujo {#create-a-stream}

1. Después de [crear el cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}, haga clic en el botón **Diseñador de secuencias** pestaña .

   ![](assets/create-a-stream-1.png)

1. Arrastre y suelte la tarjeta Pregunta .

   ![](assets/create-a-stream-2.png)

1. En Respuesta de bots de chat, responda a su pregunta como le gustaría.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >El valor de Poke se establece en activado de forma predeterminada, lo que muestra la pregunta de apertura junto al icono de chat sin que el visitante tenga que hacer clic en él para verlo.

1. Introduzca sus respuestas de usuario y haga clic en **Guardar**.

   ![](assets/create-a-stream-4.png)

1. Para &quot;Sí&quot; queremos programar una cita, así que debajo de esa opción, arrastre la tarjeta Programador de citas.

   ![](assets/create-a-stream-5.png)

1. En la columna de la derecha, haga clic en **Guardar**.

   ![](assets/create-a-stream-6.png)

1. Dado que es un objetivo, arrastre la tarjeta Goal debajo del Programador de citas.

   ![](assets/create-a-stream-7.png)

1. Asigne un nombre al objetivo (o elija uno existente) y haga clic en **Guardar**.

   ![](assets/create-a-stream-8.png)

1. Para &quot;No&quot; queremos ver si se unirán a la lista de correo, así que debajo de esa opción, arrastre sobre otra tarjeta de Pregunta.

   ![](assets/create-a-stream-9.png)

1. Introduzca su respuesta y añada opciones de respuesta para el visitante. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Para agregar más respuestas, haga clic en **Agregar respuesta**.

1. Debajo de la respuesta &quot;Sí&quot;, arrastre la tarjeta Captura de información para poder recopilar el correo electrónico del visitante.

   ![](assets/create-a-stream-11.png)

1. Haga clic en el **Tipo** y seleccione **Correo electrónico**.

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

1. Introduzca el mensaje y haga clic en **Guardar**.

   ![](assets/create-a-stream-17.png)

1. Seleccione el **Vista previa** alterne para obtener una vista previa del cuadro de diálogo.

   ![](assets/create-a-stream-18.png)

1. Cuando esté listo para activar el cuadro de diálogo, haga clic en **Publicación**.

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>Antes de hacer clic en Publicar, recuerde asegurarse de que ha [ha introducido las direcciones URL de destino](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target=&quot;_blank&quot;}.

>[!MORELIKETHIS]
>
>* [Crear un cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Criterios de audiencia](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [Informes](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

