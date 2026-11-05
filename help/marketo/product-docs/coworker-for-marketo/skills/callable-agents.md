---
description: Utilice agentes a los que llamar en CX Enterprise Coworker para Marketo Engage para ejecutar pasos de IA en campañas inteligentes que limpien, clasifiquen, enriquezcan o eliminen datos de posibles clientes.
title: Agentes a los que llamar
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
source-git-commit: 93193d2bf1f673472bb52d806864bfb083216cab
workflow-type: tm+mt
source-wordcount: '2004'
ht-degree: 1%
---
# Agentes a los que llamar {#callable-agents}

Los agentes a los que llamar le permiten utilizar un agente de IA como paso en una campaña inteligente de Marketo Engage. Cree un agente en CX Enterprise Coworker para Marketo Engage, elija los campos de posible cliente que lee y actualiza y publíquelo para su uso en campañas. Los agentes pueden ayudar a limpiar los datos, clasificar los posibles clientes, enriquecer la información que falta o filtrar los envíos de formularios.

>[!PREREQUISITES]
>
>Debe tener el permiso **Administrador de acceso** en Marketo Engage.

## Antes de empezar {#before-you-begin}

- Decida qué campos de posibles clientes debe leer el agente y qué campos debe actualizar. Cada entrada y salida debe asignarse a un campo de posible cliente de Marketo Engage.
- Confirme que los campos de salida son actualizables. No se admiten campos de solo lectura ni campos de miembros de programa.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **[!UICONTROL CX Enterprise Coworker for Marketo Engage]**.

1. Seleccione **[!UICONTROL agentes a los que llamar]** en el panel de navegación izquierdo. La lista muestra el nombre, la fecha de creación, el creador y el estado de cada agente. Busque por nombre u ordene por nombre o fecha de creación.

1. Seleccione **[!UICONTROL Crear agente al que llamar]**. Elija una plantilla o deje vacío el selector de plantillas para empezar desde cero.

1. Escriba un **[!UICONTROL nombre de agente]** y escriba **[!UICONTROL instrucciones de agente]** que describan cómo procesar cada posible cliente.

1. En **[!UICONTROL Campos de posible cliente para enviar]**, agregue los campos de posible cliente que el agente necesita como entradas. En **[!UICONTROL Campos de posible cliente para actualizar]**, agregue cada valor que el agente debe devolver y asígnelo a un campo de posible cliente actualizable.

1. Seleccione **[!UICONTROL Guardar]** para guardar un borrador o **[!UICONTROL Guardar y publicar]** para que el agente esté disponible en Marketo Engage.

1. Abra una campaña inteligente y seleccione la ficha **[!UICONTROL Flujo]**. En la sección Marketing de la lista de pasos de flujo, busque **Llamar al agente: _[Nombre del agente]_**y arrástrelo al flujo.

1. Pruebe la campaña con un pequeño conjunto de posibles clientes. Revise el registro de actividad y confirme que los campos de salida se actualizan según lo esperado antes de activar la campaña para todos los posibles clientes.

## Cosas que debe tener en cuenta {#things-to-note}

- Un agente al que llamar procesa cada posible cliente de forma independiente. Marketo Engage envía los valores de posibles clientes asignados al agente, escribe los valores devueltos en los campos de posibles clientes asignados y continúa con el siguiente paso de la campaña.
- Puede crear y administrar agentes a los que llamar en CX Enterprise Coworker para Marketo Engage. No se requiere conexión externa.
- Los agentes publicados no pueden editarse. Para cambiar un agente que ya se ha publicado, debe crear un nuevo agente y actualizar las campañas inteligentes correspondientes.

## Crear un agente {#create-an-agent}

### Crear un agente desde cero {#create-an-agent-from-scratch}

Deje el selector de plantillas vacío. El formulario comienza con un campo de entrada vacío y un campo de salida vacío. Introduzca el nombre y las instrucciones y, a continuación, configure los campos de entrada y salida para que coincidan con la regla de negocio.

### Empezar desde una plantilla {#start-from-a-template}

Elija una plantilla para rellenar previamente las instrucciones, los campos de entrada y los campos de salida. El agente se guarda como su propia copia, que puede editar o eliminar. Si elimina un agente creado a partir de una plantilla, la plantilla volverá a estar disponible en el selector.

