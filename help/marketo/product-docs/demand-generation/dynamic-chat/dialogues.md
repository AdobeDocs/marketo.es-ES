---
description: 'Cuadros de diálogo: Documentos de Marketo: Documentación del producto'
title: Cuadros de diálogo
hide: true
hidefromtoc: true
source-git-commit: 1a1d4cb7e013253ce7189150486ba03ea02d877d
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Cuadros de diálogo {#dialogues}

Los cuadros de diálogo son las conversaciones de chat específicas que configuró. Pueden personalizarse por el aspecto, así como por lo que se dice y quién lo ve.

## Crear un cuadro de diálogo nuevo {#create-a-new-dialogue}

1. Haga clic en **Diálogos**.

PICC

1. Haga clic en el botón **Create New**.

PICC

1. Introduzca un nombre (la descripción es opcional), establezca el nivel de prioridad y haga clic en **Guardar**.

PICC

>[!NOTE]
>
>EXPLICAR NIVEL DE PRIORIDAD

## Criterios de audiencia {#audience-criteria}

Al igual que las listas inteligentes de Marketo, los atributos de criterios de audiencia le permiten definir la audiencia de destino.

Hay varios atributos entre los que elegir. En este ejemplo estamos dirigiendo todos los posibles clientes conocidos de California que trabajan en una empresa con más de 50 empleados.

1. Coja el atributo Estado de posible cliente y arrástrelo a la derecha.

PICC

1. __ Isis establecido de forma predeterminada. En el campo Seleccionar valores , escriba CA (también puede hacer clic en la lista desplegable y seleccionar en la lista).

PICC

1. Coja el atributo Tamaño de la empresa y arrástrelo a la derecha.

PICC

1. Haga clic en la lista desplegable de operadores y seleccione Bueno que no.

PICC

1. Escriba 50 y haga clic en cualquier otra parte de la pantalla para guardar.

PICC

CÓMO CAPTURAR POSIBLES CLIENTES

NOTA: Puede que se mencione cómo funciona inferir/mostrar un caso de uso diferente, el correo electrónico principal está vacío

## Agregar grupos {#add-groups}

También tiene la opción de agrupar atributos, en caso de que desee tener todos los atributos junto con &quot;cualquiera&quot; de otro.

FINALICE ESTO

## Destino {#target}

Aquí es donde introduce las URL específicas en las que desea que se muestre un cuadro de diálogo específico.

Formatos aceptables:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>El uso de un asterisco actúa como comodín global. Por lo tanto, `https://*.website.com` colocaría el cuadro de diálogo en todas las páginas del sitio, incluidos los subdominios (por ejemplo: `support.website.com`). Y `https://website.com/folder/*` colocaría el cuadro de diálogo en cada página HTML de la carpeta siguiente (por ejemplo: en este caso, digamos que la carpeta es &quot;deportes&quot;, así que: website.com/sports/baseball.html, website.com/sports/football.html, etc.).

## Diseñador de secuencias {#stream-designer}

El diseñador de secuencias contiene diferentes tarjetas que puedes añadir para dar forma a la conversación de chat.

TABLA

Mensaje: Utilícelo cuando desee realizar una instrucción sin necesidad de respuesta (por ejemplo: &quot;¡Hola! Todos los artículos tienen hoy un 25% de descuento con el código SAVE25.&quot;)

Pregunta: Utilícelo cuando desee hacer una pregunta de opción múltiple, de la que proporcione las respuestas disponibles (por ejemplo: ¿Qué tipo de vehículo le interesa? Respuestas = SUV, Compacta, Camión, etc.)

Captura de información: Utilícelo cuando desee recopilar información. Los tres campos entre los que elegir son Dirección de correo electrónico, Número de teléfono y Texto (que permite al visitante escribir su propio mensaje).

Programador de citas: Proporciona al visitante un calendario de fechas disponibles para programar un seguimiento. La disponibilidad del calendario refleja [el siguiente agente en la línea](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).

Objetivo: Esta es la única tarjeta que los visitantes no verán. Depende de usted determinar en qué momento se logra un objetivo dentro del chat específico (por ejemplo: si su objetivo es recopilar el correo electrónico del visitante, coloque la tarjeta Goal después de Captura de información en el flujo ).

POSIBLE SECCIÓN PROPIA

MOSTRAR EJEMPLOS A CONTINUACIÓN