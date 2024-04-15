---
description: Notas de la versión del Dynamic Chat - Documentos de Marketo - Documentación del producto
title: Notas de la versión de Dynamic Chat
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Notas de la versión: abril de 2024 {#release-notes-apr-24}

Las versiones de Adobe Dynamic Chat funcionan con un modelo de entrega continua que permite un enfoque más escalable de la implementación de funcionalidades. A veces hay varias versiones en un mes, por lo que vuelva a consultar regularmente la información más actualizada.

La página de notas de la versión estándar de Marketo Engage [se puede encontrar aquí](/help/marketo/release-notes/current.md){target="_blank"}.

## Versión de abril {#april-release}

**Fecha de publicación: 16 de abril de 2024**

### Flujos de conversación ahora disponibles para los clientes en un paquete Select {#conversational-flows-select-package}

Cuando lanzamos Conversational Flows el año pasado, los clientes del paquete Dynamic Chat Select solo podían aprovechar esta capacidad como una prueba de 100 participaciones de por vida. Ahora los flujos de conversación están totalmente disponibles para todos los clientes en el paquete Select.

Las participaciones en Flujo de conversación se contarán para el límite mensual de 250 conversaciones comprometidas para los clientes en el paquete Seleccionar.

### Funciones de devolución de llamada {#callback-functions}

Las funciones de llamada de retorno permiten recopilar eventos de análisis de Dynamic Chat en sistemas externos, como Adobe Analytics o Google Analytics, a medida que los visitantes interactúan con conversaciones de Dynamic Chat. Para habilitar los eventos de Dynamic Chat Analytics, registre una llamada de retorno con la API para escucharlos. Esto le permite tener una vista más holística de la participación del Dynamic Chat en relación con otros datos clave, como el tráfico web.

### Condiciones de disponibilidad del agente activas añadidas a la ramificación condicional {#live-agent-availability-conditional-branching}

Además de los campos nativos y personalizados de Marketo, ahora puede utilizar la ramificación condicional para crear ramas en función de la disponibilidad del agente. Esto resulta útil si solo desea ofrecer a los visitantes la opción de hablar con un agente activo cuando hay agentes activos disponibles.

CAPTURA DE PANTALLA

### Condición de lista inteligente agregada a la bifurcación condicional {#smart-list-condition}

Con la adición de la nueva condición de lista inteligente de Marketo Engage en la bifurcación condicional, puede crear ramas basadas en audiencias preexistentes que ya ha creado en Marketo en lugar de definir condiciones de bifurcación de audiencias en Dynamic Chat.

CAPTURA DE PANTALLA

### Ramificación condicional para flujos de conversación {#conditional-branching-for-conversational-flows}

Hemos lanzado la ramificación condicional para los diálogos a principios de este año y ahora también puede aprovechar la ramificación condicional en los flujos de conversación. La ramificación condicional permite crear ramas en el flujo en función de diferentes condiciones.

### Chat en vivo para Flujos de conversación {#live-chat-for-conversational-flows}

El año pasado lanzamos la funcionalidad de chat en vivo para Diálogos, y ahora también puede agregar compromisos de chat en vivo a sus Flujos de conversación. Si utiliza flujos de conversación con sus formularios de Marketo, ahora puede permitir que visitantes cualificados chateen con un agente en directo inmediatamente después del envío del formulario.

### Actividades recientes del Marketo Engage en la bandeja de entrada del agente {#recent-marketo-engage-activities-in-agent-inbox}

Hemos añadido actividades de Marketo Engage recientes a la sección Actividades recientes de la bandeja de entrada del agente para que cuando un visitante del sitio solicite hablar con un agente, este pueda ver fácilmente si el visitante ha participado recientemente en alguna de las siguientes actividades de Marketo (últimas 25 actividades):

* Abrió el email
* Página web visitada
* Completó el formulario
* Tuvo un momento interesante

CAPTURA DE PANTALLA

### Estado de conexión del calendario en la administración de agentes {#calendar-connection-status-in-agent-management}

Los administradores ahora pueden ver fácilmente qué agentes con permisos de reservas de reuniones han conectado sus calendarios en Dynamic Chat. Esto le permite asegurarse de que todo el equipo de ventas está conectado y listo para aceptar convocatorias de reunión de Dynamic Chat.

CAPTURA DE PANTALLA

### Configuración mínima de aviso en la configuración del calendario del agente {#minimum-notice-setting-in-agent-calendar-configuration}

Los clientes informaron de que los visitantes web reservaban reuniones en su calendario con tan solo 10 minutos de antelación, por lo que introdujimos una configuración de aviso mínimo en la configuración del calendario del agente y establecimos el tiempo de espera predeterminado en 24 horas.

CAPTURA DE PANTALLA

### Nuevas notificaciones en la aplicación {#new-in-app-notifications}

Hemos introducido tres nuevas notificaciones en la aplicación para ayudarle a mantenerse informado del estado de la instancia de Dynamic Chat en tiempo real.

* Texto
* Texto
* Texto

### Comportamiento para agregar o quitar usuarios actualizado {#add-remove-user-behavior-updated}

Algunos clientes nos informan sobre los problemas que tenían al agregar y eliminar agentes en Dynamic Chat, por lo que hemos realizado algunos cambios para solucionar estos problemas.

Cuando se agrega un usuario al Admin Console con permiso de citas en directo o de citas, se muestra inmediatamente en la lista de administración del agente y está disponible para agregarlo a los cuadros de diálogo, los flujos de conversación, las reglas de enrutamiento y los equipos.

Cuando un usuario con permisos de reserva de reuniones o chat en vivo se elimina del Admin Console, se elimina inmediatamente del Dynamic Chat, ya no estará disponible para el chat en vivo o el enrutamiento de reuniones, y ya no contará con los límites de licencia.

### Rendimiento de informe de nivel de conversación mejorado {#improved-conversation-level-report-performance}

Los informes de nivel de flujo de diálogo individual y conversación ahora son más precisos y eficaces. Anteriormente, los informes de Diálogo podían tardar varios segundos en cargarse y, a veces, los datos eran incoherentes con los informes de rendimiento globales. Ahora, los informes de Diálogo individuales se cargarán en un instante y los datos siempre se alinearán con los datos de los informes globales.

CAPTURA DE PANTALLA

### Actualizaciones de permisos {#permission-updates}

Hemos limpiado la estructura de permisos y los nombres en Adobe Admin Console para que la administración de permisos sea más intuitiva.

* La categoría Administración de conversaciones ahora se denomina Conversaciones
* La categoría Reuniones ahora se denomina Actividades
* La categoría Configuración de agente ahora se denomina Agentes
* La categoría Configuración de administración ahora se llama Configuración
* Se eliminó la categoría Chat en directo y todos los permisos de chat en directo se movieron a la categoría Agentes

CAPTURA DE PANTALLA

### Compatibilidad con hipervínculos en la bandeja de entrada del agente {#support-for-hyperlinks-in-agent-inbox}

Ahora, cuando los agentes de chat en vivo comparten direcciones URL con los visitantes en el chat, esas direcciones URL estarán hipervinculadas para que los visitantes puedan simplemente hacer clic en ellos para navegar a la página, en lugar de tener que copiar y pegar la URL en su explorador.

### Introduzca el comportamiento de clave actualizado en la bandeja de entrada del agente {#enter-key-behavior-updated-in-agent-inbox}

Hemos cambiado el comportamiento de la tecla de retorno en la bandeja de entrada del agente para que al pulsar la tecla Intro o Retorno se envíe el mensaje y al pulsar Mayús+Intro se cree un salto de línea.

CAPTURA DE PANTALLA

### Página de operación por turnos eliminada {#round-robin-page-removed}

¡No te preocupes! El enrutamiento de operación por turnos sigue siendo completamente funcional y funciona del mismo modo que siempre lo ha hecho. Acabamos de eliminar la página que mostraba una lista de agentes a menudo inexacta y su orden en la cola de enrutamiento round robin.

Para proporcionar cierto contexto, cuando lanzamos Dynamic Chat en 2022, no había compatibilidad con el chat en vivo, solo con las reservas de reuniones y la página de enrutamiento round robin se diseñó solo con las reservas de reuniones en mente. Con la introducción del chat en vivo el año pasado, la página round robin se volvió obsoleta porque no reflejaba con precisión la naturaleza más compleja del enrutamiento round robin entre agentes con permisos tanto de reservación de reuniones como de chat en vivo. Exploramos algunas opciones diferentes para resolver esto, pero finalmente decidimos que eliminarlo por completo era la mejor opción para minimizar la confusión.

## Versión de febrero {#february-release}

**Fecha de publicación: 22 de febrero de 2024**

### Página Conversaciones {#conversations-page}

La nueva página Conversaciones le ofrece una ventanilla única para ver las transcripciones de todas las conversaciones (automatizadas y en directo) que se produjeron para su instancia, tanto de posibles clientes conocidos como anónimos, lo que le proporciona una mejor visibilidad sobre cómo sus clientes interactúan con sus diálogos, flujos de conversación y agentes en directo.

CAPTURA DE PANTALLA

El intervalo de fechas en el panel global aumentó de 90 días a 24 meses

Tú preguntaste y nosotros lo hicimos. Ahora puede ver datos de participación del Dynamic Chat de hasta dos años en todos los paneles de análisis.

### Ramificación condicional en cuadros de diálogo {#conditional-branching-in-dialogues}

La ramificación condicional permite crear ramas en los flujos de diálogo en función de diferentes condiciones. Ahora puede presentar contenido diferente a distintas personas en el mismo cuadro de diálogo en función de los atributos del posible cliente y de la empresa en Marketo.

## Versión de enero {#january-release}

**Fecha de la versión: 24 de enero de 2024**

### Configuración del límite de chat en directo simultáneo en la administración de agentes {#Concurrent-live-chat-limit-setting}

De forma predeterminada, cada agente de chat en vivo de su instancia puede participar en un máximo de 5 sesiones de chat en vivo a la vez. Hemos introducido una nueva configuración en la administración de agentes que le permite ajustar este límite de 1 a 10.

CAPTURA DE PANTALLA
