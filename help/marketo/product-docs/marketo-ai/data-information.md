---
description: Revise el ámbito de datos de Marketo AI, los controles de gobernanza y las consideraciones PII en los flujos de trabajo clave, como la importación de posibles clientes, el control de calidad del programa y la normalización de datos.
title: Hoja de información de datos de Marketo AI
badge: beta
source-git-commit: 06d77c31c729de70033696662fb6191eb527dedf
workflow-type: tm+mt
source-wordcount: '1454'
ht-degree: 0%

---

# Hoja de información de datos de Marketo AI {#data-information}

Marketo AI es una función nativa y agéntica de Adobe Marketo Engage que permite a los equipos de operaciones de marketing automatizar flujos de trabajo seleccionados mediante la interacción en lenguaje natural, incluida la importación de posibles clientes, la validación de programas, la normalización de datos, la creación de programas, la investigación de posibles clientes, los análisis y la orientación sobre productos. La IA de Marketo funciona dentro del entorno de Marketo Engage existente de un usuario y utiliza una infraestructura administrada por Adobe para el razonamiento y la orquestación de la IA.

**Entorno de usuario:** Marketo AI funciona dentro de un entorno de Marketo Engage existente y no presenta una nueva ruta de uso compartido usuario a usuario.

**Ámbito de datos:** El servicio procesa los datos de marketing B2B estándar que ya están presentes en el entorno del usuario, incluidos los registros de posibles clientes, los datos de programas y la actividad de campañas inteligentes.

**Servicios de IA:** Marketo AI aprovecha un mazo de cables de IA creado por Adobe y usa Azure OpenAI GPT-4.1 y Claude en AWS Bedrock para el razonamiento de IA, con herramientas de MCP de Marketo que admiten la ejecución de acciones de productos.

**Gobernanza:** los resultados generados por IA permanecen dentro del entorno del usuario y están sujetos a los controles de gobernanza, residencia y retención existentes.

**Transparencia:** los resultados generados por IA se pueden revisar a través del historial de conversaciones y auditorías para admitir la supervisión del usuario.

## Controles de acceso y despliegue

### Importar posibles clientes

**Función:** procesa los datos de posibles clientes proporcionados por el usuario para su asignación, normalización, deduplicación e importación en Marketo Engage.

### Control de calidad del programa

**Función:** evalúa los programas de Marketo comparándolos con las reglas organizativas definidas por los usuarios en un archivo de marcado de aptitudes, como los estándares de nomenclatura, el estado de aprobación, el cumplimiento de las normas de correo electrónico y la lógica de flujo.

### Crear programa a partir de información breve

**Función:** utiliza mensajes en lenguaje natural para generar estructuras de programa de Marketo, incluidas campañas inteligentes, pasos de flujo y marcadores de posición de contenido, directamente en el entorno del usuario.

### Agentes a los que llamar

**Función:** ejecuta acciones de IA activadas por acciones de flujo dentro de los pasos de flujo de Smart Campaign para casos de uso como validación, normalización y detección de bots.

### Investigación principal

**Función:** Proporciona un análisis conversacional de por qué una persona progresó o no a un hito al examinar la ejecución de pasos de flujo y la pertenencia a listas inteligentes.

### Medición y análisis

**Función:** Superficie el análisis del rendimiento de la campaña y del programa, incluidas las recomendaciones y las perspectivas de la causa raíz.

### Conocimiento del producto

**Función:** proporciona instrucciones sobre prácticas recomendadas y procedimientos de Marketo a través de una capa de conocimientos compartidos que se utiliza en la experiencia del agente.

## Casos de uso

Además de los enumerados, considere la posibilidad de utilizar la IA de Marketo para diagnosticar y solucionar problemas operativos complejos (errores de sincronización de CRM, errores de ganchos web, análisis de causas raíz de entrega de correo electrónico, discrepancias de campos), realice auditorías en toda la cuenta (capacidad de entrega de correo electrónico, conformidad con el centro de suscripciones, revisiones de campañas inteligentes, evaluaciones del modelo de puntuación) y acelere la creación de programas a partir de informes y plantillas (programas de eventos, campañas de correo electrónico en varios idiomas, configuraciones de seminarios web). La IA de Marketo está diseñada para proporcionar clasificación de posibles clientes asistida por IA y enriquecimiento de datos a escala, análisis de rendimiento con recomendaciones de corrección y depuración guiada de configuraciones técnicas como scripts de Velocity y modelos de ciclo vital.

