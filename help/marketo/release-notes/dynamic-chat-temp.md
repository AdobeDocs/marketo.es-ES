---
description: 'Notas de la versión actuales, documentos de Marketo: documentación del producto'
title: Notas de la versión de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: ce7142e471271dfb33b265e226b67bcc3b35594b
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# Notas de la versión de Dynamic Chat {#dynamic-chat-release}

Las versiones de Adobe Dynamic Chat funcionan con un modelo de entrega continua que permite un enfoque más escalable de la implementación de funcionalidades. A veces hay varias versiones en un mes, por lo que vuelva a consultar regularmente la información más actualizada.

La página de notas de la versión estándar de Marketo Engage [ se encuentra aquí](/help/marketo/release-notes/current.md){target="_blank"}.

## Lanzamiento de junio de 2025 {#june-25-release}

### Renovación de lógica de enrutamiento {#routing-logic-revamp}

Hemos rediseñado la lógica de enrutamiento de chat en vivo en Dynamic Chat para garantizar un comportamiento de participación más inteligente y predecible en todos los tipos de enrutamiento (cuenta, personalizado, equipo y Round Robin). La nueva lógica simplifica los flujos de enrutamiento y mejora la gestión de reserva cuando los agentes no están disponibles.

#### Mejoras clave en el comportamiento del enrutamiento

* **Hasta dos intentos de participación por sesión**

   * El sistema intentará conectarse con al menos dos agentes, pero estrictamente dentro de la regla de enrutamiento principal.

   * Si hay un agente disponible pero no responde (por ejemplo, rechaza o falla), el sistema intentará un segundo agente del mismo grupo.

   * La lógica de reserva (como Round Robin) solo se activa si no se encuentran agentes aptos durante la resolución inicial, para no volver a intentarlo después de un compromiso fallido.

* **Comportamiento específico de regla de enrutamiento**

_**Enrutamiento de cuenta**_

Si el dominio de correo electrónico de un visitante se asigna a una cuenta conocida, siempre se da prioridad al agente asignado.

Si el agente está disponible, el chat se dirige a ellos directamente.

Si el agente no está disponible, el sistema:

No intenta otro agente, incluso si Round Robin está habilitado como reserva.

En su lugar:

Muestra el calendario de reuniones del agente asignado (si está activado), o

Vuelve a un mensaje predeterminado (el peor caso).

La regla de enrutamiento a nivel de tarjeta (por ejemplo, Equipo o Personalizado) solo se tiene en cuenta si el enrutamiento de cuentas no es elegible (no hay dominio o agente coincidente).

_**Enrutamiento personalizado/de equipo**_

Estas reglas pueden devolver varios agentes aptos.

Si el primer agente disponible no interactúa, el sistema probará con otro agente de la misma lista.

La reserva de Round Robin no se activa solo porque un agente no haya respondido.

Si ninguno de los agentes interactúa:

El sistema muestra el calendario del primer agente probado (si está activado), o

Muestra el mensaje de reserva predeterminado.

_**Enrutamiento Round Robin**_

Cuando se utiliza como regla de enrutamiento principal, el sistema:

Intenta atraer al primer agente disponible del grupo round robin.

Si el primero no responde, vuelve a intentarlo con el siguiente mejor agente apto.

Si se utiliza el Round Robin como alternativa, solo se activa si no se resuelve ningún agente a partir de la regla principal.

**Flujo de experiencia del visitante**

El sistema comprueba si se aplica el enrutamiento de cuentas.

Si sí y el agente está disponible, → conecta inmediatamente.

Si no cumple los requisitos o el agente no está disponible, → continúa con la regla de enrutamiento a nivel de tarjeta.

Se evalúa la regla de enrutamiento de nivel de tarjeta (personalizado, por equipo o por turnos).

Se comprueba la disponibilidad de los agentes aptos (permisos, estado).

El sistema involucra a un agente y, si es necesario, intenta un segundo agente desde la misma regla.

Si ninguna participación se realiza correctamente → se aplica la lógica de reserva:

reserva de calendario (si está activada), o

Mensaje predeterminado.

La reserva de Round Robin solo se considera cuando no se encuentran agentes aptos de la regla de enrutamiento principal, no cuando los agentes individuales no responden.

**Casos de uso**

Enrutamiento de cuenta

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

Enrutamiento personalizado

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Alternativa (Round Robin)</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
</tbody></table>

Enrutamiento de equipo

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Alternativa (Round Robin)</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
</tbody></table>

Enrutamiento Round Robin

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Ejemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Alternativa (Round Robin)</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>No hay agente de reserva</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
</tbody></table>

### Notificación de impulso {#pulse-notification}

Siempre que un visitante solicita conectarse con un agente, hoy le proporcionamos una notificación en la aplicación y en el navegador, pero los agentes a menudo no pueden ver estos chats.

* Ahora el agente activo recibirá un correo electrónico, Slack, Inapp, una notificación del explorador cuando un visitante nuevo esté interesado en chatear

* El contenido de las notificaciones Pulse puede ser el mismo que el que utilizamos hoy para las notificaciones en la aplicación y en el explorador

El comportamiento debe ser el mismo que el actual para que el agente acepte cuando varios agentes lo acepten.
