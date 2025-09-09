---
description: 'Notas de la versión de Dynamic Chat, documentos de Marketo: documentación del producto'
title: Notas de la versión de Dynamic Chat
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '3414'
ht-degree: 97%

---

# Notas de la versión de Dynamic Chat {#dynamic-chat-release}

Las versiones de Adobe Dynamic Chat funcionan bajo un modelo de entrega continua que permite un enfoque más gradual para la implementación de funciones. En ocasiones, hay varias versiones en un solo mes, por lo que debe consultar regularmente la información más actualizada.

La página de notas de la versión estándar de Marketo Engage [se encuentra aquí](/help/marketo/release-notes/current.md){target="_blank"}.

## Lanzamiento de junio de 2025 {#june-2025-release}

**Fecha de publicación: 30 de junio de 2025**

### Rediseño de la lógica de enrutamiento {#routing-logic-revamp}

Hemos rediseñado la lógica de enrutamiento de chat en directo en Dynamic Chat para garantizar un comportamiento de participación más inteligente y predecible en todos los tipos de enrutamiento (cuenta, personalizado, equipo y Round Robin). La nueva lógica simplifica los flujos de enrutamiento y mejora la gestión de reserva cuando los agentes no están disponibles.

#### Mejoras clave en el comportamiento del enrutamiento

* **Hasta dos intentos de participación por sesión**

   * El sistema intentará conectarse con hasta dos agentes (como máximo), pero estrictamente dentro de la regla de enrutamiento principal.

   * Si un agente está disponible, pero no responde (por ejemplo, rechaza o no responde al chat), el sistema intenta conectarse a un agente diferente del mismo grupo.

   * La lógica de reserva (como Round Robin) solo se activa si no se encuentran agentes aptos durante la resolución inicial, para no volver a intentarlo después de una participación fallida.

* **Comportamiento específico de la regla de enrutamiento**

##### —Enrutamiento de cuenta—

Si el dominio de correo electrónico de un visitante se asigna a una cuenta conocida, siempre se da prioridad al agente asignado.

Si el agente está disponible, el chat se dirige a ellos directamente.

Si el agente no está disponible, el sistema hace lo siguiente:

* No intenta otro agente, incluso si Round Robin está habilitado como alternativa.

* En su lugar, hace lo siguiente:

   * Muestra el calendario de reuniones del agente asignado (si está activado).
o
   * Vuelve a un mensaje predeterminado (en el peor de los casos).

La regla de enrutamiento a nivel de tarjeta (por ejemplo, equipo o personalizado) solo se tiene en cuenta si el enrutamiento de cuenta no es apto (no hay dominio o agente que coincida).

##### —Enrutamiento personalizado o de equipo—

Estas reglas pueden devolver varios agentes aptos.

Si el primer agente disponible no participa, el sistema probará con otro agente de la misma lista.

La reserva de Round Robin no se activa solo porque un agente no responda.

Si ninguno de los agentes participa, ocurre lo siguiente:

* El sistema muestra el calendario del primer agente probado (si está activado).
o
* Muestra el mensaje de reserva predeterminado.

##### —Enrutamiento Round Robin—

Cuando se utiliza como regla de enrutamiento principal, el sistema hace lo siguiente:

* Intenta hacer participar el primer agente disponible del grupo Round Robin.

* Si el primer agente no responde, vuelve a intentarlo con el siguiente mejor agente apto.

Si se utiliza el Round Robin como reserva, solo se activa si no se resuelve ningún agente a partir de la regla principal.

##### Flujo de experiencia del visitante

El sistema comprueba si se aplica el enrutamiento de cuentas.

* Si es el caso y el agente está disponible, se conecta inmediatamente.

* Si el agente no es apto o no está disponible, continúa con la regla de enrutamiento a nivel de tarjeta.

Se evalúa la regla de enrutamiento a nivel de tarjeta (personalizado, equipo o Round Robin).

* Se comprueba la disponibilidad de los agentes aptos (permisos, estado).

* El sistema hace participar a un agente y, si es necesario, lo intenta con un segundo agente desde la misma regla.

* Si ningún intento de participación tiene éxito, se aplica la lógica de reserva:

   * Reserva de calendario (si está activada),
o
   * Mensaje predeterminado.

La reserva de Round Robin solo se tiene en cuenta cuando no se encuentran agentes aptos según la regla de enrutamiento principal, no cuando los agentes individuales no responden.

