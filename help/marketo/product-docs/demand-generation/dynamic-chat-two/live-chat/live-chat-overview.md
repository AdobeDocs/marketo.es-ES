---
description: Información general de Live Chat - Documentos de Marketo - Documentación del producto
title: Información general de Live Chat
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: a4fe70e1a95ff382499800049f161d1ad7dec7ab
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 2%

---

# Información general de Live Chat {#live-chat-overview}

Utilice la tarjeta de chat en vivo en el [Diseñador de secuencias](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/stream-designer.md){target="_blank"} cuando desee que los visitantes charlen con un agente activo.

## Uso de la tarjeta de chat en directo {#using-the-live-chat-card}

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>La tarjeta de chat en vivo siempre debe ser la última tarjeta de la sucursal. Si la tarjeta se coloca en un punto aleatorio de la rama, podría sorprender al visitante conectándolo de repente a un agente.

### Prácticas recomendadas {#best-practices}

* Utilice una tarjeta de preguntas antes de la tarjeta de chat en vivo preguntando al visitante si desea conectarse.
* Una vez que el visitante acepte conectarse, utilice la tarjeta de captura de información para recopilar parte de su información, como nombre/apellido, dirección de correo electrónico, cargo, etc. (se recomienda solicitar al menos el nombre y la dirección de correo electrónico).

## Opciones de tarjeta de chat en vivo {#live-chat-card-options}

Hacer clic en la tarjeta de chat en vivo en el flujo le permite elegir cómo se dirige al visitante. Elija entre round robin, un agente, reglas personalizadas o un equipo.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round Robin</b></td>
   <td>Los chats se asignan a los agentes en orden secuencial.</td>
  </tr> 
  <tr> 
   <td><b>Agente</b></td>
   <td>Elija un agente específico para recibir el chat.</td>
  </tr>
    <tr> 
   <td><b>Reglas personalizadas</b></td>
   <td>Todas las reglas personalizadas se someterán al ciclo cuando se considere hacia dónde dirigir al visitante. Si el visitante no cumple los requisitos para ninguna regla personalizada, obtiene el <a href="/help/marketo/product-docs/demand-generation/dynamic-chat-two/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">mensaje de reserva de chat en vivo</a>.</td>
  </tr> 
  <tr> 
   <td><b>Equipo</b></td>
   <td>Elija un equipo específico para recibir el chat. Si se elige esta opción, se le asigna round robin dentro de ese equipo.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Bandeja de entrada del agente](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}
