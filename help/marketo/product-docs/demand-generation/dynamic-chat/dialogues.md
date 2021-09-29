---
description: 'Cuadros de diálogo: Documentos de Marketo: Documentación del producto'
title: Cuadros de diálogo
hide: true
hidefromtoc: true
source-git-commit: 50effc2aa1fc94251b4b75bec6dcc34bf3df8a2c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Cuadros de diálogo {#dialogues}

Los cuadros de diálogo son las conversaciones individuales de chat que configurará. Aprenda a personalizarlos visualmente, a determinar en qué páginas aparecen y a decidir qué se dice y quién lo ve.

## Crear un cuadro de diálogo nuevo {#create-a-new-dialogue}

1. Haga clic en **Diálogos**.

PICC

1. Haga clic en el botón **Create New**.

PICC

1. Introduzca un nombre (la descripción es opcional), establezca el nivel de prioridad y haga clic en **Guardar**.

PICC

>[!NOTE]
>
>El nivel de prioridad determina dónde aparece el cuadro de diálogo en la lista (por ejemplo: priority = 1 significa que estará en la parte superior).

## Criterios de audiencia {#audience-criteria}

Al igual que las listas inteligentes de Marketo, los atributos de criterios de audiencia le permiten definir la audiencia de destino. Puede dirigirse a posibles clientes conocidos o desconocidos mediante atributos inferidos, de posibles clientes o de empresa (o una combinación de estos).

Hay _muchas_ combinaciones de atributos entre las que elegir. En este ejemplo estamos dirigiendo todos los posibles clientes conocidos de California que trabajan en una empresa con más de 50 empleados.

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

<table>
 <tr>
  <td><strong>Mensaje</strong></td>
  <td>Utilícelo cuando desee realizar una instrucción sin necesidad de respuesta (por ejemplo: "¡Hola! Todos los artículos tienen hoy un 25% de descuento con el código SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Pregunta</strong></td>
  <td>Utilícelo cuando desee hacer una pregunta de opción múltiple, de la que proporcione las respuestas disponibles (por ejemplo: ¿Qué tipo de vehículo le interesa? Respuestas = SUV, Compacta, Camión, etc.).</td>
 </tr>
 <tr>
  <td><strong>Captura de información</strong></td>
  <td>Utilícelo cuando desee recopilar información. Los tres campos entre los que elegir son Dirección de correo electrónico, Número de teléfono y Texto (que permite al visitante escribir su propio mensaje).</td>
 </tr>
 <tr>
  <td><strong>Programador de citas</strong></td>
  <td>Proporciona al visitante un calendario de fechas disponibles para programar un seguimiento. La disponibilidad del calendario refleja [el siguiente agente en línea] (/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).</td>
 </tr>
 <tr>
  <td><strong>Objetivo</strong></td>
  <td>Esta es la única tarjeta que los visitantes no verán. Depende de usted determinar en qué momento se logra un objetivo dentro del chat específico (por ejemplo: si su objetivo es recopilar el correo electrónico del visitante, coloque la tarjeta Goal después de Captura de información en el flujo).</td>
 </tr>
</table>

POSIBLE SECCIÓN PROPIA

MOSTRAR EJEMPLOS A CONTINUACIÓN

## Informes {#reports}

Texto
