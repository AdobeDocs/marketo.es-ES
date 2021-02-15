---
unique-page-id: 12979858
description: Preguntas más frecuentes sobre perspectivas de rendimiento - Documentos de marketing - Documentación del producto
title: Preguntas más frecuentes sobre perspectivas de rendimiento
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# Preguntas más frecuentes sobre perspectivas de rendimiento {#performance-insights-faq}

## ¿Cuál es la definición de &quot;éxito&quot; en la ficha Participación? {#what-is-the-definition-of-success-in-the-engagement-tab}

El éxito es una medida de la interacción significativa en Marketing. El propósito de un programa es crear una interacción significativa con la persona o el cliente potencial. El éxito se marca cuando una persona alcanza la condición que lo permite. Puede asistir a un seminario web, hacer clic en un vínculo de un correo electrónico o rellenar un formulario web. El éxito varía en función del canal de programa.

>[!NOTE]
>
>**Ejemplo**
>
>En un programa de seminario web, puede haber varios estados, como: Invitado, registrado y asistente. Invitado o Registrado no son interacciones significativas porque la gente no ve realmente el seminario web. En este caso, se considera que la asistencia ha sido un éxito.

## ¿Funcionará MPI con alguna CRM? {#will-mpi-work-with-any-crm}

Sí. Técnicamente, MPI no interactúa directamente con CRM para la sincronización de datos. MPI utiliza datos almacenados en la Data Warehouse de Marketing Analytics. Dado que la sincronización de CRM se produce en la aplicación de gestión de clientes potenciales, cualquier CRM compatible con Marketing integrado con la aplicación de gestión de clientes potenciales mostrará los datos correctamente. Sin embargo, es necesario asignar correctamente los campos de oportunidad de CRM a los campos de oportunidad de Marketing to.

## No tengo ningún otro producto de Marketing Analytics (ARB, RCE, RCA, Análisis de Programa). ¿Funcionará MPI para mí? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI es un complemento independiente de la aplicación de administración de posibles clientes. No requiere el uso de ningún otro producto de análisis.

## RCA también me muestra datos de rendimiento de programa. ¿Existe alguna diferencia entre los datos mostrados en MPI y RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

No. MPI origina datos del mismo almacén de datos que RCA. Por lo tanto, no verá ninguna diferencia de datos entre los dos. RCA le permite crear sus propios informes sobre la marcha. MPI le permite acceder a paneles visuales fáciles de entender.

## No quiero que algunos de mis programas (p. ej. Operativos) aparezcan en MPI. ¿Cómo puedo controlar la visibilidad de programas específicos? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Puede controlar la visibilidad de sus programas estableciendo el comportamiento de Analytics de sus programas en Operativo. Esto hará que el programa se excluya de los cálculos de análisis.

