---
description: 'Información general sobre Dynamic Chat: Documentos de Marketo: Documentación del producto'
title: Información general de conversación dinámica
hide: true
hidefromtoc: true
source-git-commit: afc7c8352b4470bfc367f3d16836fb14d55b8821
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Información general de conversación dinámica {#dynamic-chat-overview}

La conversación dinámica le permite aprovechar una interfaz fácil de usar para dirigirse a ambos posibles clientes (¿PERSONAS?) y cuentas en su (VISITANDO SU?) sitio web. Recopile contenido relevante, como su nombre, información de contacto y texto libre. Los visitantes del sitio también pueden reservar reuniones con su equipo de ventas. Los datos de participación y actividad de chat dinámico se pueden utilizar para agregar miembros a programas de Marketo y actividades de canales cruzados de déclencheur.

>[!NOTE]
>
>La conversación dinámica está en proceso de ser desarrollada gradualmente, con todas las suscripciones a la primavera de 2022. Para obtener más información, póngase en contacto con el administrador de éxito de los clientes.

## Integraciones {#integrations}

Un componente clave de la conversación dinámica es su capacidad para interactuar de forma nativa con su suscripción a Marketo. Para aprovechar todas las capacidades de esta integración, primero deberá iniciar la sincronización de datos. Según el tamaño de la base de datos de Marketo, los datos de la sincronización inicial [única](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) pueden tardar hasta 24 horas en completarse. El tiempo promedio de sincronización es inferior a dos horas.

Se sincroniza lo siguiente:

* Datos de campo de posible cliente
* Datos de campo de la empresa
* Datos de actividad

## Cuadros de diálogo {#dialogues}

Los cuadros de diálogo representan una sola participación en el chat. Piense en ello como un contenedor con todas las cosas que necesita para tener un diálogo de chat atractivo para los visitantes de su sitio web. En cada cuadro de diálogo, puede especificar en qué páginas desea que aparezca el cuadro de diálogo, a quién desea que se muestre, y el contenido y el flujo del propio cuadro de diálogo. Además, puede encontrar métricas para ver el rendimiento del cuadro de diálogo. [Obtenga más información sobre los cuadros de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configuración {#configuration}

En la pestaña Configuración , personalice el aspecto de los distintos cuadros de diálogo. Cambie la fuente, los colores, el tiempo de respuesta y mucho más. [Obtenga más información sobre Configuración](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Calendario {#calendar}

En la ficha Calendario, conecte el calendario (Outlook o Gmail) para utilizarlo en la programación de citas en el bot de conversación. Una vez que el calendario de un usuario esté conectado a Dynamic Chat, ese usuario se agregará a la cola y su calendario estará disponible para que los visitantes del sitio web programen las citas.

¿También puede personalizar el cuerpo del mensaje de correo electrónico de invitación? que se envía al visitante cuando programa una cita en el calendario del usuario.

## Reuniones {#meetings}

Aquí es donde verá todas las citas que han programado los visitantes del sitio web a través de sus distintos diálogos. Aquí encontrará la dirección de correo electrónico del posible cliente que reservó la cita, con qué agente reservaron la cita, cuándo está programada la cita y si la reunión ha tenido lugar o no.

## Enrutamiento {#routing}

Aquí es donde puede ver una lista de todos los agentes que han conectado sus calendarios, así como el orden en que se presentarán a los visitantes del sitio web Las reuniones van por turnos estilo, así que si tiene cinco agentes y el agente tres tomó la última reunión, el agente cuatro obtendrá la siguiente, seguido de cinco, y después volverá al agente uno.

## Preguntas frecuentes {#faq}

**¿La conversación dinámica permite el chat en directo?**

No, solo utiliza respuestas predeterminadas.

**¿Cómo puedo orientarme hacia los posibles clientes anónimos?**

En el cuadro de diálogo, debe utilizar el atributo _Lead Email is Empty_ .

**¿Admite la funcionalidad AI/NLP?**

No se admite la funcionalidad AI/NLP.

**¿Durante cuánto tiempo se almacenan los datos para los informes?**

90 días.

**¿Ofrece Dynamic Chat algún idioma además del inglés?**

En este momento no.
