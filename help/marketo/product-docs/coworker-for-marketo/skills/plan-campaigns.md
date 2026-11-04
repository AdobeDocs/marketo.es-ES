---
description: Utilice CX Enterprise Coworker para Marketo Engage para convertir un informe de campaña en un plan de programa estructurado que incluya lógica de audiencia, correos electrónicos, tokens y comprobaciones de control de calidad.
title: Planificar campañas
source-git-commit: b1ab5ab541fd79c8c42fbcd018e23baf51337aac
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%
---
# Planificar campañas {#plan-campaigns}

Convierta un informe de campaña en un plan de implementación estructurado para Marketo Engage. La aptitud de las campañas de Plan describe la estructura del programa, la lógica de audiencia, los correos electrónicos, las campañas inteligentes, los tokens, los informes y las comprobaciones previas a la activación. El resultado es un informe descargable que aparece en el panel del espacio de trabajo.

>[!NOTE]
>
>Esta aptitud genera planes de implementación para programas de Marketo (documentos estructurados que indican a un sistema humano o de automatización exactamente cómo crear un programa en Marketo). No crea nada en Marketo. Hay una aptitud diferente para [crear programas](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md).

## Prerrequisitos {#prerequisites}

- Para un plan de programa, proporcione un resumen de la campaña con la información disponible, como los objetivos de la campaña, el público objetivo, los mensajes, la cronología y las métricas de éxito.
- Para mejorar un resumen o plan existente, proporcione el documento y describa los cambios que desee.
- Para empezar sin una breve, solicite una breve de ejemplo o pida un plan basado en un escenario de campaña común.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **[!UICONTROL CX Enterprise Coworker for Marketo Engage]**.

1. Seleccione la aptitud **[!UICONTROL Planificar campañas]** y haga clic en **[!UICONTROL Usar esta aptitud]**.

1. Elija lo que desea hacer:
   - Planifique un programa a partir de una información de campaña.
   - Genere un resumen de campaña de ejemplo.
   - Pulir un informe existente.
   - Revisar un plan de instalación existente.

1. Proporcione el resumen o el documento. Incluya cualquier cambio específico, requisitos de la campaña o convenciones de la organización.

1. Revise el informe generado en el panel del espacio de trabajo. Ábralo para revisar los detalles o descargar el informe.

1. Revise y apruebe el plan de configuración antes de crear el programa en Marketo Engage.

## Opciones de aptitudes {#skill-options}

### Planificar un programa {#plan-a-program}

Un plan de programa traduce los requisitos de la campaña en instrucciones para crear el programa. Según el resumen, puede incluir lo siguiente:

- **Resumen del programa:** Nombre de la campaña, objetivos, audiencia de destino y cronología.
- **Estructura de carpetas:** Carpetas locales recomendadas para correos electrónicos, campañas inteligentes e informes.
- **Listas inteligentes:** lógica de segmentación, definiciones de filtros y exclusiones requeridas.
- **Configuración de correo electrónico:** Líneas de asunto, texto de preencabezado, estructura de contenido, detalles de remitente y elementos de cumplimiento.
- **Campañas inteligentes:** Nombres de campañas, designación de déclencheur o lotes, pasos de flujo y recomendaciones de programación.
- **Tokens y campos:** Mis tokens, tokens requeridos y personalizados, y cualquier campo personalizado necesario con sus tipos y valores.
- **Flujo de Recorrido:** Secuencia de campaña, pasos de espera y lógica de decisión.
- **Informes y control de calidad:** métricas de éxito, informes recomendados y comprobaciones de validación previas a la activación.

### Crear un informe de ejemplo {#create-a-sample-brief}

Solicite una breve muestra cuando desee adaptar un ejemplo. Puede especificar un tema o un tipo de campaña, como un lanzamiento de producto o un seminario web. Si solicita un plan sin proporcionar información breve, la aptitud puede utilizar un escenario de muestra, como un seminario web de lanzamiento de productos, como base del plan.

### Pulir un informe o revisar un plan {#polish-a-brief-or-revise-a-plan}

La aptitud identifica el tipo de documento a partir de su contenido, en lugar de depender únicamente de la redacción de la solicitud.

Una **información de campaña** suele describir metas, audiencia, estrategia de mensajería, cronología y métricas de éxito. Un **plan de instalación** generalmente contiene detalles de implementación, como configuraciones de listas inteligentes, pasos de flujo de campañas inteligentes, definiciones de tokens, especificaciones de correo electrónico y requisitos técnicos.

Proporcione el documento y los cambios solicitados. Por ejemplo, si solicita pulir un plan pero proporciona un resumen de campaña, la aptitud trata el documento como un resumen. Si proporciona un plan de configuración y solicita revisar un informe, éste trata el documento como un plan.

## Integración de reglas organizativas {#organizational-rules-integration}

Los documentos de configuración deben incorporar las reglas de su organización desde el contexto del sistema.

### Convenciones de nomenclatura {#naming-conventions}

- Programas: `{{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}`
- Correos electrónicos: `{{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}`
- Campañas inteligentes: `{{NUMBER}}_{{TRIGGER_OR_BATCH}}_{{ACTION}}`

### Elementos necesarios {#required-elements}

- Tres carpetas locales (01 correos electrónicos, 02 campañas inteligentes, 03 informes)
- Cuatro tokens necesarios (eventDate, eventTime, replyToEmail, senderName)
- Filtros de exclusión (cancelación de suscripción, correo electrónico no válido, marketing suspendido, Incluido en la lista de bloqueados)
- Cumplimiento de las normas de correo electrónico (vínculo de cancelación de suscripción, dirección física)

### Control de calidad previo a la activación {#pre-activation-qa}

- Validación de patrón de nombre
- Confirmación de estructura de carpetas
- Verificación del filtro de exclusión
- Comprobaciones de elementos de cumplimiento

## Casos de uso {#use-cases}

**Planifique un programa de seminario web:** Proporcione el objetivo del seminario web, la audiencia, la cronología del evento y las necesidades de mensajería. El plan de configuración puede esbozar la estructura del programa, las especificaciones de correo electrónico, la secuencia de la campaña, los tokens y las comprobaciones de control de calidad.

**Generar informe de ejemplo:** Solicite un informe de ejemplo para un tipo de campaña y, a continuación, adáptelo a los detalles de la campaña antes de solicitar un plan de programa.

**Actualizar un plan de instalación existente:** Proporcione el plan y especifique los cambios, como actualizar la cronología, agregar un paso de campaña o revisar la lógica de audiencia.

## Próximos pasos {#next-steps}

Una vez finalizada una operación de planificación, los mensajes de seguimiento adecuados pueden incluir:

- &quot;Revisar este plan de configuración&quot;
- &quot;Obtener un resumen de campaña de muestra&quot;
- &quot;Crear este programa en Marketo&quot; (para crear un programa, debe usar la aptitud [crear programas](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md)).