##### Casos de uso

<p>

_&#x200B;**Enrutamiento de cuenta**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>El dominio del visitante se asigna a una cuenta; el agente asignado tiene habilitado el chat en directo y está disponible</td>
    <td>El chat se conecta directamente al agente asignado</td>
  </tr>
  <tr>
    <td>Reserva (Round Robin)</td>
    <td>El agente asignado no está disponible, la reserva de Round Robin está habilitada</td>
    <td>El sistema selecciona un agente disponible mediante Round Robin y lo hace participar </td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>El agente asignado no está disponible, no hay reserva de Round Robin; la reserva de reunión está habilitada</td>
    <td>El sistema muestra el calendario del agente asignado o un mensaje de reserva predeterminado</td>
  </tr>
</tbody></table>

_&#x200B;**Enrutamiento personalizado**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>La lógica personalizada resuelve una lista de agentes; el primer agente está disponible y acepta el chat.</td>
    <td>El chat se conecta al primer agente.</td>
  </tr>
  <tr>
    <td>Reserva (Round Robin)</td>
    <td>La regla personalizada no resuelve ningún agente, la reserva de Round Robin está activada.</td>
    <td>El sistema selecciona un agente disponible mediante Round Robin y lo hace participar.</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>Dos agentes resueltos; ninguno acepta el chat, la reserva se establece en el calendario de reuniones.</td>
    <td>Se muestra el calendario del primer agente probado o se muestra el mensaje de reserva predeterminado.</td>
  </tr>
</tbody></table>

_&#x200B;**Enrutamiento de equipo**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>El equipo incluye agentes en el chat en directo; el primer agente disponible acepta el chat.</td>
    <td>El chat se conecta a ese agente.</td>
  </tr>
  <tr>
    <td>Reserva (Round Robin)</td>
    <td>No hay ningún agente de equipo disponible y la reserva de Round Robin está habilitada.</td>
    <td>El sistema selecciona y se conecta a un agente del grupo Round Robin.</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>Hay dos agentes disponibles, pero ninguno de los dos participa; la reserva de calendario está habilitada.</td>
    <td>Se muestra el calendario del primer agente con el que se probó o se activa un mensaje de reserva.</td>
  </tr>
</tbody></table>

_&#x200B;**Enrutamiento Round Robin**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>El grupo Round Robin tiene varios agentes; el segundo agente acepta el chat después del primero no.</td>
    <td>El chat se conecta a un segundo agente.</td>
  </tr>
  <tr>
    <td>Reserva (Round Robin)</td>
    <td>No hay agentes disponibles en el grupo Round Robin; el calendario de reuniones está habilitado.</td>
    <td>El calendario se muestra para el primer agente de la lista (si está configurado) o el mensaje de reserva.</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>No hay agentes disponibles; la reserva está deshabilitada.</td>
    <td>Se muestra un mensaje de reserva estático al visitante.</td>
  </tr>
</tbody></table>

### Notificación de pulso {#pulse-notification}

Cada vez que un visitante solicita conectarse con un agente, le proporcionamos una notificación interna de la aplicación y del explorador. Pero a veces, los agentes se pierden estos chats.

Con esta versión, el agente activo puede recibir un correo electrónico, Slack, en la aplicación y una notificación del explorador cuando un visitante nuevo está interesado en chatear.

1. En la página de inicio de Adobe Experience Cloud, haga clic en el icono Cuenta y seleccione **Preferencias**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Desplácese hacia abajo hasta _Notificaciones_ y realice las selecciones de Dynamic Chat que desee.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>El contenido de una notificación de pulso puede ser el mismo que el que utilizamos para las notificaciones en la aplicación y en el explorador.

## Versión de abril/mayo de 2025 {#apr-may-25-release}

### Sonido de notificación de mensaje {#message-notification-sound}

Ahora tiene la opción de habilitar un sonido para el visitante cada vez que se activa el bot de chat en una sesión. Hay varios sonidos para elegir.

### Habilitar los mensajes Poke en el dispositivo móvil {#enable-poke-messages-on-mobile}

“Poke”, que muestra la pregunta de apertura junto al icono de chat sin que el visitante tenga que hacer clic para verla, ahora es una opción que se puede habilitar para visitantes que usen un dispositivo móvil.

### Actualización de reserva predeterminada {#default-fallback-update}

