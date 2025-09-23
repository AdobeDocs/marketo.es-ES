---
description: Administración de agentes - Documentos de Marketo - Documentación del producto
title: Gestión de agentes
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# Gestión de agentes {#agent-management}

En la administración de agentes, vea una lista de agentes en la instancia de Dynamic Chat, administre equipos y establezca reglas de reserva.

![](assets/agent-management-1.png)

## Agentes {#agents}

Esta pestaña enumera todos los agentes de la instancia de Dynamic Chat e incluye información como el nombre, la dirección de correo electrónico, el estado del chat en vivo y más.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>¿No ve un agente que _acaba de_ agregar? Pueden tardar hasta dos horas en aparecer aquí después de agregarlas en la Admin Console de Adobe.

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
>Al crear un mensaje personalizado, puede aplicar estilo a la fuente, utilizar vínculos e incluso insertar emojis. `:)`
