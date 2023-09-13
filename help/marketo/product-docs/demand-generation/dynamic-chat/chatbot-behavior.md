---
description: 'Comportamiento del bot de chat: documentos de Marketo: documentación del producto'
title: Comportamiento del bot de chat
feature: Dynamic Chat
source-git-commit: 9a8f6fe57b585ba0eac6a577bf99e0419d8818a1
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Comportamiento del bot de chat {#chatbot-behavior}

Los siguientes son diferentes escenarios posibles que describen el comportamiento esperado del bot de chat para el visitante en cada uno.

<table>
  <tbody>
    <tr>
      <th>Abreviatura</th>
      <th>Detalles</th>
    </tr>
    <tr>
      <td>D1, D2, D3, etc.</td>
      <td>Representa varios cuadros de diálogo donde D1 es el cuadro de diálogo uno</td>
    </tr>
    <tr>
      <td>P1, P2, P3, etc.</td>
      <td>Representa las prioridades del cuadro de diálogo donde P1 es la prioridad más alta</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, etc.</td>
      <td>Representa varias páginas Web donde WP1 es la primera página Web</td>
    </tr>
    <tr>
      <td>V1, V2, V3, etc.</td>
      <td>Representa varios visitantes de página web donde V1 es el visitante uno</td>
    </tr>
   </tbody>
</table>

## Escenarios {#scenarios}

<table>
  <tr>
      <th>Escenario</th>
      <th>Comportamiento esperado del bot de chat</th>
      <th>Acción back-end</th>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 se incrementará en 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1</p>
        <p>Después de la actualización, D1 se resolverá de nuevo</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Después de la actualización, no se realizarán cambios en el déclencheur D1 ni en el recuento de participaciones</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
      </td>
      <td>D1 se resolverá en V1</td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Sin cambios en el recuento de participación D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
      </td>
      <td>D1 se resolverá en V1</td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>El recuento de participación para D1 se incrementará en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1</p>
        <p>Después de la actualización, D1 continuará</p>
      </td>
      <td>
        <p>El recuento de déclencheur y el recuento de participaciones de D1 se incrementarán en 1</p>
        <p>Después de la actualización, sin cambios en ningún recuento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1, se involucra con el bot de chat y completa D1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1</p>
        <p>Después de la actualización, no se resolverá ningún cuadro de diálogo ni el siguiente para V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur, el recuento de interacciones y el recuento completado de D1 se incrementarán en 1</p>
        <p>Después de la actualización, no se resolverá ningún cuadro de diálogo ni el siguiente</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1, WP2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>Visita de página WP1, D1 se resolverá en V1</p>
        <p>Visita de página WP2, D1 se resolverá en V2</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>En WP2, sin cambio en el recuento de déclencheur D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1, WP2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y se activa</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>Visita de página WP1, D1 se resolverá en V1</p>
        <p>Visita de página WP2, D1 se resolverá en V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur y el recuento de participaciones de D1 se incrementarán en 1</p>
        <p>En WP2, sin cambios en ningún recuento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>D2 se ha dirigido únicamente a WP2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>D1 se resolverá en WP1</p>
        <p>D1 continuará a V1 en WP2</p>
      </td>
      <td>
        <p>El recuento de déclencheur y el recuento de participaciones de D1 se incrementarán en 1</p>
        <p>Sin cambios en el déclencheur D2 o en el recuento de compromiso</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>D2 se ha dirigido únicamente a WP2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
        <p>V1 visita WP2</p>
      </td>
      <td>D1 se resolverá en WP1<br/>
      D2 se resolverá en WP2</td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>El recuento de déclencheur para D2 se incrementará en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>D2 se ha dirigido únicamente a WP2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y completa D1</p>
        <p>V1 visita WP2</p>
      </td>
      <td>D1 se resolverá el WP1 y después de la finalización<br/>D2 se resolverá en WP2</td>
      <td>
        <p>El recuento de déclencheur, el recuento de interacciones y el recuento completado de D1 se incrementarán en 1</p>
        <p>El recuento de déclencheur para D2 se incrementará en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>D2 se ha dirigido únicamente a WP2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y completa D1</p>
        <p>V1 visita WP2</p>
        <p>V1 hace clic en D2 y proporciona la primera respuesta</p>
      </td>
      <td>D1 se resolverá el WP1 y después de la finalización<br/>D2 se resolverá en WP2</td>
      <td>
        <p>El recuento de déclencheur, el recuento de interacciones y el recuento completado de D1 se incrementarán en 1</p>
        <p>El recuento de déclencheur y participación de D2 se incrementará en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
        <p>Se ha cancelado la publicación de D1</p>
      </td>
      <td>D1 se resolverá en V1</td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Sin cambios en el recuento de participación D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
        <p>Se ha cancelado la publicación de D1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1 por primera vez</p>
        <p>Después de la actualización, no se resolverá ningún cuadro de diálogo</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Sin cambios en el recuento de participación D1</p>
        <p>Después de la actualización, no se realizarán cambios en el déclencheur D1 ni en el recuento de participaciones</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 acoplado con D1</p>
        <p>Se ha cancelado la publicación de D1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1</p>
        <p>Después de la actualización, D1 continuará</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>El recuento de participación D1 se aumentará en 1</p>
        <p>Después de la actualización, como D1 se seguirá sin cambiar al recuento de déclencheur o participaciones</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
        <p>D1 se publica con nuevos cambios</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1 por primera vez</p>
        <p>Después de la actualización, se resolverá el cuadro de diálogo con los nuevos cambios</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Después de la actualización, como D1 con nuevos cambios, pero sin más cambios en el recuento de déclencheur</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se ha dirigido únicamente a WP1</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y proporciona la primera respuesta</p>
        <p>D1 se publica con nuevos cambios</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1 por primera vez</p>
        <p>Después de la actualización, el diálogo con los cambios antiguos continuará</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>El recuento de participación para D1 se incrementará en 1</p>
        <p>Después de la actualización, como el D1 anterior aparecerá, para que no se cambie el recuento de déclencheur</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 se dirige a WP1 con prioridad 1</p>
        <p>D2 previsto para WP1 con prioridad 2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 pero no responde</p>
        <p>Se ha cancelado la publicación de D1</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1 por primera vez</p>
        <p>Después de la actualización, D2 se resolverá en V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Después de la actualización, el recuento de déclencheur para D2 aumentará en 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se dirige a WP1 con prioridad 1</p>
        <p>D2 previsto para WP1 con prioridad 2</p>
        <p>V1 visita WP1 por primera vez</p>
        <p>V1 hace clic en D1 y completa D1</p>
        <p>V1 actualiza WP1 y ve D2<br/>V1 hace clic en D2 y completa D2</p>
        <p>El especialista en marketing ha realizado cambios en D1 y ha vuelto a publicar</p>
        <p>V1 actualiza WP1</p>
      </td>
      <td>
        <p>D1 se resolverá en V1 por primera vez</p>
        <p>Después de la actualización, D2 se resolverá en V1</p>
        <p>Después de completar D1 y D2, independientemente de los cambios o volver a publicar D1, D2 no se mostrará de nuevo a V1</p>
      </td>
      <td>
        <p>El recuento de déclencheur, el recuento de interacciones y el recuento completado de D1 se incrementarán en 1</p>
        <p>Actualizar después de que D2 se complete; no se realizará ninguna acción</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 se dirigió a WP1 con un déclencheur de "Tiempo en el sitio" de 30 segundos</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 se resolverá, pero no se activará en V1</p>
        <p>Después de 30 segundos, se mostrará/activará D1 en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 solo aumentará en 1 después de que se hayan transcurrido más de 30 segundos en la página web</td>
    </tr>
    <tr>
      <td>
        <p>D1 se dirigió a WP1, WP2 con el déclencheur "Tiempo en la página" de 30 segundos</p>
        <p>V1 visita WP1, WP2</p>
      </td>
      <td>
        <p>D1 se resolverá, pero no se activará en V1</p>
        <p>Después de 30 segundos, se mostrará/activará D1 en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 solo aumentará en 1 después de que se hayan transcurrido más de 30 segundos en la página web</td>
    </tr>
    <tr>
      <td>
        <p>D1 se dirigió a WP1 con un déclencheur de "porcentaje de desplazamiento" de 50</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 se resolverá, pero no se activará en V1</p>
        <p>Después del desplazamiento del 50 %, se mostrará/activará D1 en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 solo aumentará en 1 después de desplazar el 50 %</td>
    </tr>
    <tr>
      <td>
        <p>D1 se dirigió a WP1 con una prioridad y un déclencheur de evento de "Tiempo en la página" de 30 segundos</p>
        <p>D2 se dirigió a WP1 con 2 prioridad y evento "porcentaje de desplazamiento de página" de 50</p>
        <p>V1 visita WP1, después de 10 segundos V1 visita WP2, V1 visita WP1</p>
      </td>
      <td>
        <p>En WP1, se resolverá D1, pero no se activará en V1</p>
        <p>En WP2, D2 se resolverá pero no se activará en V1</p>
        <p>En WP1, D1 se resolverá y, después de 20 segundos, D1 se activará en V1</p>
      </td>
      <td>El recuento de déclencheur para D1 solo aumentará en 1 después de 30 segundos</td>
    </tr>
    <tr>
      <td>
        <p>D1 se dirigió a WP1 con un déclencheur de "Tiempo en el sitio" de 1 minuto</p>
        <p>V1 visita el WP1 durante 1 minuto y se muestra D1, pero no interactúa</p>
        <p>V1 cierra WP1 y vuelve a WP1 2 días después</p>
      </td>
      <td>
        <p>D1 se mostrará automáticamente a V1 porque ya cumplieron los criterios de déclencheur durante la sesión anterior</p>
        <p>La misma lógica se aplicará al "Tiempo en la página" y al "porcentaje de desplazamiento de la página"</p>
      </td>
      <td>
        <p>El recuento de déclencheur para D1 se incrementará en 1</p>
        <p>Después de la devolución, no se debe realizar ninguna acción</p>
      </td>
    </tr>
  </tbody>
</table>