Para cualquier regla/equipo personalizado como una tarjeta de chat en directo: si no hay agentes disponibles (o el chat no se puede conectar), volverá a Round Robin para buscar agentes disponibles (todos los que estén disponibles en ese momento, independientemente de la lógica o regla de enrutamiento que se puso en el flujo).

### Integración con Demandbase {#demandbase-integration}

Los usuarios de Demandbase pueden utilizar los atributos de persona de Demandbase para la segmentación de diálogos, la promoción condicional de la marca y el enrutamiento personalizado en Dynamic Chat.

## Versión de septiembre/octubre de 2024 {#sep-oct-release}

### Análisis de chat en directo mejorado {#enhanced-live-chat-analytics}

Se han realizado varias mejoras en el panel de análisis, entre las que se incluyen:

* Número recuento total solicitado de chats en directo: número de visitantes solicitados para un “chat con el agente”

* Total de chats conectados en directo: número de visitantes conectados frente al total solicitado para un “chat con el agente”

* Total de solicitudes de chat en directo perdidas: número de visitantes no atendidos frente al total solicitado para un “chat con el agente”

* Duración promedio del chat en minutos: analice la “duración promedio del chat” entre los visitantes y sus agentes

* Tiempo promedio de respuesta del agente en segundos: analice el “tiempo promedio empleado” por los agentes para responder a sus preguntas y respuestas en directo en el chat

