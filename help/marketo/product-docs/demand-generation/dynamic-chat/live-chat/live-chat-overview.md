---
description: Información general de Live Chat - Documentos de Marketo - Documentación del producto
title: Información general de Live Chat
feature: Dynamic Chat
exl-id: f6563e73-4b6e-437d-bf8b-ec72a9b8bcb3
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# Información general de Live Chat {#live-chat-overview}

El chat en vivo permite a los visitantes del sitio web entablar conversaciones de chat en tiempo real con sus agentes de ventas.

## Añadir agentes de chat en directo {#add-live-chat-agents}

Para comenzar con el chat en vivo, tendrás que agregar tus agentes de chat en vivo como [usuarios en Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Una vez hecho esto, puede agregar una [tarjeta de chat en vivo](#using-the-live-chat-card) a un cuadro de diálogo nuevo o existente.

Cuando los visitantes soliciten hablar con un agente a través de su cuadro de diálogo, los agentes tendrán varios [opciones de notificación](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} donde pueden comenzar a chatear con el visitante.

## Uso de la tarjeta de chat en directo {#using-the-live-chat-card}

Utilice la tarjeta de chat en vivo en el [Diseñador de secuencias](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} cuando desee que los visitantes charlen con un agente activo.

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
   <td>Todas las reglas personalizadas se someterán al ciclo cuando se considere hacia dónde dirigir al visitante. Si el visitante no cumple los requisitos para ninguna regla personalizada, obtiene el <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">mensaje de reserva de chat en vivo</a>.</td>
  </tr> 
  <tr> 
   <td><b>Equipo</b></td>
   <td>Elija un equipo específico para recibir el chat. Si se elige esta opción, se le asigna round robin dentro de ese equipo.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Bandeja de entrada del agente](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
