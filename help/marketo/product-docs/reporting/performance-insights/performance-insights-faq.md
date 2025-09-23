---
unique-page-id: 12979858
description: Preguntas frecuentes sobre las perspectivas de rendimiento - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre perspectivas de rendimiento
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# Preguntas frecuentes sobre [!UICONTROL perspectivas de rendimiento] {#performance-insights-faq}

## ¿Cuál es la definición de &quot;correcto&quot; en la ficha [!UICONTROL Participación]? {#what-is-the-definition-of-success-in-the-engagement-tab}

El éxito es una medida de la interacción significativa en Marketo. El propósito de un programa es crear una interacción significativa con la persona o el cliente potencial. El éxito se marca cuando una persona alcanza el estado que logra ese objetivo. Puede asistir a un seminario web, hacer clic en un vínculo de un correo electrónico o rellenar un formulario web. El éxito varía según el canal del programa.

>[!NOTE]
>
>En un programa de seminario web, puede haber varios estados, como Invitado, Registrado y Asistido. Las invitaciones o los registros no son interacciones significativas porque las personas no ven el seminario web. En este caso, la asistencia se considera un éxito.

## ¿Funcionará MPI con algún CRM? {#will-mpi-work-with-any-crm}

Sí. Técnicamente, MPI no interactúa directamente con CRM para la sincronización de datos. MPI utiliza datos almacenados en Marketo Analytics Data Warehouse. Dado que la sincronización CRM se produce en la aplicación de administración de posibles clientes, cualquier CRM compatible con Marketo integrado con la aplicación de administración de posibles clientes mostrará los datos correctamente. Sin embargo, los campos de oportunidad de CRM deben asignarse correctamente a los campos de oportunidad de Marketo.

## No tengo ningún otro producto de Marketing Analytics (ARB, RCE, RCA, análisis de programas). ¿MPI funcionará para mí? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI es un complemento independiente de la aplicación Lead Management. No requiere el uso de ningún otro producto de análisis.

## RCA también me muestra los datos de rendimiento del programa. ¿Hay alguna diferencia entre los datos mostrados en MPI y RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

No. MPI obtiene datos del mismo almacén de datos que RCA. Por lo tanto, no verá ninguna diferencia de datos entre los dos. RCA le permite crear sus propios informes sobre la marcha. MPI le permite acceder a paneles visuales fáciles de entender.

## No deseo que algunos de mis programas (por ejemplo, Operativos) aparezcan en MPI. ¿Cómo controlo la visibilidad de programas específicos? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Puede controlar la visibilidad de sus programas estableciendo el comportamiento de Analytics de sus programas en Operativo. Esto hará que el programa se excluya de los cálculos de Analytics.