* Panel diario: las solicitudes de chat en directo se conectan correctamente, las solicitudes de chat en directo perdidas, ordenar y filtrar las actividades de chat en directo recientes

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Puntuación de la conversación {#conversation-scoring}

Cuantifique los posibles clientes en función de la calidad de su interacción con el chat y utilice esa métrica como activador/filtro en campañas inteligentes de Marketo Engage. Use el nuevo atributo _puntuación de conversación_ en las siguientes actividades:

* Participa en un diálogo
* Participa en un flujo conversacional
* Participa con un agente

**Aspectos a tener en cuenta:**

* El valor de la puntuación oscilará entre 0, 1, 2 y 3 (el valor predeterminado es nulo)

* Cuando finaliza o se pierde la conversación, el valor de puntuación no se puede editar

* Para configurar una puntuación, haga lo siguiente:

   * En la bandeja de entrada del agente: durante una conversación en directo, el agente puede actualizar o establecer una puntuación para la conversación, que se almacena en la actividad de conversación

   * En el diseñador de flujo: en la tarjeta de objetivos, el usuario puede actualizar o establecer una puntuación para la conversación

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Nueva lógica de creación de posibles clientes {#new-lead-creation-logic}

Si un posible cliente rellena un formulario con el correo electrónico `abc@test.com` y queda marcado con la cookie xyz, más adelante rellena el mismo formulario con el correo electrónico `def@test.com`, se crea un nuevo registro de persona, pero la cookie xyz se asocia con la nueva persona y se elimina de la persona `abc@test.com`.

Por lo tanto, cuando un visitante con cookie abc aterriza en una página y proporciona un ID de correo electrónico como `abc@test.com`:

<table><thead>
  <tr>
    <th>Visitante</th>
    <th>Cookie</th>
    <th>Correo electrónico proporcionado</th>
    <th>Comportamiento esperado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anónimo</td>
    <td>abc</td>
    <td>No existe en la base de datos</td>
    <td>Crear una nueva persona</td>
  </tr>
  <tr>
    <td>Anónimo</td>
    <td>abc</td>
    <td>Existe en la base de datos</td>
    <td>Combinar persona</td>
  </tr>
  <tr>
    <td>Anónimo</td>
    <td>xyz</td>
    <td>Existe en la base de datos</td>
    <td>Combinar persona</td>
  </tr>
  <tr>
    <td>Persona conocida</td>
    <td>abc</td>
    <td>Igual que la persona existente</td>
    <td>Actualizar persona</td>
  </tr>
  <tr>
    <td>Persona conocida</td>
    <td>abc</td>
    <td>Diferente a la persona existente</td>
    <td>Si ya existe una persona conocida, transfiera la cookie y resuelva ese perfil. Si no existe ninguna persona con este correo electrónico, cree un nuevo registro de persona y transfiera la cookie</td>
  </tr>
  <tr>
    <td>Persona conocida</td>
    <td>xyz</td>
    <td>Igual que la persona existente</td>
    <td>Añadir nueva cookie a la misma persona</td>
  </tr>
  <tr>
    <td>Persona conocida</td>
    <td>xyz</td>
    <td>Diferente a la persona existente</td>
    <td>este escenario no es posible como si se tratara de una nueva cookie de   considerado de forma predeterminada como un nuevo perfil anónimo</td>
  </tr>
</tbody></table>

### Opción para heredar la fuente {#option-to-inherit-font}

Ahora puede permitir que el bot de chat herede directamente la fuente de la página web en la que se aloja en lugar de administrar la fuente de la marca en Dynamic Chat. Al habilitar esta opción, el bot de chat tomará la fuente definida en la etiqueta `<body>` de la página.

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Integración de Demandbase con Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Los usuarios de Demandbase pueden traer su propia licencia de Demandbase y activar la integración. Utilice los atributos de persona de Demandbase para la segmentación de diálogos, la promoción condicional de la marca y el enrutamiento personalizado.

La resolución de estos valores de atributo con una persona se realizaría en tiempo real y se almacenaría en el perfil de persona correspondiente.

### Tiempo de carga de flujo de conversación optimizado {#optimized-conversation-flow-load-time}

Para mejorar la experiencia del usuario, ahora se muestra un cargador con efecto brillante en lugar de un espacio en blanco mientras se carga el flujo de conversación.

**Antes**

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**Después**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## Versión de agosto de 2024 {#august-release}

**Fecha de lanzamiento: 23 de agosto de 2024**

### Personalizar el formato de los mensajes de conversación {#custom-format-conversation-messages}

Los diseñadores de flujo ahora permiten [insertar un HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"} para personalizar la apariencia de sus conversaciones.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Desplazamiento del bot de chat hasta la parte inferior {#chatbot-scroll-to-bottom}

Se ha añadido un icono en el bot de chat para que los visitantes web salten directamente al último mensaje. Esto ayuda a los visitantes a desplazarse por el texto para volver rápidamente a la conversación.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Notificaciones de pulso principales {#core-pulse-notifications}

Ahora los usuarios reciben una [notificación por correo electrónico](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"} cuando falla una reserva de reunión o un chat en directo.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Compatibilidad con varias conversaciones {#support-for-multiple-conversations}

El bot de chat ahora admite varias conversaciones. Los visitantes del sitio web pueden participar en diferentes conversaciones en diferentes páginas al mismo tiempo, con la capacidad de alternar entre ellas.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Ordenación predeterminada del contenido {#default-sorting-for-content}

De forma predeterminada, los registros de conversaciones, las preguntas sin responder y las tablas de generación de preguntas se ordenan por la fecha de creación (de la más reciente a la más antigua).

### Resolución de posibles clientes en tiempo real {#real-time-lead-resolution}

Durante una conversación con un posible cliente anónimo, se proporciona un ID de correo electrónico, resolvemos si existe un registro de posible cliente conocido con ese ID de correo electrónico y utilizamos ese registro para la personalización en tiempo real. Si encontramos varios registros, los combinamos en tiempo real. Este funcionamiento se implementa tanto en los diálogos como en los flujos conversacionales.

### Sincronización de posibles clientes sin cookies de Marketo Engage {#syncing-leads-without-cookies}

Anteriormente, cuando se activaba la sincronización de Marketo Engage, Dynamic Chat solo sincronizaba los posibles clientes conocidos con uno o más ID de cookie de Marketo Engage. Ahora, todos los posibles clientes conocidos (con ID de cookie presente o no) se sincronizarán con Dynamic Chat y se pueden utilizar para personalizar las conversaciones.

### Pasar datos sobre visitantes adicionales a flujos conversacionales {#pass-additional-visitor-data}

Si está capturando información sobre visitantes a través de otros canales, como formularios o inicios de sesión, ahora puede pasar esta información directamente a Dynamic Chat.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Datos deducidos actualizados {#refreshed-inferred-data}

La mayoría de las conversaciones en un sitio web son con personas visitantes anónimas. Aún puede dirigirse a dichos visitantes con datos deducidos, que dependen de las direcciones IP de los visitantes. Hemos actualizado nuestra base de datos de IP y los datos inferidos respectivos, que ahora admiten cuatro veces más IP.

### Sonido añadido a la notificación del explorador del agente {#sound-added-to-agent-browser-notification}

Cuando se asigna un chat en directo a un agente, recibe una notificación del explorador. Pero de vez en cuando no los ven. Hemos añadido un [sonido de notificación](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} para ayudar a evitar que se pierdan notificaciones en el futuro.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Posibilidad de actualizar el perfil del posible cliente durante el chat en directo {#update-lead-profile-during-live-chat}

Durante un chat en directo, los agentes quieren capturar información sobre el visitante y actualizar el perfil respectivo. Ahora existe la opción de actualizar los valores de atributo de los objetos de posibles clientes y de compañías.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Lanzamiento de junio de 2024 {#june-release}

**Fecha de publicación: 6 de junio de 2024**

### Tarjeta de flujo conversacional {#conversational-flow-card}

Optimice varios pasos en un flujo dentro de sus diálogos aprovechando la tarjeta Flujo conversacional.

Ejemplo: si su objetivo es impulsar los registros para su seminario web a través de varios diálogos, debe volver a crear el mismo flujo en todos los diálogos que tengan ese objetivo. Y si tiene que actualizar cualquier detalle, tendrá que editar cada diálogo individual de uno en uno. Ya no es así, gracias a la tarjeta Flujo conversacional.

Además de reutilizar los flujos a través de varios diálogos, también puede utilizar el mismo flujo de transición para que se active a través de otros canales, como formularios y páginas de aterrizaje.

![](assets/dynamic-chat-june-2024-release-1.png)

### Límites de uso {#usage-limits}

La página Límites de uso muestra información importante, como los detalles del paquete y el estado del límite de uso.

![](assets/dynamic-chat-june-2024-release-2.png)

## Lanzamiento de mayo de 2024 {#may-release}

**Fecha de la versión: 15 de mayo de 2024**

### Biblioteca de respuestas aprobadas previamente {#pre-approved-response-library}

[Cree una biblioteca con aprobación de marketing](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} de preguntas y respuestas generadas por IA para ayudar a configurar charlas sobre la IA generativa en cuestión de minutos.

![](assets/dynamic-chat-may-2024-release-1.png)

### Preguntas sin respuesta {#unanswered-questions}

[Use un repositorio de preguntas sin responder](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} de conversaciones anteriores para generar nuevas respuestas aprobadas previamente y mantener una biblioteca de respuestas con la información más reciente.

![](assets/dynamic-chat-may-2024-release-2.png)

### Resúmenes de conversación {#conversation-summaries}

[Proporcione a los agentes de ventas conversaciones resumidas](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"} que incluyan información sobre temas clave que se tratarán en las reuniones, con el fin de acortar el tiempo de preparación y dotarles de la información más reciente.

![](assets/dynamic-chat-may-2024-release-3.png)

### Métodos abreviados de ventas de GenAI {#genai-sales-shortcuts}

[Proporcione a los agentes de chat en directo formas más rápidas](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"} de acceder a las respuestas generadas por IA, editar las respuestas generadas existentes y buscar contenido adicional para enviar a los compradores durante la conversación.

![](assets/dynamic-chat-may-2024-release-4.png)

### Asistente de conversación {#conversation-assist}

Ayude a los agentes de ventas a responder con precisión durante las conversaciones en directo mediante respuestas aprobadas previamente por su equipo de marketing.

### Alicientes para la conversación {#conversation-nudges}

Anime a las personas que visitan la web con una llamada a la acción para llevar las conversaciones a buen término.

<p>

## Versión de abril de 2024 {#april-release}

**Fecha de publicación: 23 de abril de 2024**

### Flujos conversacionales ahora disponibles para todos los usuarios {#conversational-flows-available-to-all-users}

Haga que sus formularios y páginas de aterrizaje sean más conversacionales y acorte el embudo de ventas al permitir que los posibles clientes cualificados reserven una reunión o conversen con Ventas inmediatamente después del envío de un formulario con Formularios conversacionales, ahora totalmente disponibles&#42; para todos los usuarios de Dynamic Chat.

_&#42;Anteriormente estaba disponible como función de prueba con 100 interacciones de por vida. Las interacciones en el flujo conversacional ahora se contarán dentro del límite mensual de 250 conversaciones interactivas para los usuarios del paquete Select._

### Funciones de devolución de llamada {#callback-functions}

Las [funciones de devolución de llamada](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} le permiten recopilar eventos de análisis de Dynamic Chat en sistemas externos, como Adobe Analytics o Google Analytics, a medida que las personas que visitan la web interactúan con las conversaciones de Dynamic Chat. Habilite los eventos de análisis de Dynamic Chat registrando una llamada de retorno con la API para escucharlos. Esto le permite tener una vista más integral de su participación en Dynamic Chat en relación con otros datos clave, como el tráfico web.

### Condiciones de la disponibilidad del agente activo añadidas a la ramificación condicional {#live-agent-availability-conditional-branching}

Además de los campos nativos y personalizados de Marketo Engage, ahora puede utilizar la ramificación condicional para crear ramas en función de la disponibilidad del agente. Esto resulta útil si solo desea ofrecer a las personas visitantes la opción de hablar con un agente activo cuando hay agentes activos disponibles.

![](assets/dynamic-chat-release-1.png)

### Condición de lista inteligente añadida a la ramificación condicional {#smart-list-condition}

Con la incorporación de la nueva condición de lista inteligente de Marketo Engage en la ramificación condicional, puede crear ramas basadas en públicos ya existentes que ya haya creado en Marketo Engage, en lugar de definir condiciones de ramificación de públicos en Dynamic Chat.

![](assets/dynamic-chat-release-2.png)

### Ramificación condicional para flujos conversacionales {#conditional-branching-for-conversational-flows}

Hemos lanzado la ramificación condicional para los diálogos a principios de este año, y ahora también puede aprovechar la ramificación condicional en los flujos conversacionales. La ramificación condicional le permite crear ramas en el flujo en función de diferentes condiciones.

### Chat en directo para flujos conversacionales {#live-chat-for-conversational-flows}

Hemos lanzado la funcionalidad de chat en directo para los diálogos de 2023, y ahora también puede añadir interacciones de chat en directo a sus flujos conversacionales. Si utiliza flujos conversacionales con sus formularios de Marketo Engage, ahora puede permitir que personas visitantes cualificadas chateen con un agente en directo inmediatamente después del envío del formulario.

### Actividades recientes de Marketo Engage en la bandeja de entrada del agente {#recent-marketo-engage-activities-in-agent-inbox}

Hemos añadido actividades recientes de Marketo Engage a la sección Actividades recientes de la bandeja de entrada del agente, de modo que cuando una persona que visita el sitio solicita hablar con un agente, este puede ver rápidamente si dicha persona ha participado recientemente en alguna de las siguientes actividades de Marketo Engage (últimas 25 actividades):

* Correo electrónico abierto
* Página web visitada
* Formulario completo
* Tuvo un momento interesante

![](assets/dynamic-chat-release-3.png)

### Estado de conexión del calendario en la administración de agentes {#calendar-connection-status-in-agent-management}

Los administradores ahora pueden ver fácilmente qué agentes con permisos para reservar reuniones han conectado sus calendarios en Dynamic Chat. Esto le permite asegurarse de que todo su equipo de ventas esté conectado y listo para aceptar convocatorias de reunión de Dynamic Chat.

![](assets/dynamic-chat-release-4.png)

### Configuración mínima de aviso en la configuración del calendario del agente {#minimum-notice-setting-in-agent-calendar-configuration}

Los usuarios informaron de que las personas que visitan la web reservaban reuniones en su calendario con tan solo 10 minutos de antelación, por lo que introdujimos una configuración de aviso mínimo en la configuración del calendario del agente y establecimos el tiempo de espera predeterminado en 24 horas.

![](assets/dynamic-chat-release-5.png)

### Comportamiento para añadir y quitar usuarios actualizado {#add-remove-user-behavior-updated}

Algunos usuarios indicaron que tenían problemas para añadir y quitar agentes en Dynamic Chat, por lo que realizamos algunos cambios para resolver estos problemas.

Cuando se añade un usuario a Admin Console con permiso para participar en chats en directo o reservar reuniones, se muestra inmediatamente en la lista de administración de agentes y está disponible para añadirlo a los diálogos, flujos conversacionales, reglas de enrutamiento y equipos.

Cuando un usuario con permisos para reservar reuniones o participar en chats en directo se quita de Admin Console, se quita inmediatamente de Dynamic Chat, ya no estará disponible para el chat en directo o el enrutamiento de reuniones y ya no contará para los límites de licencia.

### Se ha mejorado el rendimiento del informe a nivel de conversación {#improved-conversation-level-report-performance}

Los informes a nivel de diálogo individual y flujo conversacional ahora son más precisos y eficaces. Anteriormente, los informes de Diálogo podían tardar varios segundos en cargarse y, en ocasiones, los datos no eran coherentes con los informes de rendimiento globales. Ahora, los informes de diálogo individuales se cargan en un instante, y los datos siempre se alinean con los datos del sistema de informes globales.

![](assets/dynamic-chat-release-6.png)

### Actualizaciones de permisos {#permission-updates}

Hemos limpiado la estructura de permisos y los nombres en Adobe Admin Console para que la administración de permisos sea más intuitiva.

* La categoría «Administración de conversaciones» ahora se denomina «Conversaciones»
* La categoría «Reuniones» ahora se denomina «Actividades»
* La categoría «Configuración de agentes» ahora se denomina «Agentes»
* La categoría «Configuración del administrador» ahora se llama «Configuración»
* Se eliminó la categoría «Chat en directo» y todos los permisos de chat en directo se movieron a la categoría Agentes

![](assets/dynamic-chat-release-7.png)

### Compatibilidad con hipervínculos en la bandeja de entrada del agente {#support-for-hyperlinks-in-agent-inbox}

Ahora, cuando los agentes del chat en directo comparten direcciones URL con las personas que visitan el chat, esas direcciones URL contendrán hipervínculos para que las personas visitantes puedan simplemente hacer clic en ellas para navegar a la página, en lugar de tener que copiar y pegar la URL en su explorador.

### Introducir el comportamiento de clave actualizado en la bandeja de entrada del agente {#enter-key-behavior-updated-in-agent-inbox}

Hemos cambiado el comportamiento de la tecla de retorno en la bandeja de entrada del agente, por lo que al pulsar la tecla Entrar o Retorno se enviará el mensaje y al pulsar Mayús+Entrar se creará un salto de línea.

![](assets/dynamic-chat-release-8.png)

### Página de operación de distribución equilibrada eliminada {#round-robin-page-removed}

No se preocupe. El enrutamiento de distribución equilibrada sigue siendo completamente funcional y funciona del mismo modo que siempre lo ha hecho. Acabamos de eliminar la página que mostraba una lista de agentes a menudo inexacta y su orden en la cola de enrutamiento de distribución equilibrada.

Cuando lanzamos Dynamic Chat en 2022, no había compatibilidad con el chat en directo, solo con las reservas de reuniones, y la página de enrutamiento Round Robin se diseñó teniendo en cuenta solo las reservas de reuniones. Con la introducción del chat en directo el año pasado, la página Round Robin se volvió obsoleta, ya que no reflejaba con precisión la naturaleza más compleja del enrutamiento Round Robin entre agentes con permisos tanto de reservas de reuniones como de chat en directo. Exploramos algunas opciones diferentes para resolver esto, pero finalmente decidimos eliminarlo por completo, ya que era la mejor opción para minimizar la confusión.

![](assets/dynamic-chat-release-9.png)

## Lanzamiento de febrero de 2024 {#february-release}

**Fecha de publicación: 22 de febrero de 2024**

### Página Conversaciones {#conversations-page}

La nueva página Conversaciones le ofrece un lugar único para ver las transcripciones de todas las conversaciones (automatizadas y en directo) que se produjeron para su instancia, tanto de posibles clientes conocidos como anónimos, lo que le ofrece una mejor visibilidad de cómo sus clientes participan en sus diálogos, flujos de conversación y agentes en directo.

![](assets/dynamic-chat-release-10.png)

### El intervalo de fechas en el panel global aumentó de 90 días a 24 meses {#date-range-in-global-dashboard}

Usted lo pidió y lo implementamos. Ahora puede ver datos de participación de Dynamic Chat de hasta dos años en todos los paneles de análisis.

### Ramificación condicional en diálogos {#conditional-branching-in-dialogues}

La ramificación condicional permite crear ramificaciones en los flujos de diálogo en función de diferentes condiciones. Ahora puede presentar contenido diferente a distintas personas en el mismo diálogo en función de los atributos del posible cliente y de la empresa en Marketo Engage.

## Lanzamiento de enero de 2024 {#january-release}

**Fecha de la versión: 24 de enero de 2024**

### Configuración del límite de chat en directo simultáneo en la administración de agentes {#Concurrent-live-chat-limit-setting}

De forma predeterminada, cada agente de chat en directo de su instancia puede participar en un máximo de cinco sesiones de chat en vivo a la vez. Hemos introducido una nueva configuración en la administración de agentes que le permite ajustar este límite de 1 a 10.

![](assets/dynamic-chat-release-11.png)
