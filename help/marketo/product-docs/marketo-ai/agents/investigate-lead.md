---
description: El agente principal de investigación responde a las preguntas que los especialistas en marketing formulan con más frecuencia. Es más rápido y confiable que examinar manualmente los registros de actividad, el historial de campañas inteligentes y los registros de puntuación.
title: Investigar posible cliente
beta: true
hide: true
hidefromtoc: true
source-git-commit: a2c170ced2119a86ffe1f2da1bde212afa4841f0
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Investigar posible cliente {#investigate-lead}

Averigüe por qué una persona o posible cliente específico no alcanzó un hito (como MQL, calificación de programas o una campaña) y obtenga una explicación en lenguaje sencillo de lo que sucedió.

>[!PREREQUISITES]
>
>Debe tener acceso de visualización al registro de posible cliente y al programa o hito que está investigando.

## Cómo funciona

Le dice a Marketo AI qué posible cliente está investigando y qué hito o resultado esperaba. Marketo AI examina el historial de actividades del posible cliente, el registro de puntuación, la pertenencia a programas, el historial de cualificaciones de campañas inteligentes y cualquier filtro o regla de supresión relevante. A continuación, devuelve una explicación clara de qué bloqueó o retrasó el resultado esperado: por ejemplo, &quot;La puntuación de este posible cliente alcanzó 48, pero el umbral de MQL es 50&quot; o &quot;Este posible cliente se excluyó de la campaña porque canceló la suscripción el 3 de marzo&quot;.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **Generar con IA**.

1. En la ventana del mensaje, describa lo que está investigando. Incluya el posible cliente (por correo electrónico o nombre) y lo que esperaba que sucediera.

>[!NOTE]
>
>Algunos ejemplos son: &quot;¿Por qué `john.smith@example.com` no alcanzó el MQL el mes pasado?&quot; o &quot;¿Por qué no se añadió Brenda Gonzales al programa de seminarios web del tercer trimestre?&quot;

1. Marketo AI extrae el registro del posible cliente y el historial relevante.

1. Revise la explicación. Marketo AI le informa del motivo específico por el que no se alcanzó el hito y, si es posible, de qué debería cambiar para que el posible cliente cumpla los requisitos.

1. Tome medidas basadas en la búsqueda: corrija un problema de datos, ajuste un filtro, actualice la puntuación del posible cliente o acepte que el resultado fue correcto.

## Ejemplos

**Umbral de MQL no alcanzado**
Un gerente de generación de demanda observa un posible cliente que las ventas señalaron como interesadas pero que nunca llegaron a MQL. Pregunta: &quot;¿Por qué david.chen@techcorp.com no llegó a MQL?&quot; Marketo AI encuentra que la puntuación de comportamiento del posible cliente es de 42 (8 puntos por debajo del umbral de MQL de 50) y enumera las actividades de puntuación que contribuyeron. Puede ver exactamente qué comportamientos empujarían al posible cliente por encima del umbral.

**Omisión de campaña debido a supresión**
Un administrador de campaña pregunta por qué un contacto específico no recibió un correo electrónico de invitación que se dirigía al resto de su lista. Marketo AI encuentra que el contacto está en la lista de marketing suspendido, lo que los excluye automáticamente de todos los envíos de campañas. El administrador se pone en contacto directamente con el contacto para investigar por qué se suprimieron.

**Error de calificación del programa**
Un especialista en operaciones de marketing está solucionando el problema de por qué un posible cliente que asistió a un seminario web no se añadió al programa de seguimiento posterior al evento. Marketo AI rastrea el problema: el posible cliente registrado, pero marcado como &quot;Sin programa&quot; en el programa de evento y el filtro de campaña de seguimiento requiere el estado &quot;Asistido&quot;. El estado se estableció incorrectamente en la integración.

**Plomo atascado en una crianza**
Un gerente de generación de demanda observa que un posible cliente ha estado en la misma etapa de crianza durante 90 días sin progresar. Pide a Marketo AI que investigue. Encuentra que la puntuación de participación del posible cliente cayó por debajo del umbral requerido para avanzar a la siguiente etapa y que el posible cliente no ha abierto un correo electrónico en 60 días, lo que los califica para la rama de renovación de participación en su lugar.

## Sugerencias y limitaciones

* Lead Investigation explica qué ha pasado en función de la actividad y configuración registradas de Marketo: no puede explicar las decisiones tomadas fuera de Marketo (por ejemplo, por qué un compañero ha eliminado manualmente un posible cliente).
* Si el historial de actividad de un posible cliente es muy largo, Marketo AI se centra en los eventos más recientes y relevantes relacionados con su pregunta.
* La investigación de posibles clientes es de solo lectura: le indicará lo que ha sucedido, pero no realizará cambios en el registro de posibles clientes o en la pertenencia a programas.
* Para los problemas que resultan ser problemas de calidad de datos (valores de campo que faltan, fuente de posibles clientes incorrecta), la corrección deberá realizarse manualmente en el registro de posibles clientes.
* Si la investigación revela un problema de lógica de campaña inteligente que afecta a muchos posibles clientes, utilice el control de calidad del programa para revisar la configuración completa del programa.
