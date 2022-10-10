---
description: 'Información general sobre Dynamic Chat: Documentos de Marketo: Documentación del producto'
title: Información general de conversación dinámica
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 0ca537b46247eef1e7200180d7c1516465910dac
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 1%

---

# Información general de conversación dinámica {#dynamic-chat-overview}

Dynamic Chat le permite aprovechar una interfaz fácil de usar para dirigirse tanto a las personas como a las cuentas que visitan su sitio web. Recopile contenido relevante, como nombre, información de contacto y texto libre. Los visitantes del sitio también pueden reservar reuniones con su equipo de ventas. Los datos de participación y actividad de chat dinámico se pueden utilizar para agregar miembros a programas de Marketo y actividades de canales cruzados de déclencheur.

>[!NOTE]
>
>El chat dinámico está en proceso de ser lanzado gradualmente y actualmente está en disponibilidad limitada. Esta página se actualizará con detalles de disponibilidad general (GA) a medida que estén disponibles.

>[!TIP]
>
>Visita [esta página](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) para ver vídeos de tutoriales de Dynamic Chat.

## Integraciones {#integrations}

Un componente clave de la conversación dinámica es su capacidad para interactuar de forma nativa con su suscripción a Marketo. Para aprovechar todas las capacidades de esta integración, primero deberá iniciar la sincronización de datos. Según el tamaño de la base de datos de Marketo, los datos iniciales pueden tardar hasta 24 horas. [sincronización única](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) para completar.

Se sincroniza lo siguiente:

* Datos de campo de persona
* Datos de campo de la empresa
* Datos de actividad

## Cuadros de diálogo {#dialogues}

Los cuadros de diálogo representan una sola participación en el chat. Piense en ello como un contenedor con todas las cosas que necesita para tener un diálogo de chat atractivo para los visitantes de su sitio web. En cada cuadro de diálogo, puede especificar en qué páginas desea que aparezca el cuadro de diálogo, a quién desea que se muestre, y el contenido y el flujo del propio cuadro de diálogo. Además, puede encontrar métricas para ver el rendimiento del cuadro de diálogo. [Más información sobre los cuadros de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target=&quot;_blank&quot;}.

## Configuración {#configuration}

En la pestaña Configuración , personalice el aspecto de los distintos cuadros de diálogo. Cambie la fuente, los colores, el tiempo de respuesta y mucho más. [Más información sobre la configuración](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target=&quot;_blank&quot;}.

## Calendario {#calendar}

En la ficha Calendario, conecte el calendario (Outlook o Gmail) para utilizarlo en la programación de citas en el bot de conversación. Una vez que el calendario de un usuario esté conectado a Dynamic Chat, ese usuario se agregará a la cola y su calendario estará disponible para que los visitantes del sitio web programen las citas.

También puede personalizar el cuerpo de la invitación que se envía al visitante cuando programa una cita en el calendario del usuario.

## Reuniones {#meetings}

Aquí es donde verá todas las citas que han programado los visitantes del sitio web a través de sus distintos diálogos. Aquí encontrará la dirección de correo electrónico de la persona que reservó la cita, con qué agente reservaron la cita, cuándo está programada la cita y si la hora de reunión programada ha pasado o no.

## Enrutando {#routing}

Aquí es donde puede ver una lista de todos los agentes que han conectado sus calendarios, así como el orden en que se presentarán a los visitantes del sitio web.

## Preguntas frecuentes {#faq}

**¿Puedo instalar Dynamic Chat en cualquier lugar del sitio web de mi empresa o solo funciona en páginas de aterrizaje de Marketo?**

El fragmento de JavaScript de Dynamic Chat se puede instalar en cualquier sitio web, así como en las páginas de aterrizaje de Marketo.

**¿Durante cuánto tiempo se almacenan los datos para los informes?**