| Plantilla | Finalidad | Entradas | Salidas |
| --- | --- | --- | --- |
| Nombre de empresa Normalizer | Limpia los nombres de las empresas eliminando sufijos legales, corrigiendo errores tipográficos comunes y aplicando mayúsculas de marca estándar. | Compañía | Empresa normalizada (texto); confianza (número, 0-1) |
| Teléfono E.164 Formatter | Aplica formato a los números de teléfono según el estándar internacional E.164. | Teléfono | Teléfono normalizado (texto); confianza (número) |
| Puesto de trabajo estandarizado | Estandariza los cargos y deriva la antigüedad. | Título | Título normalizado (texto); antigüedad (nivel C, vicepresidente, director, administrador, individuo o desconocido); confianza |
| Detector de bots y spam | Indica los envíos de bots o formularios de correo no deseado. | Correo electrónico, Nombre, Apellido, Empresa, Teléfono | Es bot (verdadero/falso); confianza; motivo; indicadores (separados por comas) |
| Detector de correo electrónico desechable | Identifica direcciones de correo electrónico temporales o desechables. | Correo electrónico | Es bot (verdadero/falso); confianza; motivo; tipo de correo electrónico (desechable, personal o empresarial) |
| Clasificador de posibles clientes | Segmentos de posibles clientes por tamaño de empresa, sector, personalidad e intención. | Empresa, cargo, correo electrónico, empleados, ingresos | Segmento (empresa, mercado medio, pyme, inicio o desconocido); sector; persona; nivel de intención (alto, Medium o bajo); confianza |
| Enriquecimiento de plomo | Infiere los detalles del posible cliente que faltan de la información disponible. | Correo electrónico, título, compañía | Empresa deducida, departamento, antigüedad, es el responsable de la toma de decisiones (verdadero/falso), es B2B (verdadero/falso), confianza |
| Investigación de empresa | Genera inteligencia de ventas a partir de información de la compañía. | Empresa, sitio web, descripción | Consulte la plantilla para ver la lista completa |

### Escribir instrucciones efectivas {#write-effective-instructions}

- Incluya reglas generales y ejemplos en las instrucciones del agente. Utilice las instrucciones de campo para especificar las expectativas de un resultado individual.
- Sea específico. Por ejemplo, &quot;Eliminar sufijos legales como Inc, LLC y Corp&quot; es más claro que &quot;limpiar nombres de compañías&quot;.
- Incluya ejemplos de entradas y salidas esperadas, especialmente para casos puntuales.
- Indique lo que el agente debe devolver cuando no pueda decidir, como &quot;Si no está seguro, devuelva el valor original&quot;.
- Agregue un resultado de confianza para que la lógica de campaña pueda enrutar los resultados de baja confianza para su revisión.
- Mantenga las indicaciones concisas. Las peticiones más cortas se ejecutan más rápido y cuestan menos.

## Guardar, publicar y administrar agentes {#save-publish-and-manage-agents}

### Guardar como borrador o publicar {#save-as-a-draft-or-publish}

Seleccione **[!UICONTROL Guardar]** para guardar el agente como borrador. Los borradores se pueden editar, pero no están disponibles como pasos del flujo de campaña inteligente. Seleccione **[!UICONTROL Guardar y publicar]** cuando el agente esté listo. Marketo Engage hace que el agente esté disponible como paso de flujo y le devuelve a la lista de agentes con una confirmación de publicación. Seleccione **[!UICONTROL Cancelar]** para salir sin guardar.

| Estado | Significado | Acción disponible |
| --- | --- | --- |
| Borrador | El agente se guarda, pero no está disponible en Marketo Engage. | Edítela y luego selecciona **[!UICONTROL Guardar y publicar]** cuando esté listo. |
| Publicadas | El agente está disponible en campañas inteligentes. Los agentes publicados están congelados. | Utilice el agente publicado o cree un nuevo agente para realizar cambios. |
| Error de publicación | Marketo Engage rechazó el agente, por ejemplo, porque un nombre de campo de salida está reservado. Pero el agente sigue guardado como borrador. | Edite el agente, corrija el campo denominado en el mensaje y vuelva a publicar. |

### Editar, comprobar el uso o eliminar {#edit-check-usage-or-delete}

