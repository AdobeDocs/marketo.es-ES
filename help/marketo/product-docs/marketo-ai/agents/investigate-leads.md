---
description: El agente principal de investigación responde a las preguntas que los especialistas en marketing formulan con más frecuencia. Es más rápido y confiable que examinar manualmente los registros de actividad, el historial de campañas inteligentes y los registros de puntuación.
title: Investigar posibles clientes
source-git-commit: 3f7d17870cf0d60c716095ae200c003fc8ff0e28
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Investigar posibles clientes {#investigate-leads}

Averigüe por qué una persona o posible cliente específico no alcanzó un hito (como MQL, calificación de programas o una campaña) y obtenga una explicación en lenguaje sencillo de lo que sucedió.

>[!PREREQUISITES]
>
>* Para usar esta característica, primero debe aceptar los términos de [Core Gen-AI y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.
>
>* Debe tener acceso de visualización al registro de persona/posible cliente y al programa o hito que está investigando.

>[!AVAILABILITY]
>
>Esta función se encuentra actualmente en versión beta cerrada. Por favor, no difunda esta documentación.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **Marketo AI**.

1. En la ventana del mensaje, describa lo que está investigando. Incluya el posible cliente (por correo electrónico o nombre) y lo que esperaba que sucediera.

   >[!NOTE]
   >
   >Algunos ejemplos son: &quot;¿Por qué `john.smith@example.com` no alcanzó el MQL el mes pasado?&quot; o &quot;¿Por qué no se añadió Sato Hanako al programa de seminarios web del tercer trimestre?&quot;

1. Marketo AI extrae el registro del posible cliente y el historial relevante.

1. Revise la explicación. Marketo AI le informa del motivo específico por el que no se alcanzó el hito y, si es posible, de qué debería cambiar para que el posible cliente cumpla los requisitos.

1. Tome medidas basadas en la búsqueda: corrija un problema de datos, ajuste un filtro, actualice la puntuación del posible cliente o acepte que el resultado fue correcto.

## Casos de uso {#use-cases}

**Umbral de MQL no alcanzado**: un gerente de generación de demanda observa un posible cliente que las ventas señalaron como interesado, pero que nunca llegó a MQL. Preguntan: &quot;¿Por qué `david.chen@techcorp.com` no llegó a MQL?&quot; Marketo AI encuentra que la puntuación de comportamiento del posible cliente es de 42 (8 puntos por debajo del umbral de MQL de 50) y enumera las actividades de puntuación que contribuyeron. Pueden ver exactamente qué comportamientos empujarían al posible cliente por encima del umbral.

**Omisión de campaña debido a supresión**: un administrador de campaña pregunta por qué un contacto específico no recibió un correo electrónico de invitación que se envió al resto de la lista. Marketo AI encuentra que el contacto está en la lista de marketing suspendido, lo que los excluye automáticamente de todos los envíos de campañas. El gerente se dirige a ellos directamente para investigar por qué fueron suprimidos.

**Error de calificación del programa**: un especialista en operaciones de marketing está solucionando el problema de por qué un posible cliente que asistió a un seminario web no se agregó al programa de seguimiento posterior al evento. Marketo AI rastrea el problema: el posible cliente registrado, pero marcado como &quot;Sin programa&quot; en el programa de evento y el filtro de campaña de seguimiento requiere el estado &quot;Asistido&quot;. El estado se estableció incorrectamente en la integración.

## Cosas que debe tener en cuenta {#things-to-note}

* Lead Investigation explica qué ha pasado en función de la actividad registrada y la configuración de Marketo. No puede explicar las decisiones tomadas fuera de Marketo (por ejemplo, por qué un compañero eliminó manualmente un posible cliente).
* Si el historial de actividad de un posible cliente es muy largo, Marketo AI se centra en los eventos más recientes y relevantes relacionados con su pregunta.
* Lead Investigation es de solo lectura. Le informa de lo sucedido, pero no realiza cambios en el registro de posibles clientes ni en la pertenencia a programas.
* Para los problemas que resultan ser problemas de calidad de datos (falta de valores de campo, origen de cliente potencial incorrecto), la corrección debe realizarse manualmente en el registro de cliente potencial.
* Si la investigación revela un problema de lógica de campaña inteligente que afecta a muchos posibles clientes, utilice el control de calidad del programa para revisar la configuración completa del programa.