90 días (véase la lista completa de límites) [below](#limits-in-dynamic-chat)).

**¿La conversación dinámica permite el chat en directo?**

No, solo utiliza respuestas predeterminadas.

**¿Admite Dynamic Chat algún idioma aparte del inglés?**

Sí. Dynamic Chat admite los siguientes idiomas: Francés, alemán, japonés, español, italiano, portugués de Brasil, coreano, chino simplificado y chino tradicional. Obtenga más información en la [sección inferior](#changing-the-language).

**¿Admite la funcionalidad AI/NLP?**

No se admite la funcionalidad AI/NLP.

**¿Cómo puedo orientarme hacia personas anónimas?**

En el cuadro de diálogo, debe utilizar la variable _El correo electrónico de la persona está vacío_ atributo.

## Cambio de idioma {#changing-the-language}

Siga estos pasos para cambiar el idioma de la conversación dinámica.

>[!IMPORTANT]
>
>Cambiar el idioma en el nivel de perfil cambiará el idioma para _all_ aplicaciones Experience Cloud, no solo chat dinámico.

1. En la cuenta de Experience Cloud, haga clic en el icono de configuración y seleccione **Preferencias**.

   ![](assets/dynamic-chat-overview-1.png)

1. Haga clic en el idioma actual en su dirección de correo electrónico.

   ![](assets/dynamic-chat-overview-2.png)

1. Elija el nuevo idioma (el segundo idioma es opcional) y haga clic en **Guardar**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Hay algunas docenas de idiomas entre los que elegir, sin embargo, Dynamic Chat solo admite lo siguiente: inglés, francés, alemán, japonés, español, italiano, portugués de Brasil, coreano, chino simplificado y chino tradicional.

Al actualizar el idioma, todo lo que hay en la propia aplicación cambia excepto las palabras que haya rellenado personalmente (por ejemplo, respuestas de flujo).

## Límites en la conversación dinámica {#limits-in-dynamic-chat}

<table>
  <th>Parámetro</th>
  <th>Descripción</th>
  <th>Límite</th>
 <tr>
  <td>Diálogos totales</td>
  <td>Número total de diálogos (publicados y borradores)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Cuadros de diálogo publicados</td>
  <td>Número de cuadros de diálogo publicados guardados</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Direcciones URL de destino por cuadro de diálogo</td>
  <td>Número de direcciones URL de destino que se pueden agregar a un único cuadro de diálogo</td>
  <td>20</td>
 </tr>
 <tr>
  <td>Atributos por cuadro de diálogo</td>
  <td>Número de atributos que se pueden añadir a los criterios de audiencia para un único cuadro de diálogo</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Grupos</td>
  <td>Número de grupos que se pueden agregar a un único cuadro de diálogo</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Atributos por grupo</td>
  <td>Número de atributos que se pueden agregar a un grupo</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Tarjetas</td>
  <td>Número de tarjetas que se pueden agregar al lienzo por cuadro de diálogo</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Período de retención de datos de posible cliente anónimo</td>
  <td>Duración durante cuánto tiempo se conservará la información de un posible cliente anónimo sin participación</td>
  <td>90 días</td>
 </tr>
 <tr>
  <td>Período de retención de actividad de objetivo</td>
  <td>Cantidad de tiempo que se retienen los datos de actividad de objetivo</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Período de retención de actividad del documento</td>
  <td>Cantidad de tiempo que se retienen los datos de actividad del documento</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Interactuado con período de retención de actividad de cuadro de diálogo</td>
  <td>Se conserva la cantidad de tiempo interaccionado con los datos de actividad del cuadro de diálogo</td>
  <td>90 días</td>
 </tr>
 <tr>
  <td>Período de retención de actividad de reserva de reuniones</td>
  <td>La cantidad de tiempo que la actividad de reserva de reuniones se almacenará en la conversación dinámica</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Conversaciones entabladas</td>
  <td>Número de conversaciones de chat con las que los visitantes web pueden participar cada día</td>
  <td>1.000</td>
 </tr>
 <tr>
  <td>Conversaciones activadas</td>
  <td>Número de conversaciones de chat que se pueden mostrar a los visitantes web por día</td>
  <td>25.000</td>
 </tr>
</table>
