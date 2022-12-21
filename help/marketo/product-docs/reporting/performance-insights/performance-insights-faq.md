---
unique-page-id: 12979858
description: Preguntas frecuentes sobre perspectivas de rendimiento - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre Perspectivas de rendimiento
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# Preguntas frecuentes sobre Perspectivas de rendimiento {#performance-insights-faq}

## ¿Cuál es la definición de &quot;éxito&quot; en la pestaña Participación? {#what-is-the-definition-of-success-in-the-engagement-tab}

El éxito es una medida de la interacción significativa en Marketo. El objetivo de un programa es crear una interacción significativa con la persona o el cliente potencial. El éxito se marca cuando una persona alcanza el estado que logra ese objetivo. Puede asistir a un seminario web, hacer clic en un vínculo de un correo electrónico o rellenar un formulario web. El éxito varía en función del canal del programa.

>[!NOTE]
>
>En un programa de seminario web, puede haber varios estados, como: Invitado, registrado y asistido. Invitados o registrados no son interacciones significativas porque la gente no ve el seminario web. La asistencia se considera un éxito en este caso.

## ¿Funcionará MPI con algún CRM? {#will-mpi-work-with-any-crm}

Sí. Técnicamente, MPI no interactúa directamente con CRM para la sincronización de datos. MPI utiliza datos almacenados en la Data Warehouse de Marketo Analytics. Dado que la sincronización de CRM se produce en la aplicación de Administración de posibles clientes, cualquier CRM compatible con Marketo integrado con la aplicación Administración de posibles clientes mostrará los datos correctamente. Sin embargo, los campos de oportunidad de CRM sí que deben asignarse correctamente a los campos de oportunidad de Marketo.

## No tengo ningún otro producto de Marketing Analytics (ARB, RCE, RCA, Análisis de programas). ¿Funcionará MPI para mí? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI es un complemento independiente de la aplicación Administración de posibles clientes. No requiere el uso de otros productos de análisis.

## RCA también me muestra los datos de rendimiento del programa. ¿Hay alguna diferencia entre los datos mostrados en MPI y RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

No. MPI obtiene datos del mismo almacén de datos que RCA. Por lo tanto, no verá diferencias de datos entre los dos. RCA le permite crear sus propios informes sobre la marcha. MPI le permite acceder a tableros visuales fáciles de entender.

## No quiero que algunos de mis programas (p. ej., Operativos) aparezcan en MPI. ¿Cómo puedo controlar la visibilidad de programas específicos? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Puede controlar la visibilidad de sus programas estableciendo el comportamiento de Analytics de sus programas en Operativo. Esto hará que el programa se excluya de los cálculos analíticos.