- Seleccione **[!UICONTROL Editar]** en un borrador para cambiarlo. **[!UICONTROL Guardar]** le mantiene en la página y muestra una confirmación de &quot;Agente guardado&quot;. También puede seleccionar **[!UICONTROL Guardar y publicar]**, **[!UICONTROL Cancelar]** o **[!UICONTROL Eliminar]**.
- Los agentes publicados están congelados porque las campañas inteligentes pueden depender de ellos. Cree un nuevo agente para realizar cambios.
- Compruebe **[!UICONTROL Utilizado por]** para ver qué campañas inteligentes hacen referencia a un agente antes de eliminar un agente o cambiar su configuración de campaña.
- No puede eliminar un agente mientras lo siga utilizando una campaña inteligente. Elimine el paso de flujo del agente de cada campaña enumerada y, a continuación, elimine el agente.

## Integración de reglas organizativas {#organizational-rules-integration}

### Convenciones de nomenclatura {#naming-conventions}

- **Nombre del agente:** de 1 a 100 caracteres y único dentro de la suscripción. El nombre también se utiliza en el paso de flujo de la campaña inteligente. Elija un nombre reconocible, como `Company Name Normalizer`.
- **Nombre del campo de salida:** Use letras, dígitos y guiones bajos. El nombre debe comenzar con una letra o guion bajo, ser único y no tener más de 64 caracteres.
- **Nombres reservados:** Algunos nombres de salida están reservados para el uso del sistema. Si se rechaza un nombre, elija otro, como `qualificationReason` en lugar de `reason`.

### Elementos obligatorios y campos compatibles {#required-elements-and-supported-fields}

- Asigne cada campo de entrada a un campo de posible cliente de Marketo Engage antes de guardar.
- Configure al menos un campo de salida. Asigne cada salida a un campo de posible cliente actualizable; los campos de solo lectura no están disponibles en el selector de campos.
- No se admiten los campos de miembros de programa. El selector de campos solo muestra los campos de posibles clientes.
- Los tipos de salida admitidos son **Text**, **Number** y **True/False**.
- Para devolver una lista, utilice un valor de texto separado por comas y describa el formato esperado en las instrucciones de campo.
- Cada ejecución correcta devuelve exactamente los campos de salida configurados.

### Límites {#limits}

| Configuración | Límite |
| --- | --- |
| Nombre del agente | 1-100 caracteres; únicos en la suscripción |
| Instrucciones del agente | De 1 a 4.000 caracteres |
| Campos de entrada | Hasta 20; cada uno debe asignarse a un campo de posible cliente |
| Campos de salida | 1-20; cada uno debe asignarse a un campo de posible cliente actualizable |
| Nombre del campo de salida | Hasta 64 caracteres; letras, dígitos y guiones bajos; comienza con una letra o guion bajo; único |
| Instrucciones del campo de salida | Hasta 512 caracteres |
| Posibles clientes por solicitud | Hasta 1000 posibles clientes de Marketo Engage, procesados en paralelo |

## Filtrado de contenido y gestión de datos {#content-screening-and-data-handling}

Cuando crea un agente o edita sus instrucciones, Marketo Engage las analiza para detectar infracciones de directivas, la inyección de mensajes y los intentos de filtración de datos. Algunos ejemplos son las solicitudes para revelar credenciales o anular el comportamiento del agente. Si el contenido está marcado, se bloquea el guardado y puede aparecer un mensaje, como &quot;El mensaje contiene contenido restringido&quot; o &quot;Solicitar moderación de contenido fallida&quot;. Revise el texto y vuelva a guardar.

- **Acceso:** La administración de agentes requiere el permiso **Administrador de acceso**. Los agentes y el historial de llamadas están aislados por suscripción.
- **Protección de datos de posibles clientes:** Los datos de posibles clientes se pasan por separado de las instrucciones del agente, con protecciones que tratan los valores de posibles clientes como datos en lugar de como comandos.
- **Directiva de contenido:** Si los datos de un posible cliente infringen la directiva de contenido del proveedor de IA, ese posible cliente recibe una actividad de error en lugar de un resultado.
- **Retención:** Las cargas de solicitud y respuesta, incluidos los valores de los campos de posibles clientes enviados al agente, se mantienen en el historial de llamadas durante 30 días para admitir la solución de problemas y, a continuación, se eliminan automáticamente.

## Ejecución de los agentes a los que llamar en una campaña {#how-callable-agents-run-in-a-campaign}

