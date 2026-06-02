---
description: Utilice la IA de Marketo para crear un programa de Marketo a partir de una información en lenguaje sencillo. Obtenga campañas inteligentes, programación y marcadores de posición de recursos listos para revisar y refinar.
title: Generar programas
badge: Beta
hide: true
source-git-commit: e055590a07ef9aa7cf6ebde42f6ea9f7420d7599
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Generar programas {#build-programs}

Describa una campaña de marketing en un lenguaje sencillo y Marketo AI crea la estructura del programa, con marcadores de posición de recursos y programación.

>[!PREREQUISITES]
>
>* Para usar esta característica, primero debe aceptar los términos de [Core Gen-AI y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.
>
>* Debe tener permiso para crear programas en su cuenta de Marketo.

>[!AVAILABILITY]
>
>Esta función se encuentra actualmente en versión beta cerrada. Por favor, no difunda esta documentación.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **Generar con IA**.

1. En la ventana de solicitud, escriba una descripción de la campaña que desea crear. Sea tan específico o general como desee (siempre puede refinarlo).

1. Marketo AI confirma su interpretación de la información y enumera lo que planea crear. Revise esto antes de que se cree.

1. Confirme y Marketo AI creará el programa en su entorno.

1. Abra el programa recién creado en Marketo y revise la estructura.

1. Reemplace los recursos de correo electrónico de marcador de posición por su contenido real.

1. Compruebe que los filtros de campaña inteligente y los pasos de flujo coinciden con la audiencia y la lógica deseadas.

1. Ejecute el agente [Validar programas](/help/marketo/product-docs/marketo-ai/agents/validate-programs.md) antes de activarlo.

## Casos de uso {#use-cases}

**Programa de registro de seminario web**: Un administrador de campaña escribe &quot;Cree un programa de registro de seminario web para nuestra demostración del producto de agosto. Envíe un correo electrónico de invitación, un recordatorio el día anterior y un seguimiento con el vínculo de grabación posterior&quot;. Marketo AI crea un programa con tres campañas inteligentes (invitación, recordatorio, seguimiento), correos electrónicos de marcador de posición para cada una y programación en función de la fecha del evento.

**Campaña de déclencheur de puntuación de posibles clientes**: Un especialista en operaciones de marketing escribe: &quot;Cree un programa que genere un déclencheur cuando un posible cliente alcance una puntuación de 50 y lo envíe a una lista inteligente de MQL&quot;. Marketo AI crea el programa con una campaña de déclencheur que escucha el cambio de puntuación y un paso de flujo que agrega el posible cliente a la lista de MQL.

**Nutrición para renovar la participación**: un gerente de generación de demanda pide una serie de renovación de la participación de tres correos electrónicos dirigida a los posibles clientes que no hayan participado en 90 días. Marketo AI crea la campaña por lotes con el filtro de inactividad, tres pasos de envío de correo electrónico con los pasos de espera adecuados entre ellos y un paso de flujo para actualizar el estado del posible cliente si alguien se vuelve a comprometer.

**Programa de seguimiento de eventos**: después de una feria comercial, un administrador pide a Marketo AI que cree un programa de seguimiento posterior al evento que envíe un correo electrónico de agradecimiento a los asistentes y un correo electrónico de agradecimiento a los inscritos que no se presentaron. Marketo AI crea dos campañas inteligentes, una para cada segmento, con los filtros y los marcadores de posición de correo electrónico correctos.

## Cosas que debe tener en cuenta {#things-to-note}

* Tenga una idea clara de lo que debe hacer la campaña, quién es la audiencia, qué acción déclencheur (o si es un envío por lotes) y cuál es el objetivo.
* No se requieren plantillas ni formularios por adelantado. Marketo AI crea la estructura y puede conectar recursos posteriormente (usted sigue siendo el responsable de escribir una copia del correo electrónico y configurar las páginas de aterrizaje).
* Marketo AI no puede acceder automáticamente a sus listas de audiencia existentes. Debe conectar los filtros de lista inteligente a los segmentos reales después de crear el programa.
* Los programas complejos de varios pasos con lógica de ramificación avanzada pueden necesitar un refinamiento manual después de su creación.
* Si su entorno de Marketo utiliza convenciones de nomenclatura o estructuras de carpetas, especifíquelas en la descripción para que el programa se cree en el lugar correcto.
