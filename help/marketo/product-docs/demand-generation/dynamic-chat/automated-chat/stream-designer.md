---
description: Stream Designer - Documentos de Marketo - Documentación del producto
title: Diseñador de flujo
feature: Dynamic Chat
exl-id: 310b1dff-dd93-48a6-85c2-64c58494ce48
source-git-commit: 11006e3244fd7a145a955dd08b669a897dae826b
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 2%

---

# Diseñador de flujo {#stream-designer}

Hay _muchas_ combinaciones de secuencias posibles. Este artículo contiene un ejemplo en el que el experto en marketing pregunta al visitante del sitio si tiene alguna pregunta sobre el producto. Si es así, el visitante puede programar una cita. Si no es así, el visitante tiene la opción de unirse a una lista de correo para correspondencia futura. También se les ofrece un PDF gratuito. El objetivo final es programar una cita o recopilar el correo electrónico del visitante.

>[!PREREQUISITES]
>
>Para poder usar la tarjeta de documento, primero debe [configurarla](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"} en su cuenta de Adobe.

## Transmitir tarjetas de Designer {#stream-designer-cards}

La Stream Designer contiene varias tarjetas que puedes agregar para dar forma a la conversación de chat.

<table>
 <tr>
  <td style="width:25%"><strong>Mensaje</strong></td>
  <td style="width:75%">Utilícelo cuando desee realizar una declaración sin necesidad de respuesta (por ejemplo: "¡Hola! Todos los artículos tienen un 25% de descuento hoy con el código SAVE25").
</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Pregunta</strong></td>
  <td>Úselo cuando quiera hacer una pregunta de opción múltiple, de la que proporcione las respuestas disponibles (por ejemplo: ¿Qué tipo de vehículo le interesa? Respuestas = SUV, Compact, Truck, etc.).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Documento</strong></td>
  <td>Permite incrustar documentos de PDF en cuadros de diálogo y realizar un seguimiento de la actividad de participación de los visitantes en los documentos (cuántas páginas se vieron, si se descargó el documento y/o los términos de búsqueda utilizados).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Captura de información</strong></td>
  <td>Utilícelo cuando desee recopilar información (por ejemplo, nombre, dirección de correo electrónico, cargo, etc.). Después de elegir a qué campo atribuir su respuesta, puede elegir entre dejar que el visitante escriba su respuesta o seleccionar opciones de una lista de selección que determine (sugerencia: esta última puede ayudar con la limpieza de la base de datos). También puede sobrescribir con su respuesta los datos que tenga actualmente enumerados para ellos, o bien, omitir la pregunta por completo si ya tiene un valor para ellos.</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Reserva de reuniones</strong></td>
  <td>Proporciona al visitante un calendario de fechas disponibles para programar una reunión. Elija la disponibilidad del calendario mediante round robin, un agente específico o mediante reglas personalizadas. Haga clic en <b>Agregar atributo</b> si desea capturar el nombre o la dirección de correo electrónico del agente y asignarlo al registro de persona del visitante del chat para futuras consultas (sugerencia: cree un <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campo personalizado</a> para asignar la información del agente a para no sobrescribir un campo de Marketo Engage estándar).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Objetivo</strong></td>
  <td>Esta es la única tarjeta que los visitantes no verán. Le corresponde a usted determinar en qué momento se logra un objetivo dentro del chat específico (por ejemplo, si su objetivo es recopilar el correo electrónico del visitante, coloque la tarjeta Objetivo inmediatamente después de la captura de información en el flujo).</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Acción*</strong></td>
  <td>De manera similar a los campos ocultos en un formulario, con la tarjeta de acción puede rellenar cualquier atributo de cliente potencial o compañía (que tenga un tipo de datos de <a href="/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md#string">cadena</a>) con valores implícitos que desee capturar con un registro de cliente potencial. Puede añadir la tarjeta de acción en cualquier momento de la conversación y actualizar los atributos respectivos con un valor o tokens nativos que rellenen automáticamente el valor respectivo.
  <p><i>* Esta tarjeta requiere Dynamic Chat Prime. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Chat en directo</strong></td>
  <td>Utilice la tarjeta de chat en vivo cuando desee que los visitantes chateen con un agente en vivo.
  <li>La tarjeta de chat en vivo debe ser la última tarjeta de la sucursal.</li>
  <li>Los visitantes se dirigirán a un agente en cuanto lleguen a esta tarjeta en el flujo, por lo que se recomienda preceder esta tarjeta con una tarjeta de preguntas que pregunte a los visitantes si desean chatear con un agente en directo.</li></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Respuestas generadas*</strong></td>
  <td>Cree un mensaje para el visitante cuando llegue a un determinado punto de la conversación. Configure una serie de preguntas que pueden hacerse de una sola vez para lograr el indicador clave de rendimiento deseado.
  <p><i>* Esta tarjeta requiere Dynamic Chat Prime. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Rama condicional</strong></td>
  <td>Cree ramas en los flujos de diálogo en función de diferentes condiciones. Presente contenido diferente a diferentes personas en el mismo cuadro de diálogo en función de los atributos del cliente potencial y de la compañía en Marketo Engage.</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>Flujo conversacional</strong></td>
  <td>Optimice varios pasos en un flujo dentro de sus cuadros de diálogo utilizando la tarjeta Flujo de conversación.</td>
 </tr>
</table>

## Iconos de Stream Designer {#stream-designer-icons}

En la parte superior derecha de Stream Designer, verás un puñado de íconos. Esto es lo que hacen.

<table>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-1.png"></td>
  <td>Aumenta el tamaño, creando tarjetas más grandes</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-2.png"></td>
  <td>Aleja, crea tarjetas más pequeñas</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-3.png"></td>
  <td>Abre una ventana para que usted pruebe su chat (presione el mismo botón para cerrar)</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-4.png"></td>
  <td>Permite buscar tipos de tarjeta o contenido dentro del flujo</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-5.png"></td>
  <td>Organiza todas las tarjetas del flujo</td>
 </tr>
</table>

## Crear una secuencia {#create-a-stream}

Puede crear secuencias para cuadros de diálogo o [Forms de conversación](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}. En este ejemplo, crearemos uno para un Diálogo.

1. Después de [crear tu Diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}, haz clic en la ficha **[!UICONTROL Transmitir Designer]**.

   ![](assets/stream-designer-6.png)

1. Arrastre y suelte la tarjeta _[!UICONTROL Question]_.

   ![](assets/stream-designer-7.png)

1. En [!UICONTROL Respuesta de bots de chat], escriba la pregunta como desee.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >¡Puede personalizar la experiencia para los visitantes de chat!
   >
   >* Haga clic en el icono &quot;Insertar HTML&quot; `</>` para insertar su propio HTML y obtener el aspecto deseado de la conversación.
   >
   >* Utilice tokens para que los visitantes conocidos del chat personalicen su experiencia (por ejemplo: Hello `{{lead.leadFirstName:""}}`). Haga clic en el icono de llaves `{}` y realice la selección. Agregue un valor predeterminado entre comillas si desea que los visitantes anónimos vean algo genérico (por ejemplo: Hello `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Poke está configurado como on de forma predeterminada, lo que muestra la pregunta de apertura junto al icono de chat sin que el visitante tenga que hacer clic en él para verlo. El Poke solo está disponible en la primera carta de la conversación.

1. Escriba sus respuestas de usuario y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**[!UICONTROL Editar valores almacenados]** es un paso opcional para aquellos que deseen almacenar un valor diferente en la base de datos de lo que se muestra a los visitantes en el bot de chat para los atributos asignados en la tarjeta Pregunta (por ejemplo: el visitante ve &quot;Optimización del motor de búsqueda&quot;, usted almacena ese valor como &quot;SEO&quot;).

1. Para &quot;Sí&quot; queremos reservar una reunión, así que debajo de esa opción, arrastra la tarjeta _Reserva de reunión_.

   ![](assets/stream-designer-10.png)

1. Elija su opción de enrutamiento y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/stream-designer-11.png)

1. Como ese es un objetivo, arrastre la tarjeta _[!UICONTROL Goal]_ debajo de la reserva de la reunión.

   ![](assets/stream-designer-12.png)

1. Asigne un nombre a la meta (o elija una existente) y haga clic en **[!UICONTROL Guardar]**. Asignar una puntuación de conversación es opcional.

   ![](assets/stream-designer-13.png)

1. Para &quot;No&quot; queremos ver si se unen a la lista de correo, así que debajo de esa opción, arrastra otra tarjeta de [!UICONTROL Pregunta].

   ![](assets/stream-designer-14.png)

1. Introduzca su respuesta y añada opciones de respuesta para el visitante. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Para agregar más respuestas, haga clic en **[!UICONTROL Agregar respuesta]**.

1. Debajo de la respuesta &quot;Sí&quot;, arrastre sobre la tarjeta _Captura de información_ para que pueda recopilar el correo electrónico del visitante.

   ![](assets/stream-designer-16.png)

1. Haga clic en la lista desplegable y seleccione **[!UICONTROL Dirección de correo electrónico]**.

   ![](assets/stream-designer-17.png)

1. Introduzca un mensaje de bot de chat y un marcador de posición. Si ya existe un valor para este atributo en la base de datos, elija si desea omitirlo o hacer que los datos lo sobrescriban. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/stream-designer-18.png)

1. Como recopilar su correo electrónico es una meta, arrastre la tarjeta _[!UICONTROL Goal]_ debajo de la captura de información.

   ![](assets/stream-designer-19.png)

1. Asigne un nombre a la meta (o elija una existente) y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/stream-designer-20.png)

1. Recuerde agregar una respuesta si dice &quot;No&quot;. Una opción es arrastrar una tarjeta de mensaje a continuación y decir &quot;gracias de todos modos&quot;. Pero en este ejemplo, les proporcionaremos un documento de PDF gratuito en su lugar.

   ![](assets/stream-designer-21.png)

1. En este ejemplo crearemos un nuevo documento. Asígnele un nombre, escriba la dirección URL del PDF que ya ha alojado y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/stream-designer-22.png)

1. Cuando esté listo para activar el cuadro de diálogo, haga clic en **[!UICONTROL Publicar]**.

   ![](assets/stream-designer-23.png)

>[!NOTE]
>
>Antes de hacer clic en [!UICONTROL Publicar], recuerde que debe [escribir las direcciones URL de destino](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Crear un cuadro de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Criterios de audiencia](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md){target="_blank"}
>* [API de incrustación de Adobe PDF](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"}
