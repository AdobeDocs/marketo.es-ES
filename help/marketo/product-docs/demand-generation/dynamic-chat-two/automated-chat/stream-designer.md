---
description: Diseñador de transmisiones - Documentos de Marketo - Documentación del producto
title: Diseñador de flujo
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: b4ba55769034e8fb8a7878f52e21bd08e073fa8c
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 2%

---

# Diseñador de flujo {#stream-designer}

No hay _muchos_ combinaciones de flujo posibles. Este artículo contiene un ejemplo en el que el experto en marketing pregunta al visitante del sitio si tiene alguna pregunta sobre el producto. Si es así, el visitante puede programar una cita. Si no es así, el visitante tiene la opción de unirse a una lista de correo para correspondencia futura. También se les ofrece un PDF gratis. El objetivo final es programar una cita o recopilar el correo electrónico del visitante.

>[!PREREQUISITES]
>
>Para poder usar la tarjeta de documento, primero debe [configúrelo.](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"} en su cuenta de Adobe.

## Tarjetas de diseñador de Stream {#stream-designer-cards}

El diseñador de secuencias contiene varias tarjetas que puede agregar para dar forma a la conversación de chat.

<table>
 <tr>
  <td><strong>Mensaje</strong></td>
  <td>Utilícelo cuando desee realizar una declaración sin necesidad de respuesta (por ejemplo: "¡Hola! Todos los artículos tienen un 25% de descuento hoy con el código SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Pregunta</strong></td>
  <td>Úselo cuando quiera hacer una pregunta de opción múltiple, de la que proporcione las respuestas disponibles (por ejemplo: ¿Qué tipo de vehículo le interesa? Respuestas = SUV, Compact, Truck, etc.).</td>
 </tr>
 <tr>
  <td><strong>Documento</strong></td>
  <td>Permite incrustar documentos del PDF en los cuadros de diálogo y realizar un seguimiento de la actividad de participación de los visitantes en los documentos (cuántas páginas se vieron, si se descargó el documento o los términos de búsqueda utilizados).</td>
 </tr>
 <tr>
  <td><strong>Captura de información</strong></td>
  <td>Utilícelo cuando desee recopilar información. Los tres campos para elegir son Dirección de correo electrónico, Número de teléfono y Texto (que permite al visitante escribir su propio mensaje).</td>
 </tr>
 <tr>
  <td><strong>Planificador de citas</strong></td>
  <td>Proporciona al visitante un calendario de fechas disponibles para programar un seguimiento. La disponibilidad del calendario refleja <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">el siguiente agente en la línea</a>.</td>
 </tr>
 <tr>
  <td><strong>Objetivo</strong></td>
  <td>Esta es la única tarjeta que los visitantes no verán. Le corresponde a usted determinar en qué momento se logra un objetivo dentro del chat específico (por ejemplo, si su objetivo es recopilar el correo electrónico del visitante, coloque la tarjeta Objetivo inmediatamente después de la captura de información en el flujo).</td>
 </tr>
 <tr>
  <td><strong>Acción</strong></td>
  <td>De forma similar a los campos ocultos en un formulario, con la tarjeta de acción puede rellenar cualquier atributo de posible cliente o compañía con valores implícitos que desee capturar con un registro de posible cliente. Puede añadir la tarjeta de acción en cualquier momento de la conversación y actualizar los atributos respectivos con un valor o tokens nativos que rellenen automáticamente el valor respectivo.</td>
 </tr>
 <tr>
  <td><strong>Chat en directo</strong></td>
  <td>Utilice la tarjeta de chat en vivo cuando desee que los visitantes chateen con un agente en vivo.
  <li>La tarjeta de chat en vivo debe ser la última tarjeta de la sucursal</li>
  <li>Los visitantes se dirigirán a un agente en cuanto lleguen a esta tarjeta en el flujo, por lo que se recomienda preceder esta tarjeta con una tarjeta de preguntas que pregunte a los visitantes si desean chatear con un agente en directo</li></td>
 </tr>
</table>

## Iconos del diseñador de secuencias {#stream-designer-icons}

En la parte superior derecha del Diseñador de secuencias, verá un puñado de iconos. Esto es lo que hacen.

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>Agrega una cuadrícula al fondo para aquellos que prefieren esa vista</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>Aumenta el tamaño, creando tarjetas más grandes</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>Aleja, crea tarjetas más pequeñas</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>Abre una ventana para que usted pruebe su chat (presione el mismo botón para cerrar)</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>Organiza todas las tarjetas del flujo</td>
 </tr>
</table>

## Crear una secuencia {#create-a-stream}

1. Después de que... [ha creado su cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}, haga clic en **Diseñador de secuencias** pestaña.

   ![](assets/stream-designer-6.png)

1. Arrastre y suelte la tarjeta Pregunta.

   ![](assets/stream-designer-7.png)

1. En Respuesta del bot de chat, escriba su pregunta como desee.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Puede personalizar la experiencia para los visitantes de chat conocidos mediante tokens (por ejemplo: Hello `{{lead.leadFirstName:""}}`). Simplemente haga clic en el icono de llave a la derecha y realice su selección. Agregue un valor predeterminado entre las comillas si desea que los visitantes anónimos vean algo genérico (por ejemplo: Hello `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Poke está configurado como on de forma predeterminada, lo que muestra la pregunta de apertura junto al icono de chat sin que el visitante tenga que hacer clic en él para verlo. El Poke solo está disponible en la primera carta de la conversación.

1. Introduzca sus respuestas de usuario y haga clic en **Guardar**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**Editar valores almacenados** es un paso opcional para aquellos que deseen almacenar un valor diferente en la base de datos de lo que se muestra a los visitantes en el bot de chat para los atributos asignados en la tarjeta de pregunta (por ejemplo: el visitante ve &quot;Optimización del motor de búsqueda&quot;, se almacena ese valor como &quot;SEO&quot;).

1. Para &quot;Sí&quot; queremos programar una cita, así que debajo de esa opción arrastre sobre la tarjeta Programador de citas.

   ![](assets/stream-designer-10.png)

1. En la columna de la derecha, haga clic en **Guardar**.

   ![](assets/stream-designer-11.png)

1. Como ese es un objetivo, arrastre la tarjeta Objetivo debajo del Programador de citas.

   ![](assets/stream-designer-12.png)

1. Asigne un nombre a la meta (o elija una existente) y haga clic en **Guardar**.

   ![](assets/stream-designer-13.png)

1. Para &quot;No&quot; queremos ver si se unen a la lista de correo, así que debajo de esa opción arrastre sobre otra tarjeta de Pregunta.

   ![](assets/stream-designer-14.png)

1. Introduzca su respuesta y añada opciones de respuesta para el visitante. Clic **Guardar** cuando termine.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Para agregar más respuestas, haga clic en **Agregar respuesta**.

1. Debajo de la respuesta &quot;Sí&quot;, arrastre sobre la tarjeta de captura de información para poder recopilar el correo electrónico del visitante.

   ![](assets/stream-designer-16.png)

1. Haga clic en **Tipo** y seleccione. **Correo electrónico**.

   ![](assets/stream-designer-17.png)

1. Introduzca un mensaje de bot de chat y un marcador de posición. Asegúrese de que el atributo esté asignado al campo correspondiente en Marketo y haga clic en **Guardar**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>Tipo</strong></td>
     <td>El tipo de información que desea capturar: teléfono, texto, correo electrónico.</td>
    </tr>
    <tr>
     <td><strong>Mensaje de chatbot</strong></td>
     <td>El mensaje que ve el visitante pidiéndole que proporcione la información.</td>
    </tr>
    <tr>
     <td><strong>Marcador de posición</strong></td>
     <td>Texto de muestra que ayuda al visitante a ver qué debe introducir.</td>
    </tr>
    <tr>
     <td><strong>Asignar respuesta al atributo</strong></td>
     <td>Permite sincronizar la respuesta del visitante con el campo correspondiente de su registro de persona en su suscripción a Marketo.</td>
    </tr>
   </table>

1. Como recopilar su correo electrónico es una meta, arrastre la tarjeta Objetivo debajo de Captura de información.

   ![](assets/stream-designer-19.png)

1. Asigne un nombre a la meta (o elija una existente) y haga clic en **Guardar**.

   ![](assets/stream-designer-20.png)

1. Recuerde agregar una respuesta si dice &quot;No&quot;. Una opción es arrastrar una tarjeta de mensaje a continuación y decir &quot;gracias de todos modos&quot;. Pero en este ejemplo, les proporcionaremos un documento de PDF gratuito en su lugar.

   ![](assets/stream-designer-21.png)

1. En este ejemplo crearemos un nuevo documento. Asigne un nombre, introduzca la dirección URL del PDF que ya ha alojado y haga clic en **Guardar**.

   ![](assets/stream-designer-22.png)

1. Seleccione el **Previsualizar** para previsualizar el cuadro de diálogo.

   ![](assets/stream-designer-23.png)

1. Cuando esté listo para activar el cuadro de diálogo, haga clic en **Publish**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Antes de hacer clic en Publicar, recuerde asegurarse de que ha [ha introducido sus direcciones URL de destino](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Crear un cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [Criterios de audiencia](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target="_blank"}
>* Informes de [ ](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
>* [Uso de la tarjeta de documento](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"}