## Disponibilidad y estado de despliegue

**Elegibilidad:** La habilitación inicial del usuario está limitada a los usuarios elegibles de Marketo Engage que hayan aceptado el Adobe Gen AI Rider.

**Aprovisionamiento:** El acceso se administra mediante los controles de habilitación de productos existentes y el aprovisionamiento de indicadores de características dentro de la experiencia de Marketo Engage.

**Modelo de despliegue:** La implementación progresa a través de Alpha y Private Beta antes de una expansión pública de Beta más amplia.

**Ámbito geográfico:** La versión inicial está destinada a usuarios globales de Marketo Engage, excluida China continental.

**Ámbito del sector:** El despliegue actual no incluye capacidades específicas verticales para sectores altamente regulados como la atención médica, los servicios financieros, el gobierno o la defensa.

## Documentación y asistencia

**Documentación:** La documentación de Experience League se está ampliando como parte de la preparación general para la disponibilidad.

**Modelo de soporte:** El enfoque de soporte actual incluye la admisión de comentarios del usuario, el horario de oficina y una comunidad Experience League de Marketo AI.

**Supervisión del servicio:** Adobe identifica la observabilidad, los paneles de comentarios y los mecanismos de evaluación de la calidad como componentes importantes de la madurez del lanzamiento y la mejora continua.

## Exclusiones y datos fuera de ámbito

**No hay nuevos datos de categoría especial:** Marketo AI no introduce nuevos procesos para datos de salud, financieros, de ubicación precisa, biométricos u otros datos de categoría especial.

**No hay una nueva ruta para compartir:** El servicio no crea un nuevo mecanismo de uso compartido de contenido de usuario a usuario.

**Salidas contenidas en el usuario:** Las salidas generadas por IA permanecen dentro del entorno de Marketo Engage existente del usuario bajo los controles de gobernanza existentes.

**Exclusiones actuales:** El despliegue inicial excluye China continental y no proporciona capacidades específicas verticales para industrias altamente reguladas.

## Uso de Azure OpenAI y Claude en AWS Bedrock

En esta sección se explica cómo Azure OpenAI admite flujos de trabajo de Marketo AI. Cualquier diagrama relacionado o descripción de flujo debe leerse junto con los controles descritos aquí, incluidas las limitaciones en el ámbito de los datos, la supervisión del usuario y la formación sobre modelos.

**Propósito:** Azure OpenAI GPT-4.1 se usa para el razonamiento conversacional y la orquestación de flujos de trabajo impulsados por agentes.

**Ámbito de datos:** Las entradas se limitan a datos de marketing B2B estándar que ya están presentes en el entorno de Marketo Engage del usuario y son necesarias para cumplir con el flujo de trabajo solicitado.

**Salida de IA:** Las salidas de IA están determinadas por las indicaciones y la configuración del usuario, y las funciones de IA de Marketo no toman ninguna decisión de forma autónoma sin la configuración del usuario.

**Formación:** Adobe no usa datos de usuario para entrenar o ajustar modelos OpenAI de Azure para este servicio.

**Supervisión del usuario:** las salidas generadas por IA siguen siendo revisables en Marketo Engage a través de las capacidades de historial de conversaciones y auditorías.

## Retención y almacenamiento de datos

**Salidas contenidas por el usuario:** Las salidas generadas por IA, como listas de posibles clientes limpias, informes de control de calidad, estructuras de programas generadas y datos normalizados, permanecen dentro del entorno de Marketo Engage del usuario.

**Alineación de control:** Los datos de salida siguen estando sujetos a los controles de control, residencia y retención de datos existentes del usuario en Marketo Engage.

**No hay un nuevo almacén entre usuarios:** El servicio no introduce una ruta de acceso de uso compartido de datos entre usuarios independiente.

## Ubicaciones de procesamiento y almacenamiento de datos

Esta sección resume los entornos en los que funciona Marketo AI y dónde se produce el procesamiento. Si el documento incluye diagramas regionales o imágenes de infraestructura, esos materiales deben entenderse como representaciones de alto nivel de la ubicación del servicio y el flujo de procesamiento, en lugar de esquemas de red exhaustivos.

**Entorno de aplicación:** Marketo AI funciona dentro del entorno de Adobe Marketo Engage existente del usuario.

