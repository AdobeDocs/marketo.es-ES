---
description: Notas de la versión del Dynamic Chat - Documentos de Marketo - Documentación del producto
title: Notas de la versión de Dynamic Chat
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: e2fcd5587df8776a07b092cd03f081a88480353e
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Notas de la versión de Dynamic Chat {#dynamic-chat-release}

Las versiones de Adobe Dynamic Chat funcionan con un modelo de entrega continua que permite un enfoque más escalable de la implementación de funcionalidades. A veces hay varias versiones en un mes, por lo que vuelva a consultar regularmente la información más actualizada.

La página de notas de la versión estándar de Marketo Engage [se puede encontrar aquí](/help/marketo/release-notes/current.md){target="_blank"}.

## Lanzamiento de abril de 2024 {#april-release}

**Fecha de publicación: 16 de abril de 2024**

### Flujos de conversación ahora disponibles para los usuarios en Seleccionar paquete {#conversational-flows-select-package}

Cuando lanzamos Conversational Flows el año pasado, los que estaban en el paquete Dynamic Chat Select solo podían aprovechar la capacidad como una prueba de 100 participaciones de por vida. Ahora, los flujos de conversación están totalmente disponibles para todos los que formen parte del paquete Select.

Las participaciones en Flujo de conversación se contarán para el límite mensual de 250 conversaciones comprometidas para los usuarios en el paquete Seleccionar.

### Funciones de devolución de llamada {#callback-functions}

Las funciones de llamada de retorno permiten recopilar eventos de análisis de Dynamic Chat en sistemas externos, como Adobe Analytics o Google Analytics, a medida que los visitantes interactúan con conversaciones de Dynamic Chat. Para habilitar los eventos de Dynamic Chat Analytics, registre una llamada de retorno con la API para escucharlos. Esto le permite tener una vista más integral de la participación del Dynamic Chat en relación con otros datos clave, como el tráfico web.

### Condiciones de disponibilidad del agente activas añadidas a la ramificación condicional {#live-agent-availability-conditional-branching}

Además de los campos de Marketo Engage nativo y personalizado, ahora puede utilizar la ramificación condicional para crear ramas en función de la disponibilidad del agente. Esto resulta útil si solo desea ofrecer a los visitantes la opción de hablar con un agente activo cuando hay agentes activos disponibles.

![](assets/dynamic-chat-release-1.png)

### Condición de lista inteligente agregada a la bifurcación condicional {#smart-list-condition}

Con la adición de la nueva condición de lista inteligente de Marketo Engage en la bifurcación condicional, puede crear ramas basadas en audiencias preexistentes que ya ha creado en Marketo Engage, en lugar de definir condiciones de bifurcación de audiencias en Dynamic Chat.

![](assets/dynamic-chat-release-2.png)

### Ramificación condicional para flujos de conversación {#conditional-branching-for-conversational-flows}

Hemos lanzado la ramificación condicional para los cuadros de diálogo a principios de este año, y ahora también puede aprovechar la ramificación condicional en los flujos de conversación. La ramificación condicional permite crear ramas en el flujo en función de diferentes condiciones.

### Chat en vivo para Flujos de conversación {#live-chat-for-conversational-flows}

Hemos lanzado la funcionalidad de chat en vivo para Diálogos en 2023, y ahora también puede agregar compromisos de chat en vivo a sus Flujos de conversación. Si utiliza flujos de conversación con sus formularios de Marketo Engage, ahora puede permitir que visitantes cualificados chateen con un agente en directo inmediatamente después del envío del formulario.

### Actividades recientes del Marketo Engage en la bandeja de entrada del agente {#recent-marketo-engage-activities-in-agent-inbox}

Hemos añadido actividades de Marketo Engage recientes a la sección Actividades recientes de la bandeja de entrada del agente, de modo que cuando un visitante del sitio solicita hablar con un agente, este puede ver rápidamente si el visitante ha participado recientemente en alguna de las siguientes actividades de Marketo Engage (últimas 25 actividades):

* Abrió el email
* Página web visitada
* Completó el formulario
* Tuvo un momento interesante

![](assets/dynamic-chat-release-3.png)

### Estado de conexión del calendario en la administración de agentes {#calendar-connection-status-in-agent-management}

Los administradores ahora pueden ver fácilmente qué agentes con permisos de reservas de reuniones han conectado sus calendarios en Dynamic Chat. Esto le permite asegurarse de que todo su equipo de ventas está conectado y listo para aceptar convocatorias de reunión de Dynamic Chat.

![](assets/dynamic-chat-release-4.png)

### Configuración mínima de aviso en la configuración del calendario del agente {#minimum-notice-setting-in-agent-calendar-configuration}

Los usuarios informaron de que los visitantes web reservaban reuniones en su calendario con tan solo 10 minutos de antelación, por lo que introdujimos una configuración de aviso mínimo en la configuración del calendario del agente y establecimos el tiempo de espera predeterminado en 24 horas.

![](assets/dynamic-chat-release-5.png)

### Comportamiento para agregar o quitar usuarios actualizado {#add-remove-user-behavior-updated}

Algunos usuarios indicaron que tenían problemas para agregar y eliminar agentes en Dynamic Chat, por lo que realizamos algunos cambios para resolver estos problemas.

Cuando se agrega un usuario al Admin Console con permiso de citas en directo o de citas, se muestra inmediatamente en la lista de administración del agente y está disponible para agregarlo a los cuadros de diálogo, los flujos de conversación, las reglas de enrutamiento y los equipos.

Cuando un usuario con permisos de reserva de reuniones o chat en vivo se elimina del Admin Console, se elimina inmediatamente del Dynamic Chat, ya no estará disponible para el chat en vivo o el enrutamiento de reuniones, y ya no contará con los límites de licencia.

### Rendimiento de informe de nivel de conversación mejorado {#improved-conversation-level-report-performance}

Los informes de nivel de flujo de diálogo individual y conversación ahora son más precisos y eficaces. Anteriormente, los informes de Diálogo podían tardar varios segundos en cargarse y, en ocasiones, los datos no eran coherentes con los informes de rendimiento globales. Ahora, los informes de Diálogo individuales se cargan en un instante y los datos siempre se alinean con los datos de informes globales.

![](assets/dynamic-chat-release-6.png)

### Actualizaciones de permisos {#permission-updates}

Hemos limpiado la estructura de permisos y los nombres en Adobe Admin Console para que la administración de permisos sea más intuitiva.

* La categoría &quot;Administración de conversaciones&quot; ahora se denomina &quot;Conversaciones&quot;
* La categoría &quot;Reuniones&quot; ahora se denomina &quot;Actividades&quot;
* La categoría &quot;Configuración de agente&quot; ahora se denomina &quot;Agentes&quot;
* La categoría &quot;Configuración de administración&quot; ahora se llama &quot;Configuración&quot;
* Se eliminó la categoría &quot;Chat en directo&quot; y todos los permisos de chat en directo se movieron a la categoría Agentes

![](assets/dynamic-chat-release-7.png)

### Compatibilidad con hipervínculos en la bandeja de entrada del agente {#support-for-hyperlinks-in-agent-inbox}

Ahora, cuando los agentes de chat en vivo comparten direcciones URL con los visitantes en el chat, esas direcciones URL estarán hipervinculadas para que los visitantes puedan simplemente hacer clic en ellas para navegar a la página, en lugar de tener que copiar y pegar la URL en su explorador.

### Introduzca el comportamiento de clave actualizado en la bandeja de entrada del agente {#enter-key-behavior-updated-in-agent-inbox}

Hemos cambiado el comportamiento de la tecla de retorno en la bandeja de entrada del agente, por lo que al pulsar la tecla Intro o Retorno se enviará el mensaje y al pulsar Mayús+Intro se creará un salto de línea.

![](assets/dynamic-chat-release-8.png)

### Página de operación por turnos eliminada {#round-robin-page-removed}

¡No te preocupes! El enrutamiento round robin sigue siendo completamente funcional y funciona del mismo modo que siempre lo ha hecho. Acabamos de eliminar la página que mostraba una lista de agentes a menudo inexacta y su orden en la cola de enrutamiento round robin.

Cuando lanzamos Dynamic Chat en 2022, no había compatibilidad con el chat en vivo, solo con las reservas de reuniones y la página de enrutamiento round robin se diseñó teniendo en cuenta solo las reservas de reuniones. Con la introducción del chat en vivo el año pasado, la página round robin se volvió obsoleta ya que no reflejaba con precisión la naturaleza más compleja del enrutamiento round robin entre agentes con permisos tanto de reservación de reuniones como de chat en vivo. Exploramos algunas opciones diferentes para resolver esto, pero finalmente decidimos que eliminarlo por completo era la mejor opción para minimizar la confusión.

![](assets/dynamic-chat-release-9.png)

## Lanzamiento de febrero de 2024 {#february-release}

**Fecha de publicación: 22 de febrero de 2024**

### Página Conversaciones {#conversations-page}

La nueva página Conversaciones le ofrece una ventanilla única para ver las transcripciones de todas las conversaciones (automatizadas y en directo) que se produjeron para su instancia, tanto de posibles clientes conocidos como anónimos, lo que le ofrece una mejor visibilidad de cómo sus clientes interactúan con sus diálogos, flujos de conversación y agentes activos.

![](assets/dynamic-chat-release-10.png)

### El intervalo de fechas en el panel global aumentó de 90 días a 24 meses {#date-range-in-global-dashboard}

Tú preguntaste y nosotros lo hicimos. Ahora puede ver datos de participación del Dynamic Chat de hasta dos años en todos los paneles de análisis.

### Ramificación condicional en cuadros de diálogo {#conditional-branching-in-dialogues}

La ramificación condicional permite crear ramas en los flujos de diálogo en función de diferentes condiciones. Ahora puede presentar contenido diferente a distintas personas en el mismo cuadro de diálogo en función de los atributos del posible cliente y de la empresa en Marketo Engage.

## Lanzamiento de enero de 2024 {#january-release}

**Fecha de la versión: 24 de enero de 2024**

### Configuración del límite de chat en directo simultáneo en la administración de agentes {#Concurrent-live-chat-limit-setting}

De forma predeterminada, cada agente de chat en vivo de su instancia puede participar en un máximo de 5 sesiones de chat en vivo a la vez. Hemos introducido una nueva configuración en la administración de agentes que le permite ajustar este límite de 1 a 10.

![](assets/dynamic-chat-release-11.png)
