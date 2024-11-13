---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 7fbfdc6d34d2f1174e921464d64689b0c5687914
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 3%

---

# Notas de la versión de Dynamic Chat TEMP {#dynamic-chat-release}

## Versión de septiembre/octubre de 2024 {#august-release}

### Análisis de chat en vivo mejorado {#enhanced-live-chat-analytics}

Se han realizado varias mejoras en el panel de Analytics, entre las que se incluyen:

* Número total solicitado de chats en directo: número de visitantes solicitados para un &quot;chat con el agente&quot;

* Total de chat en directo conectado: número de visitantes conectados frente al total solicitado para un &quot;chat con el agente&quot;

* Total de solicitudes de chat en vivo perdidas: número de visitantes desatendidos frente al total solicitado para un &quot;chat con el agente&quot;

* Duración media del chat en minutos: Analice la &quot;duración media del chat&quot; entre los visitantes y sus agentes.

* Tiempo medio de respuesta del agente en segundos: Analice el &quot;tiempo medio empleado&quot; por los agentes para responder a sus preguntas y respuestas en directo en el chat

* Tablero diario: las solicitudes de chat en vivo se conectan correctamente, las solicitudes de chat en vivo se pierden, ordenan y filtran las actividades de chat en vivo recientes

CAPTURA DE PANTALLA

### Puntuación de conversación {#conversation-scoring}

Cuantifique los posibles clientes en función de la calidad de su interacción de chat y utilice esa métrica como Déclencheur/filtro en campañas inteligentes de Marketo Engage. Use el nuevo atributo _puntuación de conversación_ en las siguientes actividades:

* Participa en un diálogo
* Interactúe con un flujo de conversación
* Interacción con un agente

**Aspectos a tener en cuenta:**

* El valor de la puntuación estará entre 0, 1, 2 y 3 (el valor predeterminado es nulo)

* Una vez finalizada o eliminada la conversación, en la actividad guarde el valor de la puntuación y publique que que no se pueda editar????? (qué significa esta frase)

* Configurar una puntuación:

   * En la bandeja de entrada del agente: durante una conversación en directo, el agente puede actualizar o establecer una puntuación para la conversación, que se almacena en la actividad de conversación

   * En el diseñador de secuencias: en la tarjeta de objetivos, el usuario puede actualizar o establecer una puntuación para la conversación

CAPTURA DE PANTALLA

CAPTURA DE PANTALLA

CAPTURA DE PANTALLA

### Nueva lógica de creación de posibles clientes {#new-lead-creation-logic}

Si un posible cliente rellena un formulario con el correo electrónico `abc@test.com` y está cookie como xyz, más adelante rellena el mismo formulario con el correo electrónico `def@test.com`, se crea un nuevo posible cliente, pero la cookie xyz se asocia al nuevo posible cliente y se elimina del mismo `abc@test.com`.

A partir de ese momento, `abc@test.com` será un posible cliente sin cookie. POSIBLE CLIENTE ANÓNIMO??

Por lo tanto, cuando un visitante con cookie abc aterriza en una página y proporciona un ID de correo electrónico como `abc@p.com`:

TABLA

### Tiempo de carga de flujo de conversación optimizado {#optimized-conversation-flow-load-time}

Para mejorar la experiencia del usuario, ahora se muestra un cargador de reflejos en lugar de un espacio en blanco mientras se carga el flujo de conversación. CONVERSACIÓN O CONVERSACIÓN???

**Antes de**

GIF

**Después**

GIF

### Opción para heredar la fuente {#option-to-inherit-font}

Ahora puede permitir que el bot de chat herede directamente la fuente de la página web en la que se aloja en lugar de administrar la fuente de la marca en Dynamic Chat. Al habilitar esta opción, el bot de chat tomará la fuente definida en la etiqueta `<body>` de la página.

CAPTURA DE PANTALLA

### Integración de Demandbase con Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Los usuarios de Demandbase pueden traer su propia licencia de Demandbase y activar la integración. Utilice los atributos de persona de Demandbase para la segmentación de diálogos, la promoción condicional de la marca y el enrutamiento personalizado.

La resolución de estos valores de atributos con un posible cliente se realizaría en tiempo real y se almacenaría en el perfil del posible cliente correspondiente.
