---
description: Funciones de devolución de llamada - Documentos de Marketo - Documentación del producto
title: Funciones de devolución de llamada
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: f355022fb7e6f733bb7485229e395b0fe1a9818f
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 7%

---

# Funciones de devolución de llamada {#callback-functions}

Puede utilizar las funciones de devolución de llamada de widget de Dynamic Chat para enviar eventos de conversación a cualquier plataforma de terceros.

## Introducción {#getting-started}

Este evento indica que el widget de Dynamic Chat está listo para usarse y se activa cuando se cargan en la página web todos los scripts relacionados con Dynamic Chat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
}); 
```

## Eventos de conversación {#conversation-events}

Estos eventos están relacionados con una conversación dirigida a una página específica de un visitante específico.

### Conversación activada

Se resuelve una conversación (por ejemplo, un Diálogo) dirigida a un visitante del sitio web y se le muestra el bot de chat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // code here will execute when the chatbot is loaded for a visitor 
    }); 
});  
```

### Conversación comprometida {#conversation-engaged}

El visitante participó (por ejemplo, proporcionó su primera respuesta) con el bot de chat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when a visitor engages with the chatbot 
     }); 
}); 
```

### Conversación finalizada {#conversation-completed}

El visitante ha llegado al final de la conversación.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when a conversation is completed 
     }); 
}); 
```

### Conversación cerrada

El visitante ha cerrado la conversación antes de llegar al final.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when a conversation is closed 
    }); 
}); 
```

El parámetro `event` es un objeto con metadatos relacionados con la conversación. Puede acceder a estos metadatos si accede a `event.data`.

Estos son algunos valores de metadatos clave a los que puede acceder:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadatos</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre de la conversación</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificación de conversación</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversación (flujo de diálogo/conversación)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interfaz de usuario (emergente/bot de chat/en línea)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Identificación de la sesión</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Eventos de entrada de visitante

Estos eventos se activan cuando un visitante que participa en una conversación proporciona su información de contacto (por ejemplo, número de teléfono o dirección de correo electrónico). A continuación se muestran los eventos que entran dentro de esta categoría.

### Número de teléfono {#phone-number}

Este evento se activa cuando un visitante proporciona su número de teléfono durante la conversación.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
 // code here will execute when a visitor provides their phone number 
    }); 
});  
```

### Identificación de email {#email-id}

Este evento se activa cuando un visitante proporciona su dirección de correo electrónico durante la conversación.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
}); 
```

El parámetro `event` es un objeto con metadatos relacionados con la conversación. Puede acceder a estos metadatos si accede a `event.data`.

Estos son algunos valores de metadatos clave a los que puede acceder:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadatos</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre de la conversación</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificación de conversación</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversación (flujo de diálogo/conversación)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interfaz de usuario (emergente/bot de chat/en línea)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Identificación de la sesión</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Eventos de reserva de reuniones {#meeting-booking-events}

Estos eventos se activan cuando un visitante reserva una reunión con su representante empresarial.

A continuación se muestran los eventos que entran dentro de esta categoría.

### Reunión reservada {#meeting-booked}

Este evento se activa cuando un visitante reserva una reunión en el calendario de un agente.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
}); 
```

El parámetro `event` es un objeto con metadatos relacionados con la conversación. Puede acceder a estos metadatos si accede a `event.data`.

Estos son algunos valores de metadatos clave a los que puede acceder:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadatos</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre de la conversación</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificación de conversación</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversación (flujo de diálogo/conversación)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interfaz de usuario (emergente/bot de chat/en línea)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Identificación de la sesión</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nombre del agente</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Identificación del agente</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>Información de reunión</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Eventos de chat en directo {#live-chat-events}

Estos eventos se activan cuando un visitante se conecta con un agente activo durante su participación con el bot de chat.

A continuación se muestran los eventos que entran dentro de esta categoría.

### Chat en directo solicitado {#live-chat-requested}

Este evento se activa cuando un visitante selecciona la opción de chatear con un agente activo y se está resolviendo un agente disponible.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests a live chat 
    }); 
}); 
```

### Chat en directo iniciado {#live-chat-initiated}

Este evento se activa cuando un visitante selecciona la opción de chatear con un agente activo y un agente acepta el chat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepts the chat 
    }); 
}); 
```

### Chat en directo finalizado {#live-chat-ended}

Este evento se activa cuando finaliza una conversación entre un visitante y el agente en directo.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
}); 
```

### Tiempo de espera de chat {#live-chat-timeout}

Este evento se activa cuando se agota el tiempo de espera de una conversación de chat en directo porque el visitante deja de responder o se cae.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandons a live chat 
    }); 
}); 
```

El parámetro `event` es un objeto con metadatos relacionados con la conversación. Puede acceder a estos metadatos si accede a `event.data`.

Estos son algunos valores de metadatos clave a los que puede acceder:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadatos</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre de la conversación</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificación de conversación</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversación (flujo de diálogo/conversación)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interfaz de usuario (emergente/bot de chat/en línea)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Identificación de la sesión</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nombre del agente</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Identificación del agente</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

Si desea enviar cualquiera de estos eventos a una plataforma de análisis como Adobe Analytics o Google Analytics, debe añadir su llamada de seguimiento respectiva dentro de estos eventos de Dynamic Chat. Se parecería a algo como el ejemplo siguiente.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
}); 
```
