---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 5dbc3add8acaae02f25c1f9b9ae39ecfc1aaf259
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 3%

---

# Notas de la versión de Dynamic Chat {#dynamic-chat-release}

Las versiones de Adobe Dynamic Chat funcionan con un modelo de entrega continua que permite un enfoque más escalable de la implementación de funcionalidades. A veces hay varias versiones en un mes, por lo que vuelva a consultar regularmente la información más actualizada.

La página de notas de la versión estándar de Marketo Engage [ se encuentra aquí](/help/marketo/release-notes/current.md){target="_blank"}.

## Lanzamiento de junio de 2025 {#june-2025-release}

### Renovación de lógica de enrutamiento {#routing-logic-revamp}

Hemos rediseñado la lógica de enrutamiento de chat en vivo en Dynamic Chat para garantizar un comportamiento de participación más inteligente y predecible en todos los tipos de enrutamiento (cuenta, personalizado, equipo y Round Robin). La nueva lógica simplifica los flujos de enrutamiento y mejora la gestión de reserva cuando los agentes no están disponibles.

#### Mejoras clave en el comportamiento del enrutamiento

* **Hasta dos intentos de participación por sesión**

   * El sistema intentará conectarse con hasta dos agentes (como máximo), pero estrictamente dentro de la regla de enrutamiento principal.

   * Si un agente está disponible pero no responde (por ejemplo, rechaza o pierde el chat), el sistema intentará conectarse a un agente diferente del mismo grupo.

   * La lógica de reserva (como Round Robin) solo se activa si no se encuentran agentes aptos durante la resolución inicial, para no volver a intentarlo después de un compromiso fallido.

* **Comportamiento específico de regla de enrutamiento**

_&#x200B;**Enrutamiento de cuenta**&#x200B;_

Si el dominio de correo electrónico de un visitante se asigna a una cuenta conocida, siempre se da prioridad al agente asignado.

Si el agente está disponible, el chat se dirige a ellos directamente.

Si el agente no está disponible, el sistema:

* No intenta otro agente, incluso si Round Robin está habilitado como reserva.

* En su lugar:

   * Muestra el calendario de reuniones del agente asignado (si está activado).
-o-
   * Vuelve a un mensaje predeterminado (el peor caso).

La regla de enrutamiento a nivel de tarjeta (por ejemplo, Equipo o Personalizado) solo se tiene en cuenta si el enrutamiento de cuentas no es elegible (no hay dominio o agente coincidente).

_&#x200B;**Enrutamiento personalizado/de equipo**&#x200B;_

Estas reglas pueden devolver varios agentes aptos.

Si el primer agente disponible no interactúa, el sistema probará con otro agente de la misma lista.

La reserva de Round Robin no se activa solo porque un agente no responda.

Si ninguno de los agentes interactúa:

* El sistema muestra el calendario del primer agente probado (si está activado).
-o-
* Muestra el mensaje de reserva predeterminado.

_&#x200B;**Enrutamiento Round Robin**&#x200B;_

Cuando se utiliza como regla de enrutamiento principal, el sistema:

* Intenta atraer al primer agente disponible del grupo round robin.

* Si el primer agente no responde, vuelve a intentarlo con el siguiente mejor agente apto.

Si se utiliza el Round Robin como alternativa, solo se activa si no se resuelve ningún agente a partir de la regla principal.

_&#x200B;**Flujo de experiencia del visitante**&#x200B;_

El sistema comprueba si se aplica el enrutamiento de cuentas.

* Si sí y el agente está disponible, se conecta inmediatamente.

* Si el agente no cumple los requisitos o no está disponible, continúa con la regla de enrutamiento a nivel de tarjeta.

Se evalúa la regla de enrutamiento de nivel de tarjeta (personalizado, por equipo o por turnos).

* Se comprueba la disponibilidad de los agentes aptos (permisos, estado).

* El sistema involucra a un agente y, si es necesario, intenta un segundo agente desde la misma regla.

* Si ninguna participación tiene éxito, se aplica la lógica de reserva:

   * reserva de calendario (si está activada),
-o-
   * Mensaje predeterminado.

La reserva de Round Robin solo se considera cuando no se encuentran agentes aptos de la regla de enrutamiento principal, no cuando los agentes individuales no responden.

##### Casos de uso {#use-cases}

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
    <td>Alternativa (Round Robin)</td>
    <td>El agente asignado no está disponible, la opción de reserva de Round Robin está activada</td>
    <td>El sistema selecciona un agente disponible mediante Round Robin y lo involucra </td>
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
    <td>Alternativa (Round Robin)</td>
    <td>La regla personalizada no resuelve ningún agente, la opción de reserva de Round Robin está activada.</td>
    <td>El sistema selecciona un agente disponible mediante Round Robin y lo involucra.</td>
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
    <td>El equipo incluye agentes con chat en vivo; el primer agente disponible acepta el chat.</td>
    <td>El chat se conecta a ese agente.</td>
  </tr>
  <tr>
    <td>Alternativa (Round Robin)</td>
    <td>No hay ningún agente de equipo disponible y la opción de reserva de Round Robin está activada.</td>
    <td>El sistema selecciona y se conecta con un agente del grupo Round Robin.</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>Hay dos agentes disponibles, pero ninguno de los dos interactúa; reserva de calendario habilitada.</td>
    <td>Se muestra el calendario del primer agente probado o se activa un mensaje de reserva.</td>
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
    <td>Alternativa (Round Robin)</td>
    <td>No hay agentes disponibles en el grupo Round Robin; el calendario de reuniones está habilitado.</td>
    <td>El calendario se muestra para el primer agente en la lista (si está configurado) o se muestra un mensaje de reserva.</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>No hay agentes disponibles; la reserva está desactivada.</td>
    <td>Se muestra un mensaje de reserva estático al visitante.</td>
  </tr>
</tbody></table>

### Notificación de impulso {#pulse-notification}

Cada vez que un visitante solicita conectarse con un agente, le proporcionamos una notificación interna de la aplicación y del explorador. Pero a veces, los agentes se pierden estas charlas.

Con esta versión, el agente activo puede recibir un correo electrónico, Slack, en la aplicación y una notificación del explorador cuando un visitante nuevo está interesado en chatear.

1. En la página de inicio de Adobe Experience Cloud, haga clic en el icono Cuenta y seleccione **Preferencias**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Desplácese hacia abajo hasta _Notificaciones_ y realice las selecciones de Dynamic Chat que desee.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>El contenido de una notificación Pulse puede ser el mismo que el que utilizamos para las notificaciones en la aplicación y en el explorador.
