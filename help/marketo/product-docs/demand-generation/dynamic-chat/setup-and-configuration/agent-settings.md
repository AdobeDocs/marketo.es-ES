---
description: Configuración del agente - Documentos de Marketo - Documentación del producto
title: Configuración del agente
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
source-git-commit: 8cc63658ddd0e5b6343dc690d4009d4466250998
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 1%

---

# Configuración del agente {#agent-settings}

Configure su calendario y establezca la disponibilidad de la reunión/chat en vivo.

>[!PREREQUISITES]
>
>Asegúrese de que se hayan concedido a sus agentes los [permisos](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} adecuados.

![](assets/agent-settings-1.png)

## Conectar calendario {#connect-calendar}

En la pestaña de configuración del Calendario, conecte el calendario de Outlook o Gmail para utilizarlo en la programación de citas en el bot de chat.

![](assets/agent-settings-2.png)

Una vez que el calendario de un usuario está conectado a Dynamic Chat, se agrega a la cola y el calendario estará disponible para que los visitantes del sitio web programen citas en.

>[!NOTE]
>
>Puede conectar un calendario por usuario. Si desea recibir reuniones en varios calendarios, debe agregar varios usuarios y hacer que cada uno conecte sus calendarios.

Los usuarios también pueden personalizar el cuerpo de la invitación que se envía al visitante cuando este programa una cita en el calendario del usuario. También pueden seleccionar la casilla de verificación de la parte inferior para incluir un vínculo de Google Meet o Microsoft Teams (según el calendario conectado).

![](assets/agent-settings-3.png)

>[!TIP]
>
>Utilice el icono de token (llaves) para personalizar los correos electrónicos de confirmación de reserva de la reunión con atributos de persona o compañía.

### Permisos {#permissions}

La configuración con Outlook concede los siguientes permisos a Dynamic Chat:

* Acceso completo a sus calendarios
* Inicie sesión y lea su perfil
* Mantener el acceso a los datos a los que le ha dado acceso
* Leer la configuración del buzón

La configuración con Google concede los siguientes permisos a Dynamic Chat:

* Crear, cambiar o eliminar calendarios
* Actualización de eventos de calendario individuales
* Cambiar la configuración, incluso quién puede ver los eventos
* Cambiar con quién se comparte el calendario
* Acceso a su nombre, dirección de correo electrónico, preferencia de idioma e imagen de perfil

## Disponibilidad de reserva de reunión {#meeting-booking-availability}

Establezca su zona horaria y la disponibilidad de hora/día de la semana para recibir las reservas de la reunión.

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Duración de la reunión</b></td>
   <td>Determina la cantidad de tiempo que los visitantes verán en las ranuras de reunión disponibles.</td>
  </tr> 
  <tr> 
   <td><b>Tiempo de espera entre reuniones</b></td>
   <td>Cantidad de tiempo que se establece como búfer para después de la reunión. Si lo establece para 30 minutos, nadie podrá reservar una reunión con usted hasta 30 minutos después del final programado de una reunión en su calendario.</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>Puede seleccionar varios bloques de tiempo en el mismo día (por ejemplo, viernes de 8 a 12 p _y_ de 1 p. a 5 p.) haciendo clic en el signo **+** que aparece a la derecha.

## Disponibilidad de chat en vivo {#live-chat-availability}

Establece tu zona horaria y disponibilidad de hora/día de la semana para recibir chats en vivo.

![](assets/agent-settings-5.png)

Si ha iniciado sesión en la aplicación, recibirá una notificación dentro de la aplicación de un chat entrante. Si no has iniciado sesión, recibirás una notificación en el navegador (si has [configurado eso](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}).

>[!IMPORTANT]
>
>* La opción de [disponibilidad](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} en la bandeja de entrada del agente **anulará** lo que se ha introducido en la pestaña _Disponibilidad del chat en vivo_. Por lo tanto, si el agente está programado como disponible de 1p a 5p pero necesita tomarse un descanso rápido a 3p, no es necesario que modifique la configuración de su agente. El estado de cambio de disponibilidad permanecerá hasta que se cambie manualmente, hasta que se alcance el siguiente bloque de tiempo de disponibilidad del agente o hasta la medianoche del huso horario especificado por el agente (consulte la siguiente viñeta para obtener más información).
>
>* Cuando el agente utiliza el conmutador de disponibilidad para cambiar su estado a &quot;disponible&quot;, su estado se restablece automáticamente (cambia a no disponible) a medianoche del huso horario especificado en su programación de disponibilidad. Si no se especifica ninguna zona horaria, el valor predeterminado es UTC (hora universal coordinada).

>[!TIP]
>
>Puede seleccionar varios bloques de tiempo en el mismo día (por ejemplo, viernes de 8 a 12 p _y_ de 1 p. a 5 p.) haciendo clic en el signo **+** que aparece a la derecha.

## Fotografía del perfil del agente

Aunque un agente tiene la capacidad de cargar su propia fotografía de perfil, esa acción no se realiza en Dynamic Chat. Tendrían que navegar a `account.adobe.com/profile`. Obtenga más información aquí: [Actualice el perfil de su cuenta](https://helpx.adobe.com/es/manage-account/using/edit-adobe-account-personal-profile.html).

>[!NOTE]
>
>La imagen de perfil que se muestra en `experience.adobe.com` es **no** compatible.
