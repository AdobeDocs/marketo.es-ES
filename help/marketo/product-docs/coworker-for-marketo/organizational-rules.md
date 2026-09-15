---
description: La descripción se incluye aquí.
title: Reglas organizativas
source-git-commit: 0949e5193333d56943a5c9a52c1715ecbcb274f3
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%
---
# Reglas organizativas {#organizational-rules}

Las reglas organizativas definen los estándares de operaciones de marketing y los requisitos de control en un único documento que guía al compañero en la creación de programas, la planificación de campañas y los flujos de trabajo de validación.

## ¿Qué son las reglas organizativas? {#what-are-organizational-rules}

Las reglas organizativas son un documento de configuración basado en Markdown que captura los estándares de campaña de su organización:

* Convenciones de nomenclatura para programas, correos electrónicos y campañas inteligentes
* Recursos y estructura necesarios (carpetas, tokens e informes)
* Requisitos de cumplimiento (vínculos de cancelación de suscripción, parámetros de UTM, filtros de exclusión)
* Prácticas recomendadas (diseño de correo electrónico, configuración de listas inteligentes)

Cada instancia de Marketo incluye reglas organizativas predeterminadas. Puede personalizarlos para que reflejen las necesidades de gobernanza específicas de su organización.

## Dónde se utilizan las reglas organizativas {#where-organizational-rules-are-used}

Las reglas organizativas guían a los compañeros de trabajo en tres aptitudes:

| Habilidad | Aplicación de las reglas |
| --- | --- |
| Generar programas | Las reglas guían la creación de la estructura del programa, la asignación de nombres y la configuración inicial. El compañero marca cualquier problema de cumplimiento en su informe antes de crear el programa. |
| Planificar campañas | Las reglas informan sobre cómo los compañeros de trabajo estructuran las campañas inteligentes, los filtros y los pasos de flujo en función de sus estándares. |
| Validar programas | Las reglas definen lo que comprueba el colaborador al validar los programas antes de la activación. |

## Cómo acceder y personalizar las reglas organizativas {#how-to-access-and-customize-organizational-rules}

1. En Mi Marketo, haga clic en el icono **Colaborador de Marketo Engage**.
1. Haga clic en el icono de engranaje.
1. Seleccione la ficha **Reglas organizativas**.
1. Revise las reglas predeterminadas (que vienen precompletadas con las prácticas recomendadas de operaciones de marketing).
1. Edite las reglas para que coincidan con las de su organización:

   * Convenciones de nomenclatura (programas, correos electrónicos, campañas)
   * Estructura de carpetas requerida
   * Tokens y campos obligatorios
   * Normas de cumplimiento y exclusión

1. Actualice el número de versión cuando realice cambios.
1. Guarde los cambios. Todas las aptitudes de colaborador utilizarán inmediatamente las reglas personalizadas.

## Estructura de reglas organizativas {#organizational-rules-structure}

Las reglas organizativas tienen el formato Markdown con YAML frontmatter:

```markdown
---
name: Your Organization Name — Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## ⚠️ REQUIRED Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## Prácticas recomendadas para reglas organizativas {#best-practices-for-organizational-rules}

* **Comenzar con valores predeterminados**: revise las reglas predeterminadas antes de personalizar. Reflejan las prácticas recomendadas del sector para las operaciones de marketing.
* **Mantener las reglas centradas**: solo incluye los requisitos que importan a tu organización. Las reglas innecesarias crean ruido y reducen las puntuaciones de cumplimiento de manera innecesaria.
* **Realizar comprobaciones automáticas y manuales**:

  * Comprobaciones automatizadas: convenciones de nomenclatura, carpetas requeridas, uso de tokens (los compañeros pueden verificarlas).
  * Comprobaciones manuales: diseño visual de correo electrónico, conformidad con la marca, lógica de campaña (el colaborador las marcará como pasos de revisión manuales).

* **Equilibrar la rigidez con la flexibilidad**: las reglas demasiado estrictas pueden ralentizar la creación del programa. Las reglas demasiado laxas no detectan problemas de cumplimiento importantes.
* **Versión de las reglas**: Actualice el número de versión cuando realice cambios significativos para que su equipo sepa que se han actualizado los estándares de gobernanza.
* **Comunicar cambios**: cuando actualice las reglas organizativas, informe a su equipo de operaciones de marketing qué ha cambiado y por qué.

## Lo que el compañero puede y no puede validar {#what-coworker-can-and-cannot-validate}

El compañero puede validar (comprobaciones automatizadas):

* Las convenciones de nomenclatura coinciden con sus patrones
* Existe una estructura de carpetas requerida
* Los tokens requeridos están establecidos
* El correo electrónico tiene un vínculo de cancelación de suscripción y elementos de pie de página necesarios
* Los vínculos externos incluyen parámetros de UTM
* Los nombres de campañas inteligentes siguen las convenciones

El compañero NO PUEDE validar (se requiere revisión manual):

* Lógica de filtro de lista inteligente (limitación de API: debe configurar los filtros manualmente)
* Lógica de paso de flujo de campaña inteligente (limitación de API: debe configurar los flujos manualmente)
* Procesamiento visual y capacidad de respuesta del correo electrónico (requiere inspección visual)
* Conformidad con la marca y tono de mensajería (requiere criterio humano)
* Reglas de segmentación de contenido dinámico (limitación de API)

Cuando el compañero encuentra algo que no puede validar, lo marca como un paso de revisión manual en el flujo de trabajo.

## Puntuación de cumplimiento {#compliance-scoring}

Al utilizar Validar programas, el colaborador calcula una puntuación de conformidad en función de lo siguiente:

* **Comprobaciones superadas** — El compañero verificó el cumplimiento y no encontró problemas
* **Comprobaciones con errores** — El compañero encontró infracciones de las reglas de organización
* **Pasos de revisión manual**: elementos que requieren verificación humana (NO se contabilizan en su puntuación)

Un programa puede tener un cumplimiento del 100% y seguir precisando pasos de revisión manuales; se excluyen del cálculo de puntuación.

## Ejemplos de personalización de reglas organizativas {#examples-of-organizational-rules-customization}

**Ejemplo 1: convención de nomenclatura estricta**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

Utilícelo si su organización requiere un control estricto entre regiones y unidades de negocio.

**Ejemplo 2: Nomenclatura flexible con prefijo obligatorio**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

Utilice esta opción si desea coherencia en los códigos de región pero flexibilidad en el resto.

**Ejemplo 3: Reglas mínimas (enfoque en el cumplimiento)**

```markdown
# Email Compliance — REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

Utilícelo si su organización prioriza el cumplimiento de las normas sobre la coherencia de nomenclatura/estructura.

## Resolución de problemas {#troubleshooting}

**Q: he actualizado las reglas de organización, pero el compañero sigue usando las reglas antiguas.**

R: Los cambios se aplican inmediatamente a los nuevos programas y validaciones. Si está trabajando en un programa existente, actualice el navegador o inicie un nuevo flujo de trabajo de Compañero para ver las reglas actualizadas.

**Q: ¿Puedo volver a las reglas predeterminadas?**

R: Sí. Vaya a **Configuración** > **Reglas organizativas** y haga clic en **Restablecer a valores predeterminados**. Las reglas personalizadas se sustituirán por las reglas predeterminadas.

**Q: Mi puntuación de cumplimiento es baja a pesar de que el programa tiene buena apariencia.**

R: Compruebe qué comprobaciones están fallando. Revise las reglas de organización para ver si son demasiado estrictas para los flujos de trabajo actuales o si necesita ajustar el programa para que cumpla con sus estándares.
