---
description: Use Colaborador para Marketo Engage para crear un programa de Marketo adaptando una plantilla existente. Obtenga campañas inteligentes, programación y marcadores de posición de recursos listos para revisar y refinar.
title: Generar programas
source-git-commit: fc1bcbdaa543e39127945852a6f89e69f2966c21
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%
---
# Generar programas {#build-programs}

Describa una campaña de marketing en un lenguaje sencillo y el colaborador de Marketo Engage adapta una plantilla de programa existente para adaptarla a sus necesidades, actualiza automáticamente el contenido del correo electrónico y crea recursos adicionales mediante la duplicación de la estructura de la plantilla.

Las [reglas organizativas](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"} de su organización guían el modo en que Coworker for Marketo Engage estructura y valida el programa durante la creación. Estas reglas garantizan que el nuevo programa se ajuste a las convenciones de nomenclatura, los tokens necesarios, la estructura de carpetas y los estándares de conformidad.

>[!PREREQUISITES]
>
>* Para usar esta característica, primero debe aceptar los términos de [Core Gen-AI y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.
>
>* Debe tener permiso para crear programas en su cuenta de Marketo y tener al menos un programa de Marketo existente para utilizarlo como plantilla. El programa de plantillas debe contener al menos un correo electrónico y una campaña inteligente.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el icono **Colaborador de Marketo Engage**.

1. Seleccione un programa de plantillas. Elija un programa existente que coincida con su tipo de campaña (por ejemplo, Correo electrónico, Seminario web, Nutrición).

1. En la ventana de solicitud, escriba una descripción de la campaña que desea crear. Sea tan específico o general como desee (siempre puede refinarlo).

1. El colaborador de Marketo Engage confirma su interpretación de la información y enumera lo que planea crear. Revise esto antes de que se cree.

1. Confirm y Coworker para Marketo Engage crea el programa en su entorno.

1. Abra el programa recién creado en Marketo y revise la estructura.

1. Reemplace los recursos de correo electrónico de marcador de posición por su contenido real.

1. Compruebe que los filtros de campaña inteligente y los pasos de flujo coinciden con la audiencia y la lógica deseadas.

1. Después de completar todos los refinamientos manuales (configurar la lógica de Smart Campaign, finalizar filtros, personalizar el contenido del correo electrónico), ejecute [Validar programas](/help/marketo/product-docs/coworker-for-marketo/skills/validate-programs.md) para asegurarse de que los cambios cumplan con las reglas de organización antes de activarlos.

## Casos de uso {#use-cases}

**Programa de registro de seminario web**: Un administrador de campaña escribe &quot;Cree un programa de registro de seminario web para nuestra demostración del producto de agosto. Envíe un correo electrónico de invitación, un recordatorio el día anterior y un seguimiento con el vínculo de grabación posterior&quot;. Un compañero de Marketo Engage crea un programa con tres campañas inteligentes (invitación, recordatorio, seguimiento), correos electrónicos de marcador de posición para cada una y programación en función de la fecha del evento.

**Campaña de déclencheur de puntuación de posibles clientes**: Un especialista en operaciones de marketing escribe: &quot;Cree un programa que genere un déclencheur cuando un posible cliente alcance una puntuación de 50 y lo envíe a una lista inteligente de MQL&quot;. Compañero de Marketo Engage crea el programa con una campaña de déclencheur que escucha el cambio de puntuación y un paso de flujo que agrega el posible cliente a la lista de MQL.

**Nutrición para renovar la participación**: un gerente de generación de demanda pide una serie de renovación de la participación de tres correos electrónicos dirigida a los posibles clientes que no hayan participado en 90 días. Compañero de Marketo Engage crea la campaña por lotes con el filtro de inactividad, tres pasos de envío de correo electrónico con los pasos de espera adecuados entre ellos y un paso de flujo para actualizar el estado del posible cliente si alguien se vuelve a comprometer.

**Programa de seguimiento de eventos**: después de una feria comercial, un administrador le pide a Marketo Engage que cree un programa de seguimiento posterior al evento que envíe un correo electrónico de agradecimiento a los asistentes y un correo electrónico de agradecimiento a los inscritos que no se presentaron. Un compañero de Marketo Engage crea dos campañas inteligentes, una para cada segmento, con los filtros y los marcadores de posición de correo electrónico correctos.

>[!NOTE]
>
>En cada ejemplo anterior, el colaborador clona una plantilla de programa existente (un correo electrónico o programa de evento simple con estructura básica) y crea los correos electrónicos y campañas adicionales duplicando los recursos de plantilla y actualizando su contenido. Los pasos y filtros de flujo de la campaña inteligente se adaptan siempre que sea posible, pero puede requerir un refinamiento manual para que coincida con la lógica de campaña específica.

## Cosas que debe tener en cuenta {#things-to-note}

* Tenga una idea clara de lo que debe hacer la campaña, quién es la audiencia, qué acción déclencheur (o si es un envío por lotes) y cuál es el objetivo.
* Se requiere la selección de plantillas. Elija una plantilla con al menos un correo electrónico y una campaña inteligente. La herramienta no puede funcionar con plantillas vacías.
* El contenido del correo electrónico se genera automáticamente, pero los filtros de campañas inteligentes y los pasos de flujo siguen siendo manuales. Debe configurar la lógica después de la creación para que coincida con el comportamiento deseado de la campaña.
* Los recursos adicionales se crean mediante duplicación. Si el informe llama a 4 correos electrónicos pero la plantilla tiene 1, la herramienta crea 3 duplicados. Revise todos para mantener la coherencia; heredan el diseño y la estructura de la plantilla.
* El compañero de Marketo Engage no puede acceder automáticamente a sus listas de audiencia existentes. Debe configurar manualmente los filtros de la lista inteligente para que se dirijan a los segmentos reales después de crear el programa.
* Los programas complejos de varios pasos con lógica de ramificación avanzada pueden necesitar un refinamiento manual después de su creación.
* Si su entorno de Marketo utiliza convenciones de nomenclatura o estructuras de carpetas, especifíquelas en la descripción para que el programa se cree en el lugar correcto.