>[!NOTE]
>
>Obtenga más información acerca de cómo establecer el comportamiento de análisis [aquí](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Estoy ejecutando una campaña multicanal para el lanzamiento de un nuevo producto. ¿Cómo puedo ver el rendimiento de esta campaña en todos los canales en un solo lugar? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Recomendamos que, para los programas que forman parte de dicha campaña, utilice etiquetas de programa. Las etiquetas de programas se sincronizan automáticamente con MPI y puede filtrarlas en todos los paneles MPI para ver el rendimiento de su campaña multicanal.

## ¿Tendré acceso a la configuración de atribución si no tengo RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Puede acceder a la configuración de atribución si tiene MPI, independientemente de si tiene RCA o no.

## Recibo una alerta en MPI cuando inicio sesión diciéndome que la configuración de atribución es incorrecta. ¿Qué sucede? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcula si todas sus oportunidades se incluyen en Analytics o no. Si no es así, se le pedirá que considere la posibilidad de cambiar la configuración de atribución (Explícito, Implícito, Híbrido) para incluir más oportunidades.

También es posible que pierda oportunidades debido a la falta de Coste del programa en sus programas. Revise el comportamiento de Analytics de sus programas. Pueden ser:

1. Predeterminado: el comportamiento predeterminado es que el programa se incluiría en MPI SOLAMENTE si hay al menos un costo de período, incluso uno con cero dólares asignados.

1. Inclusivo: esta opción garantizará que el programa esté disponible en MPI independientemente de si ha incluido o no un coste de período.

1. [Operativo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs): esta opción hace que el programa no se muestre en MPI.

>[!NOTE]
>
>El costo de período **tiene** que configurar para los informes de éxito y nombres nuevos en el panel de participación. Este tablero utiliza datos de coste de período para sumar éxitos y nuevos nombres. Si el coste del período no está configurado, el panel de participación no presentará informes correctamente, independientemente de la configuración de comportamiento de Analytics anterior.

## ¿Por qué me estoy perdiendo algunas oportunidades en MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Dos razones clave por las que puede estar perdiendo oportunidades en MPI son:

1. La configuración de atribución se establece en Explícita, pero las oportunidades no tienen asignadas funciones de contacto
1. El coste del periodo no está incluido en los programas

MPI calcula si todas sus oportunidades se incluyen en Analytics o no. Si no es así, se le pedirá que considere la posibilidad de cambiar la configuración de atribución (Explícito, Implícito, Híbrido) para incluir más oportunidades.

También es posible que pierda oportunidades debido a la falta de Coste del programa en sus programas. La alerta aparecerá, pero no indica a qué programas faltan costes. Revise la configuración de su programa para incluir los costos y asegurarse de que todos sus programas y oportunidades estén incluidos en el MPI.

## ¿Por qué no veo los filtros Campos personalizados, Tipo de oportunidad y ABM en el panel de participación? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Los campos personalizados, el tipo de oportunidad y los filtros ABM son todos atributos relacionados con una oportunidad. El panel de participación le permite medir su participación y la adquisición de posibles clientes, estén o no asociados a una oportunidad. Dado que el panel Participación no tiene en cuenta la oportunidad, los campos personalizados, el tipo de oportunidad y los filtros ABM no se aplican.

## Deseo utilizar un campo de oportunidad de Salesforce personalizado para los informes de ingresos en lugar del campo de importe de oportunidad de Salesforce estándar. ¿MPI me permitirá hacer eso? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sí. [Soporte de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) puede reasignar el campo Cantidad de oportunidades de Marketo a un campo de oportunidad de Salesforce personalizado siempre y cuando el tipo de campo sea moneda. Dado que MPI señala al campo de cantidad de oportunidad de Marketo, MPI puede utilizar los datos del campo personalizado de Salesforce reasignado.

>[!NOTE]
>
>Después de la reasignación, el MPI mostrará los datos a partir de ahora. La cantidad histórica no se cambiará.

## Si no utilizo oportunidades, ¿puedo seguir utilizando MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI está diseñado para permitirle medir el rendimiento del programa desde la parte superior del canal hasta el impacto en los ingresos. Si no utiliza las oportunidades, aún podrá hacer lo siguiente:

* Vea el rendimiento de sus programas de nutrición para la participación de la audiencia.
* Vea el rendimiento de sus programas de adquisición de posibles clientes.
* Vea el rendimiento de las campañas multicanal mediante etiquetas de programa.
* Consulte las tendencias de participación de la audiencia de los últimos 12 meses.
* Guarde y exporte datos de rendimiento en PowerPoint.

## ¿Puedo medir el éxito de las estrategias basadas en cuentas en MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sí. MPI se integra perfectamente con [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) para extraer listas de cuentas ABM a MPI. Puede utilizar el filtro Lista de cuentas ABM para elegir la lista ABM deseada para filtrar los datos.

## ¿La atribución está disponible al instante cuando compro MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Las funcionalidades de atribución de Marketo están disponibles para nuestros clientes cuando compran MPI. Sin embargo, se requiere la [configuración adecuada](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) para garantizar que las oportunidades y los datos del programa fluyen correctamente a MPI.

## ¿Qué tengo que hacer para configurar la atribución? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuración de oportunidad

   1. Asegúrese de que las oportunidades se sincronicen con su CRM
   1. Si la configuración de Atribución está establecida en Explícito, asegúrese de que las funciones de contacto de las oportunidades se rellenen
   1. Se recomienda cambiar la configuración de Atribución a Híbrida
   1. Configuración del programa

      1. Incluir el coste del programa en los programas
      1. Revise el comportamiento de Analytics para indicar si un programa debe incluirse en Analytics
      1. Defina los criterios de éxito para cada canal que tenga
      1. Vincular persona a programas

         1. Asegúrese de que el programa de adquisición y la fecha de adquisición se hayan establecido para cada persona de la base de datos para que funcione la Atribución de primer contacto.
         1. Asegúrese de que los programas establecen estados de éxito para las personas de la base de datos

>[!TIP]
>
>Todos los pasos de configuración requeridos se detallan en [este artículo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## ¿Cuál es la diferencia entre MPI y el Analizador de programas? {#whats-the-difference-between-mpi-and-the-program-analyzer}

El analizador de programas le permite comparar sus programas con un máximo de cuatro medidas. MPI le permite analizar la contribución de su canal y programa hacia una métrica elegida como Éxito, Nuevas oportunidades creadas, etc. También le permite ver la tendencia del canal a 12 meses en función de una métrica específica que haya elegido.

## ¿Cuál es la diferencia entre MPI y Advanced Report Builder? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

El Report Builder avanzado (a veces denominado RCE) está diseñado para la creación de informes de autoservicio (o específicos), que suelen realizar las operaciones de marketing. MPI está diseñado para proporcionar a los líderes de marketing y a los especialistas en marketing acceso con un solo clic al análisis de rendimiento. Se requiere una configuración mínima.

## ¿Qué ha pasado con la opción &quot;Año anterior&quot; en el filtro de fechas de Contribución? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Hemos eliminado temporalmente la selección &quot;Año anterior&quot;. Sigue existiendo la opción de ver los datos de rendimiento de todo el año mediante la selección de Intervalo de fechas personalizado.