>[!NOTE]
>
>Obtenga más información sobre la configuración del comportamiento analítico [here](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Estoy ejecutando una campaña multicanal para el lanzamiento de un nuevo producto. ¿Cómo puedo ver el rendimiento de esta campaña en todos los canales en un solo lugar? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Recomendamos que, para los programas que forman parte de una campaña de este tipo, utilice etiquetas de programa. Las etiquetas de programa se sincronizan automáticamente con MPI y puede filtrarlas en todos los tableros MPI para ver el rendimiento de la campaña multicanal.

## ¿Tendré acceso a la configuración de atribución si no tengo RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Puede acceder a la configuración de atribución si tiene MPI, independientemente de si tiene RCA o no.

## Recibo una alerta en MPI cuando inicio sesión diciéndome que mi configuración de atribución es incorrecta. ¿Qué está mal? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcula si se incluyen o no todas las oportunidades en analytics. Si no es así, se le pedirá que considere la posibilidad de cambiar la configuración de atribución (Explícito, implícito, híbrido) para incluir más oportunidades.

También puede que falten oportunidades debido a que el costo del programa no aparece en sus programas. Revise el comportamiento de Analytics de sus programas. Pueden ser:

1. Predeterminado: el comportamiento predeterminado es que el programa se incluiría en MPI SOLO si hay al menos un coste de período, incluso uno con cero dólares asignados.

1. Inclusivo : esta opción garantiza que el programa esté disponible en MPI independientemente de si ha incluido o no un coste de período.

1. [Operativo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Esta opción hace que el programa no se muestre en MPI.

>[!NOTE]
>
>Costo de período **has** que se configurará para los informes de éxito y nombres nuevos en el panel Participación. Este tablero utiliza los datos de Coste de Período para acumular los éxitos y los nuevos nombres. Si no se configura Costo de período, el panel de participación no informará correctamente independientemente de la configuración de comportamiento de Analytics anterior.

## ¿Por qué estoy perdiendo algunas oportunidades en MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Dos razones clave por las que puede estar perdiendo oportunidades en MPI son:

1. La configuración de atribución se establece en Explícito pero las oportunidades no tienen asignados roles de contacto
1. El costo de período no está incluido en los programas

MPI calcula si se incluyen o no todas las oportunidades en analytics. Si no es así, se le pedirá que considere la posibilidad de cambiar la configuración de atribución (Explícito, implícito, híbrido) para incluir más oportunidades.

También puede que falten oportunidades debido a que el costo del programa no aparece en sus programas. La alerta aparecerá, pero no le indica a qué programas faltan costes. Revise la configuración de su programa para incluir los costes, para asegurarse de que todos sus programas y oportunidades estén incluidos en MPI.

## ¿Por qué no veo los filtros Campos personalizados, Tipo de oportunidad y ABM en el panel Participación? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Los campos personalizados, el tipo de oportunidad y los filtros ABM son atributos relacionados con una oportunidad. El panel Participación le permite medir su participación y la adquisición de posibles clientes tanto si están asociados a una oportunidad como si no. Dado que el panel Participación no tiene en cuenta la oportunidad, los campos personalizados, el tipo de oportunidad y los filtros ABM no se aplican.

## Deseo utilizar un campo de oportunidad de Salesforce personalizado para los informes de ingresos en lugar del campo Cantidad de oportunidad de Salesforce estándar. ¿El MPI me permitirá hacer eso? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sí. [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) puede reasignar el campo Cantidad de oportunidad de Marketo a un campo de oportunidad de Salesforce personalizado siempre que el tipo de campo sea moneda. Dado que MPI apunta al campo Cantidad de oportunidad de Marketo , MPI puede utilizar los datos del campo personalizado reasignado de Salesforce.

>[!NOTE]
>
>Después de la reasignación, MPI mostrará los datos en adelante. La cantidad histórica no cambiará.

## Si no utilizo oportunidades, ¿puedo seguir usando MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI está diseñado para permitirle medir el rendimiento del programa desde la parte superior del canal hasta el impacto en los ingresos. Si no utiliza oportunidades, podrá:

* Vea el rendimiento de sus programas de formación para la participación de la audiencia.
* Ver el rendimiento de los programas de adquisición de posibles clientes.
* Vea el rendimiento de las campañas multicanal a través de etiquetas de programa.
* Consulte las tendencias de participación de la audiencia de los últimos 12 meses.
* Guarde y exporte datos de rendimiento en PowerPoint.

## ¿Puedo medir el éxito de las estrategias basadas en cuentas en MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sí. MPI se integra con [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) para extraer listas de cuentas ABM en MPI sin problemas. Puede usar el filtro Lista de cuentas ABM para elegir la lista ABM por la que filtrar los datos.

## ¿La atribución está disponible al instante cuando compro MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Las funcionalidades de atribución de Marketo están disponibles para nuestros clientes cuando compran MPI. Sin embargo, [configuración adecuada](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) es necesario para garantizar que las oportunidades y los datos de los programas se transfieran correctamente a MPI.

## ¿Qué tengo que hacer para configurar la atribución? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuración de oportunidad

   1. Asegúrese de que las oportunidades se sincronizan con su CRM
   1. Si la configuración de atribución está establecida en Explícito, asegúrese de que las funciones de contacto en oportunidades se rellenen
   1. Se recomienda cambiar la configuración de atribución a híbrido
   1. Configuración del programa

      1. Incluir el costo del programa en los programas
      1. Revise el comportamiento de Analytics para indicar si un programa debe incluirse en Analytics
      1. Establezca los criterios de éxito para cada canal que tenga
      1. Vincular persona a programas

         1. Asegúrese de que el Programa de adquisición y la Fecha de adquisición se hayan establecido para cada persona de la base de datos para que funcione la Atribución de primer toque.
         1. Asegúrese de que los programas establezcan estados de éxito para las personas de la base de datos

>[!TIP]
>
>Todos los pasos de configuración necesarios se detallan en [este artículo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## ¿Cuál es la diferencia entre MPI y Program Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

El Analizador de programas le permite comparar sus programas con un máximo de cuatro medidas. MPI le permite analizar su contribución de canal y programa hacia una métrica seleccionada, como Éxito, Nuevas oportunidades creadas, etc. También le permite ver la tendencia del canal de 12 meses en función de una métrica específica que haya elegido.

## ¿Cuál es la diferencia entre MPI y el Report Builder avanzado? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

El Report Builder avanzado (a veces denominado RCE) está diseñado para informes de autoservicio (o específicos), que normalmente se realizan mediante operaciones de marketing. MPI está diseñado para proporcionar a los responsables de marketing y a los especialistas en marketing acceso con un clic al análisis de rendimiento. Se requiere una configuración mínima.

## ¿Qué ha pasado con la opción &quot;Año anterior&quot; del filtro de fechas de la contribución? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Se ha eliminado temporalmente la selección &quot;Año anterior&quot;. Aún tiene la opción de ver los datos de rendimiento de todo el año mediante la selección Intervalo de fechas personalizado .
