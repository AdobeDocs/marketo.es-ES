---
description: Información general del Dynamic Chat - Documentos de Marketo - Documentación del producto
title: Resumen del Dynamic Chat
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 2f5b79e9fb0340dd1ed65b00f2ec3ac487b7b7ca
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 2%

---

# Resumen del Dynamic Chat {#dynamic-chat-overview}

Dynamic Chat le permite aprovechar una interfaz fácil de usar para dirigirse tanto a las personas como a las cuentas que visitan el sitio web. Recopile contenido relevante, como nombre, información de contacto y texto libre. Los visitantes del sitio también pueden reservar reuniones con su equipo de ventas. Los datos de participación y actividad del Dynamic Chat se pueden utilizar para añadir miembros a programas de Marketo y actividades multicanal de déclencheur.

>[!TIP]
>
>Visita [esta página](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html){target="_blank"} para ver vídeos de tutoriales de Dynamic Chat.

## Integraciones {#integrations}

Un componente clave de Dynamic Chat es su capacidad para interactuar de forma nativa con la suscripción de Marketo. Para aprovechar todas las capacidades de esta integración, primero debe iniciar la sincronización de datos. Según el tamaño de la base de datos de Marketo, los datos iniciales pueden tardar hasta 24 horas en completarse. [sincronización única](/help/marketo/product-docs/demand-generation/dynamic-chat-two/integrations/adobe-marketo-engage.md){target="_blank"} para completar.

Se sincroniza lo siguiente:

* Datos del campo de persona
* Datos de campo de empresa
* Datos de actividad

## Diálogos {#dialogues}

Los cuadros de diálogo representan una única participación en el chat. Piense en él como un contenedor con todo lo que necesita para tener un diálogo de chat atractivo para los visitantes de su sitio web. En cada cuadro de diálogo, puede especificar en qué página desea que aparezca el cuadro de diálogo, a quién desea que se muestre y el contenido y flujo del propio cuadro de diálogo. Además, puede encontrar métricas para ver el rendimiento de su cuadro de diálogo. [Más información sobre los Cuadros de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/dialogue-overview.md){target="_blank"}.

## Configuración {#configuration}

En la pestaña Configuración, personalice el aspecto de los distintos cuadros de diálogo. Cambiar fuente, colores, tiempo de respuesta y mucho más. [Más información sobre la Configuración](/help/marketo/product-docs/demand-generation/dynamic-chat-two/setup-and-configuration/configuration.md){target="_blank"}.

## Calendario {#calendar}

Conecte el calendario de Outlook o Gmail para utilizarlo en la programación de citas en el bot de chat. [Más información sobre el Calendario](/help/marketo/product-docs/demand-generation/dynamic-chat-two/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## Reuniones {#meetings}

Aquí es donde verá todas las citas programadas por los visitantes del sitio web a través de los distintos cuadros de diálogo. [Más información sobre las Reuniones](/help/marketo/product-docs/demand-generation/dynamic-chat-two/meeting-list.md){target="_blank"}

## Enrutando {#routing}

Aquí puede ver una lista de todos los agentes que han conectado sus calendarios, el orden en que se presentarán a los visitantes del sitio web y la creación de reglas de enrutamiento personalizadas. [Más información sobre el Enrutamiento](/help/marketo/product-docs/demand-generation/dynamic-chat-two/setup-and-configuration/routing.md){target="_blank"}

## Chat en directo {#live-chat}

Ofrezca a sus visitantes web cualificados la posibilidad de conectarse con sus representantes de ventas a través de [chat en vivo](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/live-chat-overview.md){target="_blank"}.

## Preguntas frecuentes {#faq}

**¿Puedo instalar Dynamic Chat en cualquier lugar del sitio web de mi empresa o solo funciona en las páginas de aterrizaje de Marketo?**

El fragmento de JavaScript de Dynamic Chat se puede instalar en cualquier sitio web, así como en páginas de aterrizaje de Marketo.

**¿Durante cuánto tiempo se almacenan los datos para la creación de informes?**

90 días.

**¿El Dynamic Chat permite el chat en vivo?**

No, solo utiliza respuestas predeterminadas.

**¿Dynamic Chat admite otros idiomas además del inglés?**

Sí. Dynamic Chat admite los siguientes idiomas: francés, alemán, japonés, español, italiano, portugués (Brasil), coreano, chino simplificado y chino tradicional. Obtenga más información en la [sección siguiente](#changing-the-language).

**¿Admite la funcionalidad AI/NLP?**

No admitimos la funcionalidad AI/NLP.

**¿Cómo puedo dirigirme a personas anónimas?**

En el cuadro de diálogo, debe utilizar el _Correo electrónico de persona está vacío_ atributo.

## Cambio de idioma {#changing-the-language}

Siga estos pasos para cambiar el idioma del Dynamic Chat.

>[!IMPORTANT]
>
>Si cambia el idioma en el nivel de perfil, se cambiará el idioma de _todo_ Aplicaciones Experience Cloud, no solo Dynamic Chat.

1. En la cuenta de Experience Cloud, haga clic en el icono de configuración y seleccione **Preferencias**.

   ![](assets/dynamic-chat-overview-1.png)

1. Haga clic en el idioma actual debajo de su dirección de correo electrónico.

   ![](assets/dynamic-chat-overview-2.png)

1. Elija su nuevo idioma (el segundo idioma es opcional) y haga clic en **Guardar**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Hay algunas docenas de idiomas para elegir, sin embargo, el Dynamic Chat solo admite lo siguiente: inglés, francés, alemán, japonés, español, italiano, portugués de Brasil, coreano, chino simplificado y chino tradicional.

Al actualizar el idioma, todo cambia en la propia aplicación, excepto las palabras que haya rellenado personalmente (por ejemplo, respuestas de flujo).

## Límites de retención de datos de Dynamic Chat {#dynamic-chat-data-retention-limits}

<table>
  <th>Tipo de datos</th>
  <th>Período de retención</th>
 <tr>
  <td>Posible Cliente Anónimo Sin Ninguna Participación</td>
  <td>90 días</td>
 </tr>
 <tr>
  <td>Actividad de objetivo</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Actividad de documento</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Interactuó con la actividad de diálogo</td>
  <td>90 días</td>
 </tr>
 <tr>
  <td>Actividad de reserva de reunión</td>
  <td>24 meses</td>
 </tr>
</table>