**Procesamiento de IA:** Marketo AI usa Azure OpenAI GPT-4.1 y Claude en AWS Bedrock para el razonamiento conversacional y la orquestación de tareas.

**Ubicación de datos de usuario:** Los datos de usuario y los resultados generados por IA permanecen dentro del entorno Marketo Engage del usuario y están sujetos a los controles de residencia, control y retención existentes del usuario.

**No hay ningún almacén independiente entre usuarios:** El servicio no introduce una capa de almacenamiento o de uso compartido de datos entre usuarios independiente.

## Ámbito de datos por tipo de flujo de trabajo

Los datos procesados por Marketo AI están determinados por el patrón de uso del usuario y el flujo de trabajo específico invocado. No todos los flujos de trabajo requieren el procesamiento de datos de nivel de posible cliente.

### Flujos de trabajo que solo aprovechan los metadatos de la campaña (sin información de posibles clientes)

* Creación de programas a partir de información breve: genera estructuras de programas, campañas inteligentes, pasos de flujo y marcadores de posición de contenido a partir de instrucciones en lenguaje natural
* Clonación y traducción de correo electrónico: duplica y traduce el contenido de HTML de correo electrónico, las líneas de asunto y la copia de marketing entre las variantes de idioma
* Auditoría de campañas: revisa las configuraciones de campañas inteligentes, las definiciones de déclencheur/filtros, la lógica de flujo y las convenciones de nomenclatura
* Validación de control de calidad del programa: evalúa los programas según las reglas definidas por el usuario para el cumplimiento, el estado de aprobación y la integridad estructural
* Revisiones del centro de suscripciones y la arquitectura del programa: analiza la lógica de campaña y la estructura del programa
* Conocimiento del producto e instrucciones sobre las prácticas recomendadas: proporciona respuestas de procedimientos de Marketo desde una capa de conocimiento compartida

### Flujos de trabajo que aprovechan los registros de nivel de cliente potencial (campos de contacto B2B estándar)

* Investigación y solución de problemas de posibles clientes: examina los valores de los campos de posibles clientes individuales proporcionados por el usuario, el historial de actividades y la progresión del ciclo vital para diagnosticar por qué un posible cliente alcanzó o no el estado MQL o calificó para una campaña de marketing
* Importación y normalización de posibles clientes: procesa los datos de posibles clientes proporcionados por el usuario, incluidos nombres, direcciones de correo electrónico, números de teléfono y campos de empresa, para la asignación, limpieza y deduplicación
* Clasificación y enriquecimiento de posibles clientes: evalúa los registros de posibles clientes con una puntuación definida por el usuario o lógica de clasificación (por ejemplo, posibles clientes válidos frente a spam para el estado de la base de datos, personas con fines de personalización, posibles clientes empresariales con posibles clientes de correo electrónico corporativo frente a posibles clientes)
* Auditorías de calidad de datos y capacidad de entrega: analiza los datos de participación de nivel de posible cliente, los patrones de rechazo y los registros duplicados para identificar problemas de estado de la base de datos
* Análisis del rendimiento de Campaign: muestra patrones de participación de posibles clientes, datos de conversión y composición de audiencias para admitir el análisis del rendimiento

### Minimización de datos por diseño

* En todos los casos, los datos enviados al modelo de IA se limitan a lo necesario para cumplir la solicitud de usuario específica dentro de ese flujo de trabajo
* Marketo AI sigue los permisos de Marketo Engage existentes del usuario; no proporciona acceso a registros de posibles clientes, campos o programas más allá de lo que el usuario tiene permiso para ver a través de la interfaz de usuario del producto
* Los usuarios que deseen limitar el procesamiento de datos de posibles clientes pueden restringir el acceso a los flujos de trabajo de investigación de la herramienta a través de los controles de funciones y permisos de Marketo Engage existentes, al tiempo que conservan el acceso completo a las capacidades de IA estructural y administrativa

### Sin exposición a datos incrementales

La API funciona como un acelerador de permisos de usuario existentes, no como una ruta de escalación. Un usuario que no puede ver ciertos campos, programas o particiones de posibles clientes en la interfaz de usuario de Marketo Engage tampoco puede mostrar esos datos a través de la IA de Marketo. El servicio no omite las reglas de partición, los permisos de nivel de campo o las restricciones del espacio de trabajo.
