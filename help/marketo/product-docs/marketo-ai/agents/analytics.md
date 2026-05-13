---
description: Hable con la inteligencia artificial aplicada a Marketo sobre los datos de rendimiento de Marketo Engage. Haga preguntas en lenguaje sencillo y obtenga respuestas basadas en su entorno de Marketo.
title: Analytics
beta: true
hide: true
source-git-commit: cb30495d71d5b4d4fe86d33eed0677eaee882c5e
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Analytics {#analytics}

Analytics le permite hablar sobre los datos de rendimiento de Marketo. Haga preguntas en lenguaje sencillo y obtenga respuestas basadas en su entorno de Marketo.

>[!PREREQUISITES]
>
>Debe tener acceso a los programas e informes que está consultando.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **Generar con IA**.

1. En la ventana de solicitud, haga una pregunta de rendimiento. Sea específico sobre el periodo de tiempo o el programa si tiene uno en mente.

1. Revise el resumen que devuelve Marketo AI. Incluirá métricas clave como tasas de apertura, tasas de clics, tasas de conversión y recuentos de posibles clientes según lo que haya preguntado.

1. Haga preguntas de seguimiento para explorar áreas específicas (por ejemplo, &quot;¿Qué correo electrónico de ese programa tuvo la tasa de clics más alta?&quot; o &quot;¿En qué se diferencia eso del último trimestre?&quot;).

## Casos de uso {#use-cases}

**Revisión trimestral del programa**: Un administrador de generación de demanda se está preparando para una reunión de revisión de campaña. Se preguntan: &quot;¿Cómo funcionaron mis programas de nutrición del segundo trimestre en general?&quot; Marketo AI devuelve las tasas de apertura, las tasas de clics para abrir, las tasas de cancelación de suscripción y el número de personas/posibles clientes que progresaron a MQL en todos los programas de nutrición del segundo trimestre, con una nota sobre los programas que superaron el promedio del grupo.

**Comparando dos campañas**: un administrador de campaña ejecutó dos versiones de una serie de invitaciones a seminarios web con líneas de asunto diferentes. Preguntan: &quot;¿Cómo se compara el programa del seminario web de abril con el de marzo en términos de tasa de registro?&quot; Marketo AI devuelve los números de registro de cada uno y resalta la diferencia, para que puedan ver qué enfoque funcionó mejor.

**Búsqueda de contenido de alto rendimiento**: un especialista en operaciones de marketing desea saber qué recursos de correo electrónico generaron la mayor participación el mes pasado. Preguntan: &quot;¿Qué correos electrónicos tuvieron las tasas de clics más altas en mayo?&quot; Marketo AI devuelve una lista clasificada de recursos de correo electrónico con tasas de clics, para que puedan identificar qué ha resonado e informar las decisiones de contenido futuras.

## Cosas que debe tener en cuenta {#things-to-note}

* **Las respuestas de Analytics se basan en los datos disponibles en su instancia de Marketo**: si no se realiza el seguimiento de un programa o no se captura una métrica, Marketo AI no podrá generar informes al respecto.
* **Los intervalos de fechas muy grandes o las preguntas amplias pueden devolver resúmenes de alto nivel en lugar de detalles granulares**: Por ejemplo, &quot;¿Cómo funcionaron todos mis programas en los últimos dos años?&quot;
* **Marketo AI puede mostrar datos, pero no puede realizar cambios** en los programas o informes según lo que encuentre.
* **Para obtener informes personalizados detallados con filtros y desgloses específicos**, las herramientas de informes integradas de Marketo o una integración de BI pueden ser más apropiadas.
* **La atribución en campañas multitáctiles requiere la configuración adecuada del programa**: Marketo AI informará sobre lo que se rastrea, no deducirá la atribución que no se configuró.
