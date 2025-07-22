---
description: Información general de Dynamic Chat - Documentos de Marketo - Documentación del producto
title: Información general de Dynamic Chat
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 4%

---

# Información general de [!DNL Dynamic Chat] {#dynamic-chat-overview}

Dynamic Chat le permite aprovechar una interfaz fácil de usar para dirigirse tanto a las personas como a las cuentas que visitan el sitio web. Recopile contenido relevante, como nombre, información de contacto y texto libre. Los visitantes del sitio también pueden chatear con un agente activo e incluso reservar reuniones con su equipo de ventas. Los datos de actividad y participación de Dynamic Chat se pueden utilizar para añadir miembros a programas de Marketo y actividades de déclencheur multicanal.

>[!TIP]
>
>Visite [esta página](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html?lang=es){target="_blank"} para ver vídeos de tutoriales de Dynamic Chat.

## Integraciones {#integrations}

Un componente clave de Dynamic Chat es su capacidad para interactuar de forma nativa con la suscripción de Marketo. Para aprovechar todas las capacidades de esta integración, primero debe iniciar la sincronización de datos. Según el tamaño de la base de datos de Marketo, los datos pueden tardar hasta 24 horas en completarse para la [sincronización única](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"} inicial.

Se sincroniza lo siguiente:

* Datos del campo de persona
* Datos de campo de empresa
* Datos de actividad

## Diálogos {#dialogues}

Los cuadros de diálogo representan una única participación en el chat. Piense en él como un contenedor con todo lo que necesita para tener un diálogo de chat atractivo para los visitantes de su sitio web. En cada cuadro de diálogo, puede especificar en qué página desea que aparezca el cuadro de diálogo, a quién desea que se muestre y el contenido y flujo del propio cuadro de diálogo. Además, puede encontrar métricas para ver el rendimiento de su cuadro de diálogo. [Más información sobre los cuadros de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}.

## Configuración {#configuration}

En la pestaña Configuración, personalice el aspecto de los distintos cuadros de diálogo. Cambiar fuente, colores, tiempo de respuesta y mucho más. [Más información sobre la configuración](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}.

## Calendario {#calendar}

Conecte el calendario de Outlook o Gmail para utilizarlo en la programación de citas en el bot de chat. [Más información sobre el Calendario](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## Reuniones {#meetings}

Aquí es donde verá todas las citas programadas por los visitantes del sitio web a través de los distintos cuadros de diálogo. [Más información sobre las reuniones](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## Enrutando {#routing}

Aquí puede ver una lista de todos los agentes que han conectado sus calendarios, el orden en que se presentarán a los visitantes del sitio web y la creación de reglas de enrutamiento personalizadas. [Más información sobre el enrutamiento](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## Chat en directo {#live-chat}

Ofrezca a sus visitantes calificados para que se conecten con sus representantes de ventas a través de [chat en vivo](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}.

## Flujo conversacional {#conversational-flow}

[Diseña una conversación](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"} que un visitante pueda activar según la acción que designes (por ejemplo, rellenar un formulario, hacer clic en un vínculo, etc.).

## IA generativa {#generative-ai}

[IA generativa](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"} en Adobe Dynamic Chat procesa las señales de intención, las preferencias del usuario y el comportamiento anterior en tiempo real para generar mensajes relevantes y personalizados para los visitantes del chat.

## Cambio de idioma {#changing-the-language}

Siga los pasos a continuación para cambiar el idioma de Dynamic Chat.

>[!IMPORTANT]
>
>Si cambia el idioma en el nivel de perfil, se cambiará el idioma de _todas_ las aplicaciones de Experience Cloud, no solo [!DNL Dynamic Chat].

1. En tu cuenta de Experience Cloud, haz clic en el icono de configuración y elige **[!UICONTROL Preferencias]**.

   ![](assets/dynamic-chat-overview-1.png)

1. Haga clic en el idioma actual debajo de su dirección de correo electrónico.

   ![](assets/dynamic-chat-overview-2.png)

1. Elija su nuevo idioma (el segundo idioma es opcional) y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Hay algunas docenas de idiomas para elegir, pero [!DNL Dynamic Chat] solo admite lo siguiente: inglés, francés, alemán, japonés, español, italiano, portugués (Brasil), coreano, chino simplificado y chino tradicional.

Al actualizar el idioma, todo cambia en la propia aplicación, excepto las palabras que haya rellenado personalmente (por ejemplo, respuestas de flujo).

## Límites de retención de datos de Dynamic Chat {#dynamic-chat-data-retention-limits}

A continuación se muestran algunos de los límites y parámetros dentro de Dynamic Chat. Para obtener una lista completa, consulte la [página de descripción del producto](https://helpx.adobe.com/es/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"} de Marketo Engage.

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

## Preguntas frecuentes {#faq}

Consulte las [preguntas frecuentes sobre Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}.