1. Cuando se ejecuta la campaña, Marketo Engage envía al agente los valores de los campos de posibles clientes asignados para cada posible cliente correspondiente.
1. El agente procesa cada posible cliente de forma independiente y devuelve los campos de salida configurados.
1. Marketo Engage escribe los resultados en los campos de posibles clientes asignados. Los campos modificados también aparecen como actividades de cambio de valor de datos estándar.
1. La campaña pasa al siguiente paso.

El procesamiento es asincrónico. El paso de flujo espera un resultado hasta la ventana de espera de paso de flujo en Marketo Engage. Si un posible cliente falla (por ejemplo, debido a un tiempo de espera), ese posible cliente recibe una actividad de error y otros posibles clientes continúan. Cada resultado aparece en el registro de actividad del posible cliente para el agente al que llamar.

Utilice campos de salida en la lógica de campaña. Por ejemplo, la rama en **Is bot** para enrutar los envíos de correo no deseado de forma diferente, o la rama en **confianza** para enviar resultados de baja confianza a un paso de revisión.

## Control de calidad previo a la activación {#pre-activation-qa}

Antes de activar una campaña para todos los posibles clientes:

- Ejecute la campaña con un pequeño conjunto de posibles clientes de prueba.
- Revise el registro de actividad de cada posible cliente y confirme que los campos de salida se actualizan correctamente.
- Casos extremos de prueba, incluidos valores que faltan e entradas inusuales.
- Confirme que las ramas de campaña gestionan valores como una baja confianza o una clasificación de bot/spam como estaba previsto.

## Casos de uso {#use-cases}

- **Limpieza de datos:** Estandarizar nombres de compañías, formatear números de teléfono a E.164 y normalizar títulos de trabajos cuando se crean o importan posibles clientes.
- **Detección de bots y correo no deseado:** Compruebe los envíos en busca de nombres de galimatías, correos electrónicos sospechosos y números de teléfono de dígitos repetidos; bifurque la campaña en función del resultado.
- **Detección de correo electrónico desechable:** Identifique las direcciones de correo electrónico temporales y envíelas de forma diferente a las direcciones comerciales.
- **Clasificación del posible cliente:** El segmento lleva por tamaño de compañía, sector, persona e intención de admitir el enrutamiento o la puntuación.
- **Enriquecimiento del posible cliente:** Infiera detalles que faltan, como el departamento, la antigüedad o si un posible cliente es un encargado de la toma de decisiones.
- **Reglas personalizadas:** Cree una comprobación o categorización de sí/no que se pueda describir como una regla de procesamiento de posibles clientes, como marcar posibles clientes de una región o industria.

## Resolución de problemas {#troubleshooting}

| Problema | Resolución |
| --- | --- |
| **Agentes** no aparece en la navegación. | Pida al administrador de Marketo Engage que conceda el permiso **Administración de acceso**. |
| Guardar está bloqueado con un mensaje de contenido. | Revise las instrucciones del agente o las instrucciones de campo para eliminar el contenido marcado y, a continuación, vuelva a guardar. |
| El estado del agente es **Error de publicación**. | Edite el agente, corrija el campo mencionado en el mensaje y seleccione **Guardar y publicar**. |
| No puede editar un agente publicado. | Los agentes publicados están congelados. Cree un nuevo agente para realizar cambios. |
| No puede eliminar un agente. | Elimine su paso de flujo de cada campaña inteligente enumerada como con el agente y, a continuación, elimínelo. |
| Un nombre de campo se comunica como reservado. | Elija un nombre de campo de salida diferente, como `qualificationReason`, y vuelva a guardar. |
| Algunos posibles clientes reciben una actividad de error. | Compruebe el registro de actividad del posible cliente. Los errores individuales, incluidos los tiempos de espera o las violaciones de las políticas de contenido, no afectan a otros posibles clientes. |
| Resultados inesperados. | Especifique las instrucciones, agregue ejemplos, perfeccione las instrucciones de campo y vuelva a probarlas con un pequeño conjunto de posibles clientes. |

## Próximos pasos {#next-steps}

- Revise la lista **Utilizado por** del agente y confirme qué campañas inteligentes lo usará.
- Pruebe el paso de flujo con un pequeño grupo de posibles clientes y valide los registros de actividad y los campos de salida.
- Utilice los campos de salida para añadir ramas de campaña para clasificaciones o resultados de baja confianza.
- Elimine el paso de flujo del agente de todas las campañas antes de eliminar el agente.
