---
description: 'Comportamiento de los bots de chat: Documentos de Marketo: Documentación del producto'
title: Comportamiento de los bots de chat
hide: true
hidefromtoc: true
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 97b1a00b8ff1dc29a92687a70c71093fc8c04267
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Comportamiento de los bots de chat {#chatbot-behavior}

A continuación se presentan diferentes escenarios posibles que superan el comportamiento esperado del bot de chat para el visitante en cada uno de ellos.

<table>
  <tbody>
    <tr>
      <th>Abreviación</th>
      <th>Detalles</th>
    </tr>
    <tr>
      <td>D1, D2, D3, etc.</td>
      <td>Representa varios cuadros de diálogo donde D1 es el cuadro de diálogo uno</td>
    </tr>
    <tr>
      <td>P1, P2, P3, etc.</td>
      <td>Representa las prioridades del diálogo en las que P1 es la prioridad más alta</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, etc.</td>
      <td>Representa varias páginas web donde WP1 es la primera página web</td>
    </tr>
    <tr>
      <td>V1, V2, V3, etc.</td>
      <td>Representa varios visitantes de página web donde V1 es visitante uno</td>
    </tr>
   </tbody>
</table>

## Situaciones {#scenarios}

<table>
  <tr>
      <th>Situación</th>
      <th>Comportamiento esperado de los bots de chat</th>
      <th>Acción back-end</th>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>Visitas V1 WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1 </p>
      </td>
      <td>El recuento de déclencheur para D1 debe aumentarse en 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>Visitas V1 WP1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1</p>
        <p>Después de la actualización, D1 debe resolverse de nuevo</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>Después de la actualización, no hay cambio en el déclencheur D1 ni en el recuento de participación</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió</p>
      </td>
      <td>D1 debe resolverse en V1</td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>Sin cambios en el recuento de participación D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
      </td>
      <td>D1 debe resolverse en V1</td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>El recuento de participación para D1 debe aumentarse en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1</p>
        <p>Después de la actualización, se debe continuar con D1</p>
      </td>
      <td>
        <p>El recuento de déclencheur y el recuento de participación para D1 deben incrementarse en 1</p>
        <p>Después de la actualización, no se realiza ningún cambio en ningún recuento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1, interactúa con el bot de chat y completa D1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1</p>
        <p>Después de la actualización, no se debe resolver ningún cuadro de diálogo ni el cuadro de diálogo siguiente para V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur, el recuento de participación y el recuento completado para D1 deben incrementarse en 1</p>
        <p>Después de la actualización, no se debe resolver ningún cuadro de diálogo ni el cuadro de diálogo siguiente</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 sólo para WP1, WP2</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió </p>
        <p>Visitas V1 WP2</p>
      </td>
      <td>
        <p>La visita a la página WP1, D1 debe resolverse en V1</p>
        <p>La visita a la página WP2, D1 debe resolverse en V2</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>En WP2, no hay cambio en el recuento de déclencheur D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 sólo para WP1, WP2</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y participa</p>
        <p>Visitas V1 WP2</p>
      </td>
      <td>
        <p>La visita a la página WP1, D1 debe resolverse en V1</p>
        <p>La visita a la página WP2, D1 debe resolverse en V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur y el recuento de participación para D1 deben incrementarse en 1</p>
        <p>En WP2, no hay cambio en ningún recuento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>D2 orientado únicamente a WP2</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
        <p>Visitas V1 WP2</p>
      </td>
      <td>
        <p>D1 debe resolverse en el WP1</p>
        <p>D1 debería continuar con V1 en el WP2</p>
      </td>
      <td>
        <p>El recuento de déclencheur y el recuento de participación para D1 deben incrementarse en 1</p>
        <p>Sin cambio en el déclencheur D2 o en el recuento de participación</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>D2 orientado únicamente a WP2</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió </p>
        <p>Visitas V1 WP2</p>
      </td>
      <td>D1 debe resolverse en el WP1<br/>
      D2 debe resolverse en el WP2</td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>El recuento de déclencheur para D2 debe incrementarse en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>D2 orientado únicamente a WP2</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y completa D1</p>
        <p>Visitas V1 WP2</p>
      </td>
      <td>La D1 debería resolverse en el primer período de sesiones y en el período posterior a la terminación<br/>D2 debe resolverse en el WP2</td>
      <td>
        <p>El recuento de déclencheur, el recuento de participación y el recuento completado para D1 deben incrementarse en 1</p>
        <p>El recuento de déclencheur para D2 debe incrementarse en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>D2 orientado únicamente a WP2</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y completa D1</p>
        <p>Visitas V1 WP2</p>
        <p>Los clics V1 en D2 proporcionan la primera respuesta </p>
      </td>
      <td>La D1 debería resolverse en el primer período de sesiones y en el período posterior a la terminación<br/>D2 debe resolverse en el WP2</td>
      <td>
        <p>El recuento de déclencheur, el recuento de participación y el recuento completado para D1 deben incrementarse en 1</p>
        <p>El recuento de déclencheur y participación para D2 debe aumentarse en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió</p>
        <p>D1 no se ha publicado</p>
      </td>
      <td>D1 debe resolverse en V1</td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>No hay cambios en el recuento de participación D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió</p>
        <p>D1 no se ha publicado</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1 por primera vez</p>
        <p>Después de la actualización, no se debe resolver ningún cuadro de diálogo</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>No hay cambios en el recuento de participación D1</p>
        <p>Después de la actualización, no hay cambios en el déclencheur D1 ni en el recuento de participación</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 con D1 </p>
        <p>D1 no se ha publicado</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1</p>
        <p>Después de la actualización, se debe continuar con D1</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>El recuento de participación D1 debe aumentarse en 1</p>
        <p>Después de la actualización, ya que D1 no se cambiará más en el recuento de déclencheur o de participación</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió</p>
        <p>D1 se publica con nuevos cambios</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1 por primera vez</p>
        <p>Después de la actualización, el cuadro de diálogo con los cambios nuevos debe resolverse</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>Después de la actualización, como D1 con nuevos cambios, pero sin cambios adicionales en el recuento de déclencheur</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 únicamente para WP1</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>Los clics V1 en D1 proporcionan la primera respuesta</p>
        <p>D1 se publica con nuevos cambios</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1 por primera vez</p>
        <p>Después de la actualización, el cuadro de diálogo con los cambios antiguos debe continuar</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>El recuento de participación para D1 debe aumentarse en 1 </p>
        <p>Después de la actualización, ya que aparecerá el antiguo D1, por lo que no se cambiará el recuento de déclencheur</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 con prioridad 1</p>
        <p>D2 destinado al WP1 con 2 prioridades</p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no respondió</p>
        <p>D1 no se ha publicado</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1 por primera vez</p>
        <p>Después de la actualización, D2 debe resolverse en V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>Después de la actualización, el recuento de déclencheur para D2 debe aumentarse en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 con prioridad 1</p>
        <p>D2 destinado al WP1 con 2 prioridades </p>
        <p>V1 visita el WP1 por primera vez</p>
        <p>V1 hace clic en D1 y completa D1</p>
        <p>V1 actualiza WP1 y ve D2<br/>V1 hace clic en D2 y completa D2</p>
        <p>El experto en marketing ha realizado cambios en D1 y ha vuelto a publicar</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse en V1 por primera vez</p>
        <p>Después de la actualización, D2 debe resolverse en V1</p>
        <p>Después de completar D1 y D2, independientemente de los cambios o de la republicación de D1, D2 no debe volver a mostrarse en V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur, el recuento de participación y el recuento completado para D1 deben incrementarse en 1</p>
        <p>Actualizar después de que se complete la D2, no hay que realizar ninguna acción</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 dirigido para WP1 con el déclencheur "Tiempo en el sitio" de 30 segundos</p>
        <p>Visitas V1 WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse, pero no se activará en V1</p>
        <p>Después de 30 segundos, se debe mostrar/activar D1 en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 debe aumentarse en 1 solo después de haber pasado más de 30 segundos en la página web</td>
    </tr>
    <tr>
      <td>
        <p>D1 destinado a WP1, WP2 con un déclencheur de "Tiempo en la página" de 30 segundos</p>
        <p>Visitas V1 WP1, WP2</p>
      </td>
      <td>
        <p>D1 debe resolverse, pero no se activará en V1</p>
        <p>Después de 30 segundos, se debe mostrar/activar D1 en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 debe aumentarse en 1 solo después de haber pasado más de 30 segundos en la página web</td>
    </tr>
    <tr>
      <td>
        <p>D1 con un déclencheur de "porcentaje de desplazamiento" de 50</p>
        <p>Visitas V1 WP1</p>
      </td>
      <td>
        <p>D1 debe resolverse, pero no se activará en V1</p>
        <p>Después de un desplazamiento del 50 %, se debe mostrar/activar D1 a V1</p>
      </td>
      <td>El recuento de déclencheur para D1 debe aumentarse en 1 solo después de desplazarse un 50 %</td>
    </tr>
    <tr>
      <td>
        <p>D1 dirigido a WP1 con 1 prioridad y déclencheur de evento "Tiempo en la página" de 30 segundos</p>
        <p>D2 destinado a WP1 con 2 prioridad y "porcentaje de desplazamiento de página" de evento de 50</p>
        <p>V1 visita WP1, después de 10 segundos V1 visita WP2, V1 visita WP1</p>
      </td>
      <td>
        <p>En WP1, D1 debe resolverse, pero no se activará en V1</p>
        <p>En WP2, D2 debe resolverse, pero no se activará en V1</p>
        <p>En WP1, D1 debe resolverse y después de 20 segundos D1 debe activarse en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 debe aumentarse en 1 solo después de 30 segundos</td>
    </tr>
    <tr>
      <td>
        <p>D1 dirigido a WP1 con el déclencheur "Tiempo en el sitio" de 1 minuto</p>
        <p>La V1 visita el WP1 durante 1 minuto y se muestra en la D1, pero no interactúa</p>
        <p>V1 cierra WP1 y vuelve a WP1 2 días después</p>
      </td>
      <td>
        <p>La D1 debe mostrarse automáticamente a la V1, ya que ya ha cumplido los criterios de déclencheur durante la sesión anterior</p>
        <p>La misma lógica debería aplicarse a "Tiempo en la página" y "porcentaje de desplazamiento de la página".</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 debe aumentarse en 1</p>
        <p>Después del retorno, no hay que adoptar ninguna medida</p>
      </td>
    </tr>
  </tbody>
</table>
