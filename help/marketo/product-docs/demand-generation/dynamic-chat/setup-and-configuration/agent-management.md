---
description: Obtenga información sobre la administración de agentes en Dynamic Chat. Vea agentes, administre equipos, establezca reglas de reserva y controle cómo se asignan las reuniones y el chat en vivo.
title: Gestión de agentes
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
TQID: 'https://experienceleague.adobe.com/WZgOsCc5-8oEKLPhj6ziYMIhrYKHxHjrqhLp73mirSU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 4%
---
# Gestión de agentes {#agent-management}

En la administración de agentes, vea una lista de agentes en la instancia de Dynamic Chat, administre equipos y establezca reglas de reserva.

![](assets/agent-management-1.png)

## Agentes {#agents}

Esta pestaña enumera todos los agentes de la instancia de Dynamic Chat e incluye información como el nombre, la dirección de correo electrónico, el estado del chat en vivo y más.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Si un agente agregado recientemente no aparece aquí, podrían pasar hasta dos horas después de agregarlo en la Admin Console de Adobe.

## Equipos {#teams}

Los administradores pueden crear equipos de agentes para facilitar el envío a grupos específicos de agentes de ventas.

>[!AVAILABILITY]
>
>El acceso a los equipos requiere una suscripción a Dynamic Chat Prime. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

![](assets/agent-management-3.png)

### Crear un equipo {#create-a-team}

1. Haga clic en **+ Crear equipo**.

   ![](assets/agent-management-4.png)

1. Dé un nombre a su equipo.

   ![](assets/agent-management-5.png)

1. Haga clic en el menú desplegable **Agregar agentes** y seleccione los agentes que desee.

   ![](assets/agent-management-6.png)

1. Haga clic en **Crear**.

   ![](assets/agent-management-7.png)

## Reglas de reserva {#fallback-rules}

### Reunión alternativa {#meeting-fallback}

Seleccione un mensaje estándar (del sistema) o escriba uno personalizado para que los visitantes vean cuándo no está disponible la reserva de la reunión.

![](assets/agent-management-8.png)

### Live Chat Fallback {#live-chat-fallback}

Seleccione un mensaje estándar (del sistema) o escriba uno personalizado para que los visitantes vean cuándo Live Chat no está disponible.

![](assets/agent-management-9.png)

>[!NOTE]
>
>* Si selecciona la casilla de verificación _Incluir opción de reserva de reunión_, el visitante del chat tendrá la opción de reservar una reunión cuando no haya agentes disponibles para el chat en vivo.
>
>* **Para cualquier regla o equipo personalizado como una tarjeta de Live Chat**: Al comprobar si hay agentes, si no están disponibles o no se pudieron conectar, volverá a Round Robin para intentar encontrar &quot;agentes disponibles&quot; (todos los que están disponibles en ese momento, independientemente de la lógica o regla de enrutamiento que se haya colocado en el flujo).

>[!TIP]
>
>Al crear un mensaje personalizado, puede aplicar estilo a la fuente, utilizar vínculos e incluso insertar emojis.

## Configuración {#settings}

### Límite de chats en directo simultáneos {#concurrent-live-chat}

Establece el número de chats activos simultáneos que un agente puede tomar al mismo tiempo. Puede establecer entre 1 y 10.

![](assets/agent-management-10.png)

### Límite de tiempo de espera del visitante {#visitor-wait-time}

Controle la cantidad máxima de tiempo que un visitante esperará (en segundos) para conectarse a un agente activo antes de que el visitante reciba un mensaje de reserva. Puede ajustarse entre 10 y 500 segundos.

![](assets/agent-management-11.png)