>[!NOTE]
>
>Obtenga más información sobre la configuración del comportamiento de análisis [aquí](https://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings).

## Estoy ejecutando una campaña de varios canales para un nuevo lanzamiento de producto. ¿Cómo puedo vista el rendimiento de esta campaña en todos los canales en un solo lugar? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Recomendamos que, para programas que forman parte de una campaña de este tipo, utilice las etiquetas programa. Las etiquetas de programa se sincronizan automáticamente con MPI y puede filtrarlas en todos los paneles MPI para vista del rendimiento de campaña de varios canales.

## ¿Tendré acceso a la configuración de atribución si no tengo RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Puede acceder a la configuración de atribución si tiene MPI, independientemente de si tiene RCA o no.

## Recibo una alerta en MPI cuando inicio sesión diciéndome que mi configuración de atribución es incorrecta. ¿Qué pasa? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcula si todas las oportunidades se incluyen o no en los análisis. Si no es así, se le pedirá que considere la posibilidad de cambiar la configuración de atribución (Explícita, Implícita, Híbrida) para incluir más oportunidades.

También es posible que falten oportunidades debido a que el costo de Programa no está presente en los programas. Revise el comportamiento de Analytics de sus programas. Pueden ser:

1. Predeterminado: el comportamiento predeterminado es que el programa se incluiría en MPI SOLAMENTE si hay al menos un costo de período, incluso uno con cero dólares asignados.
1. Inclusivo: esta opción garantiza que el programa esté disponible en MPI independientemente de si ha incluido o no un costo de período.
1. [Operativo](https://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms) : esta opción hace que el programa no se muestre en MPI.

>[!NOTE]
>
>El costo del período **tiene** que configurarse para el éxito y el sistema de informes de nuevos nombres en el panel de compromiso. Este panel utiliza los datos de costo de período para los éxitos acumulados y los nuevos nombres. Si el costo de período no está configurado, el panel de participación no informará correctamente independientemente de la configuración de comportamiento de Analytics anterior.

## ¿Por qué estoy perdiendo algunas oportunidades en el MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Dos razones clave por las que podría perder oportunidades en MPI son:

1. La configuración de atribución está establecida en Explícita pero las oportunidades no tienen asignadas funciones de contacto
1. El costo de período no se incluye en los programas

MPI calcula si todas las oportunidades se incluyen o no en los análisis. Si no es así, se le pedirá que considere la posibilidad de cambiar la configuración de atribución (Explícita, Implícita, Híbrida) para incluir más oportunidades.

También es posible que falten oportunidades debido a que el costo de Programa no está presente en los programas. La alerta aparecerá pero no indica a qué programas le faltan costes. Revise la configuración del programa para incluir costes y asegurarse de que todos los programas y oportunidades se incluyen en MPI.

## ¿Por qué no veo los campos personalizados, el tipo de oportunidad y los filtros ABM en el panel de compromiso? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Los campos personalizados, el tipo de oportunidad y los Filtros ABM son atributos relacionados con una oportunidad. El panel de participación le permite medir su participación y la adquisición de posibles clientes, estén o no asociados con una oportunidad. Dado que el panel de compromiso no tiene en cuenta la oportunidad, los campos personalizados, el tipo de oportunidad y los Filtros ABM no se aplican.

## Deseo utilizar un campo de oportunidad de Salesforce personalizado para el sistema de informes de ingresos en lugar del campo de cantidad de oportunidad de Salesforce estándar. ¿El MPI me permitirá hacer eso? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sí. [La ](https://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) asistencia técnica de marketing puede reasignar el campo Importe de oportunidad de marketing a un campo de oportunidad de Salesforce personalizado, siempre que el tipo de campo sea moneda. Dado que MPI apunta al campo de cantidad Oportunidad de marketing, MPI puede utilizar los datos del campo de Salesforce personalizado reasignado.

>[!NOTE]
>
>Después de la reasignación, MPI mostrará los datos a partir de ahora. El importe histórico no cambiará.

## Si no uso oportunidades, ¿puedo seguir usando MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI está diseñado para permitirle medir el rendimiento del programa desde la parte superior del canal hasta el impacto en los ingresos. Si no utiliza las oportunidades, podrá:

* Rendimiento de vista de sus programas de alimentación para la participación en la audiencia.
* Rendimiento de vista de los programas de adquisición de posibles clientes.
* Rendimiento de vista de campañas de varios canales mediante etiquetas de programa.
* Consulte las tendencias de compromiso de audiencia de los últimos 12 meses.
* Guarde y exporte datos de rendimiento en PowerPoint.

## ¿Puedo medir el éxito de las estrategias basadas en cuentas en MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sí. MPI se integra con [ABM de marketing](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) para extraer listas de cuentas ABM en MPI sin problemas. Puede utilizar el filtro de Lista de cuenta ABM para elegir la lista ABM deseada para filtrar los datos.

## ¿La atribución está disponible al instante cuando compro MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Las capacidades de atribución de marketing están disponibles para nuestros clientes cuando compran MPI. Sin embargo, se requiere [configuración adecuada](https://docs.marketo.com/x/mRPG) para garantizar que las oportunidades y los datos de programa fluyan correctamente en MPI.

## ¿Qué tengo que hacer para configurar la atribución? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuración de oportunidad

   1. Asegurarse de que las oportunidades se sincronizan con su CRM
   1. Si la configuración de atribución está establecida en Explícita, asegúrese de que las funciones de contacto en las oportunidades se rellenen
   1. Se recomienda cambiar la configuración de atribución a híbrido
   1. Configuración de programa

      1. Incluir el costo de programa en los programas
      1. Revise el comportamiento de los análisis para indicar si se debe incluir un programa en los análisis
      1. Establezca los criterios de éxito para cada canal que tenga
      1. Vincular persona a Programas

         1. Asegúrese de que el Programa de adquisición y la fecha de adquisición se han establecido para cada persona de la base de datos para que funcione la atribución de primer toque.
         1. Asegúrese de que los programas estén configurando estados de éxito para las personas de la base de datos

>[!TIP]
>
>Todos los pasos de configuración necesarios se detallan en [este artículo](https://docs.marketo.com/x/mRPG).

## ¿Cuál es la diferencia entre MPI y el analizador de Programas? {#whats-the-difference-between-mpi-and-the-program-analyzer}

El Analizador de Programas permite comparar los programas en hasta cuatro medidas. MPI le permite analizar la contribución de canales y programas hacia una métrica seleccionada, como Éxito, Nuevas oportunidades creadas, etc. También le permite realizar vistas de la tendencia de canales de 12 meses en función de una métrica específica que haya elegido.

## ¿Cuál es la diferencia entre MPI y el Report Builder avanzado? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

El Report Builder avanzado (a veces denominado RCE), está diseñado para el sistema de informes de autoservicio (o ad hoc), normalmente realizado por Operaciones de mercadotecnia. MPI está diseñado para proporcionar a los líderes de marketing y a los especialistas en marketing acceso de un solo clic a la análisis de rendimiento. Se requiere una configuración mínima.

## ¿Qué ha pasado con la opción &quot;Año anterior&quot; del filtro de fecha de contribución? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Se ha eliminado temporalmente la selección &quot;Año anterior&quot;. Todavía tiene la opción de ver los datos de rendimiento de todo el año mediante la selección Intervalo de fechas personalizado.
