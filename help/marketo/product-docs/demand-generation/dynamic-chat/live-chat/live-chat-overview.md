---
description: Descripción general de la conversación en vivo - Marketo Docs - Documentación de productos
title: Información general del chat en vivo
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 56070990d8bcea61fbbf3b382e5abae786b2488e
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Información general del chat en vivo {#live-chat-overview}

El chat en vivo permite a los visitantes del sitio web participar en conversaciones de chat en tiempo real con sus agentes de ventas.

>[!NOTE]
>
>Los flujos conversacionales y el chat en vivo son funciones de prueba compartidas que tienen un límite de vida útil combinado de 100 participaciones para aquellos en el paquete Dynamic Chat Select. Cuando se alcanza este límite, todos los flujos conversacionales publicados dejarán de activarse y los visitantes que solicitud chatear con un agente en vivo recibirán el mensaje de reserva global. Para aumentar este límite, póngase en contacto con su representante de cuentas para discutir las opciones de actualización de paquetes.

## Añadir agentes de chat en directo {#add-live-chat-agents}

Para comenzar con el chat en vivo, tendrás que agregar tus agentes de chat en vivo como [usuarios en Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Una vez hecho esto, puede agregar una [tarjeta de chat en vivo](#using-the-live-chat-card) a un cuadro de diálogo nuevo o existente.

Cuando los visitantes soliciten hablar con un agente a través de su cuadro de diálogo, los agentes tendrán varios [opciones de notificación](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} donde pueden comenzar a chatear con el visitante.

>[!NOTE]
>
>El avatar del agente activo utiliza la imagen perfil del Adobe Systems cuenta perfil del agente. Para actualizar la imagen, siga [estos pasos](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Uso de la tarjeta de chat en vivo {#using-the-live-chat-card}

Utilice la tarjeta de chat en vivo en el [Diseñador de secuencias](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} cuando desee que los visitantes charlen con un agente activo.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>La tarjeta de chat en vivo siempre debe ser la última tarjeta de la sucursal. Si la tarjeta se coloca en un punto aleatorio de la rama, podría sorprender al visitante conectándolo de repente a un agente.

### Prácticas recomendadas {#best-practices}

* Utilice una tarjeta de preguntas antes de la tarjeta de chat en vivo preguntando al visitante si desea conectarse.
* Después de que el visitante acepte conectarse, use el tarjeta de captura de información para recopilar parte de su información, gustar nombre / apellido, dirección correo electrónico, cargo, etc. (Se recomienda al menos solicitud nombre y dirección correo electrónico).

## Tarjeta de chat en vivo Opciones {#live-chat-card-options}

Hacer clic en el tarjeta de chat en vivo en la transmisión le permite elegir cómo se enruta el visitante. Elija entre round robin, un agente, reglas personalizadas o un equipo.

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
   <td>Se recorrerán todas las reglas personalizadas cuando se considere dónde dirigir el visitante. Si el visitante no califica para ningún regla personalizado, recibe el mensaje</a> de reserva de chat <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">en vivo.</td>
  </tr> 
  <tr> 
   <td><b>Equipo</b></td>
   <td>Elija un equipo específico para recibir el chat. Si se elige esta opción, se le asigna round robin dentro de ese equipo.</td>
  </tr>
 </tbody> 
</table>

## Notificaciones de chat en directo {#live-chat-notifications}

>[!IMPORTANT]
>
>Para recibir notificaciones del navegador para el chat en vivo, todos los agentes de chat en vivo deben activar notificaciones del navegador para el Dynamic Chat cuando se le solicite.

### Activación de notificaciones {#enabling-notifications}

Los agentes de chat en vivo verán un banner en la parte superior de la pantalla cuando inicien sesión que dice &quot;Habilite las notificaciones de explorador para recibir notificaciones de chat en vivo&quot;. Haga clic en **Habilitar**.

![](assets/live-chat-overview-4.png)

El navegador solicitará a los agentes de chat en vivo que muestren notificaciones. Clic **Permitir**.

![](assets/live-chat-overview-5.png)

Si los agentes no reciben notificaciones del explorador incluso después de permitirlas, es posible que tengan que habilitar las notificaciones para el explorador en la configuración de notificaciones del sistema operativo:

[Pasos para Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Pasos para Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### Cuando un chat en vivo se enruta a un agente {#when-a-live-chat-is-routed-to-an-agent}

Cuando un chat en vivo se dirige a un agente, verán un banner azul en la parte superior de la pantalla pidiéndoles que acepten.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>También tiene la opción de configurar explorador notificaciones, que le alerta en caso de que no haya iniciado sesión en Dynamic Chat.
>
>* Habilitar notificaciones explorador en [Google Cromo](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Activar notificaciones explorador en [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### Cosas a tener en cuenta {#things-to-note}

* Los agentes tienen 45 segundos para responder antes de que se agote el tiempo de espera del mensaje &quot;Aceptar chat&quot;. Después, los visitantes recibirán la [mensaje de reserva](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. Para suscriptores de Dynamic Chat Prime que tienen la opción de enrutamiento configurada como **Equipo**, se intentará con un agente más antes de que aparezca el mensaje de reserva.
* Hay un límite de 10 chats en vivo por agente en este momento.

>[!MORELIKETHIS]
>
>[Bandeja de entrada del agente](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
