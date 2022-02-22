---
description: 'Información general sobre Dynamic Chat: Documentos de Marketo: Documentación del producto'
title: Información general de conversación dinámica
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Información general de conversación dinámica {#dynamic-chat-overview}

Dynamic Chat le permite aprovechar una interfaz fácil de usar para dirigirse tanto a las personas como a las cuentas que visitan su sitio web. Recopile contenido relevante, como nombre, información de contacto y texto libre. Los visitantes del sitio también pueden reservar reuniones con su equipo de ventas. Los datos de participación y actividad de chat dinámico se pueden utilizar para agregar miembros a programas de Marketo y actividades de canales cruzados de déclencheur.

>[!NOTE]
>
>El chat dinámico está en proceso de ser lanzado gradualmente y actualmente está en disponibilidad limitada. Esta página se actualizará con detalles de disponibilidad general (GA) a medida que estén disponibles.

>[!TIP]
>
>Visita [esta página](https://dcweb.z20.web.core.windows.net/) para ver vídeos de tutoriales, así como una demostración grabada de Dynamic Chat.

## Integraciones {#integrations}

Un componente clave de la conversación dinámica es su capacidad para interactuar de forma nativa con su suscripción a Marketo. Para aprovechar todas las capacidades de esta integración, primero deberá iniciar la sincronización de datos. Según el tamaño de la base de datos de Marketo, los datos iniciales pueden tardar hasta 24 horas. [sincronización única](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) para completar.

Se sincroniza lo siguiente:

* Datos de campo de persona
* Datos de campo de la empresa
* Datos de actividad

## Cuadros de diálogo {#dialogues}

Los cuadros de diálogo representan una sola participación en el chat. Piense en ello como un contenedor con todas las cosas que necesita para tener un diálogo de chat atractivo para los visitantes de su sitio web. En cada cuadro de diálogo, puede especificar en qué páginas desea que aparezca el cuadro de diálogo, a quién desea que se muestre, y el contenido y el flujo del propio cuadro de diálogo. Además, puede encontrar métricas para ver el rendimiento del cuadro de diálogo. [Más información sobre los cuadros de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configuración {#configuration}

En la pestaña Configuración , personalice el aspecto de los distintos cuadros de diálogo. Cambie la fuente, los colores, el tiempo de respuesta y mucho más. [Más información sobre la configuración](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Calendario {#calendar}

En la ficha Calendario, conecte el calendario (Outlook o Gmail) para utilizarlo en la programación de citas en el bot de conversación. Una vez que el calendario de un usuario esté conectado a Dynamic Chat, ese usuario se agregará a la cola y su calendario estará disponible para que los visitantes del sitio web programen las citas.

También puede personalizar el cuerpo de la invitación que se envía al visitante cuando programa una cita en el calendario del usuario.

## Reuniones {#meetings}

Aquí es donde verá todas las citas que han programado los visitantes del sitio web a través de sus distintos diálogos. Aquí encontrará la dirección de correo electrónico de la persona que reservó la cita, con qué agente reservaron la cita, cuándo está programada la cita y si la reunión ha tenido lugar o no.

## Enrutamiento {#routing}

Aquí es donde puede ver una lista de todos los agentes que han conectado sus calendarios, así como el orden en que se presentarán a los visitantes del sitio web. Las reuniones van por ahí al estilo de robin, así que si tienes cinco agentes y el agente tres tomó la última reunión, el agente cuatro obtendrá la siguiente, seguido del agente cinco, y luego volverá al agente uno.

## Preguntas frecuentes {#faq}

**¿La conversación dinámica permite el chat en directo?**

No, solo utiliza respuestas predeterminadas.

**¿Cómo puedo orientarme hacia personas anónimas?**

En el cuadro de diálogo, debe utilizar la variable _El correo electrónico de la persona está vacío_ atributo.

**¿Admite la funcionalidad AI/NLP?**

No se admite la funcionalidad AI/NLP.

**¿Durante cuánto tiempo se almacenan los datos para los informes?**

90 días.

**¿Ofrece Dynamic Chat algún idioma además del inglés?**

En este momento no.
