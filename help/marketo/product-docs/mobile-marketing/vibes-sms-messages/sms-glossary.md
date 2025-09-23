---
description: 'Glosario de SMS: documentos de Marketo, documentación del producto'
title: Glosario de SMS
feature: Mobile Marketing
exl-id: 0c23ca9f-f994-42ae-bd72-7d37289b7a94
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 1%

---

# Glosario de SMS {#sms-glossary}

A continuación se muestran algunos términos comunes que encontrará al usar mensajes SMS de Vibes con Marketo Engage.

<table>
<thead>
  <tr>
    <th>Término</th>
    <th>Definición</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Campaña de adquisición</td>
    <td>Una campaña realizada para adquirir nuevos suscriptores en las listas de suscripción. Se puede agregar un suscriptor a una campaña de adquisición a través de un formulario web de Marketo o enviando un mensaje de texto con una palabra clave.</td>
  </tr>
  <tr>
    <td>Administrador de campañas</td>
    <td>Campaign Manager se encuentra en la plataforma Vibes y es donde se puede configurar una lista de suscripción y una campaña de adquisición. Los usuarios con una licencia de plataforma de Vibes completa tienen acceso a tipos de campaña adicionales.</td>
  </tr>
  <tr>
    <td>Clave de compañía</td>
    <td>Company_key es un identificador alfanumérico único para la cuenta de plataforma. Si tiene varias cuentas de compañía en la plataforma Vibes (como cuentas secundarias), puede tener varias claves de compañía. Cada instancia de Marketo Engage solo se puede asignar a una clave de compañía de Vibes.</td>
  </tr>
  <tr>
    <td>CTA (call to action)</td>
    <td>Señalización digital o física o escritura verbal para la adquisición de suscriptores en un programa de mensaje de texto recurrente o lista de suscripción. Se puede colocar en línea, en las redes sociales, en correos electrónicos, en papel, etc.</td>
  </tr>
  <tr>
    <td>Dominio corto personalizado</td>
    <td>Si utiliza el acortador de vínculos de Vibes, la URL abreviada aparecerá, de forma predeterminada, en la URL abreviada de Vibes: https://vbs.cm/xxxxxx. Un dominio corto personalizado es un dominio único de su marca. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">Más información sobre los dominios cortos personalizados</a>.<p>
    Esto solo se aplica a los mensajes enviados desde la plataforma Vibes, específicamente los mensajes de campaña de adquisición y los mensajes predeterminados de código corto.<p>
    Se recomienda usar el abreviador de URL de Marketo para tener datos de clics en el programa de Marketo.</td>
  </tr>
  <tr>
    <td>Mensajes predeterminados</td>
    <td>Mensajes obligatorios para el código corto para responder a las solicitudes de AYUDA, DETENER y mensajes no reconocidos.</td>
  </tr>
  <tr>
    <td>Desconectar</td>
    <td>Las desconexiones son una forma de exclusión debido a que el número de móvil se elimina de una red de operadores. Las razones para una desconexión incluyen: una cuenta se ha cerrado por completo, una cuenta de prepago se quedó sin fondos o el número se eliminó de la red de operadores por otras razones desconocidas. Los números de móvil desconectados y no transferidos a otro operador de telefonía móvil cancelan la suscripción a todas las listas de suscripción de la plataforma Vibes.</td>
  </tr>
  <tr>
    <td>Inclusión doble</td>
    <td>Método de adquisición que requiere que un suscriptor potencial confirme su consentimiento para ser agregado a una lista de suscripción con un comando de respuesta, como "Y" o su código postal. El uso de un mensaje de doble inclusión puede ayudarle a cumplir con las directrices de mensajería de texto estatales y federales.</td>
  </tr>
  <tr>
    <td>Evento</td>
    <td>Un evento es una incidencia definida que se puede enviar a la plataforma Vibes y utilizar para almacenar en déclencheur las acciones activadas por API, incluidos los envíos de mensajes. Cada evento contiene datos específicos del evento, incluido un event_type, que se utiliza para determinar a qué campaña de mensajes activada por API corresponde. La API de evento se puede activar mediante Webhook en Marketo Engage. Obtenga más información con nuestra <a href="https://developer-platform.vibes.com/reference/event-api">referencia de API de eventos</a>.</td>
  </tr>
  <tr>
    <td>Palabra clave</td>
    <td>Una palabra corta o cadena alfanumérica que el consumidor envía al código corto para iniciar una experiencia móvil.</td>
  </tr>
  <tr>
    <td>Código largo (10DLC)</td>
    <td>Un ID de remitente desde el que se envían mensajes bidireccionales entre la marca y el consumidor. Los códigos largos de EE. UU. tienen 10 dígitos numéricos.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Número de directorio móvil o número de teléfono de una persona. Los números de MDN y de teléfono móvil no son identificadores únicos en Marketo.</td>
  </tr>
  <tr>
    <td>Base de datos móvil</td>
    <td>La base de datos móvil es la base de datos donde Vibes almacena los datos del suscriptor. Cada suscriptor tiene un "registro de persona" único, en el que se rellenan el número de móvil y los campos personalizados asociados.</td>
  </tr>
  <tr>
    <td>Participante</td>
    <td>Persona que tiene una o más interacciones móviles (como enviar un mensaje de texto) con su programa móvil, pero que no se ha suscrito a una lista de suscripción.</td>
  </tr>
  <tr>
    <td>Registro de persona</td>
    <td>Un registro de persona es una recopilación de datos de un número de teléfono móvil específico. A cada registro de persona también se le asigna una clave persona única para la identificación. Los ID de Marketo están vinculados a las vibraciones mediante el campo external_person_id. Obtenga más información acerca de los registros de personas en <a href="https://developer-platform.vibes.com/reference/person-api">Vibes Person API documentation</a>.</td>
  </tr>
  <tr>
    <td>Código corto</td>
    <td>Un ID de remitente desde el que se envían mensajes bidireccionales entre la marca y el consumidor. Los códigos cortos de Estados Unidos tienen entre 5 y 6 dígitos numéricos. Los códigos cortos canadienses tienen de 4 a 6 dígitos numéricos. La integración de Marketo LaunchPoint con Vibes admite un código corto por instancia.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Servicio de mensajes cortos. Este es un mensaje que incluye solo texto.</td>
  </tr>
  <tr>
    <td>Listas de suscripción</td>
    <td>Una lista de números de teléfono móvil (y sus registros personales correspondientes) que proporcionaron consentimiento para recibir mensajes recurrentes de su programa.</td>
  </tr>
  <tr>
    <td>Suscriptor</td>
    <td>Un número de móvil suscrito a una o varias listas de suscripción.</td>
  </tr>
  <tr>
    <td>Plataforma de vibraciones</td>
    <td>El sitio web en el que inicia sesión para administrar sus campañas. Vaya a <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> para acceder a la plataforma Vibes.</td>
  </tr>
</tbody>
</table>
