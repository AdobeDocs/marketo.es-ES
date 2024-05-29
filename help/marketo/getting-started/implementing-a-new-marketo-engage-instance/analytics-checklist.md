---
description: Configure la sección Analytics para la nueva instancia de Marketo Engage.
title: 'Nuevas prácticas recomendadas para instancias: lista de comprobación de Analytics'
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 00656b2167435d51da55537d251d84910002e46d
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 1%

---

# Nuevas prácticas recomendadas para instancias: lista de comprobación de Analytics {#new-instance-best-practices-analytics-checklist}

La sección Analytics ofrece informes globales que analizan el rendimiento de sus esfuerzos de marketing. Obtenga información acerca de los pasos necesarios para navegarlos.

Recuerde lo siguiente [descargar las listas de comprobación](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) y realice un seguimiento de su progreso.

## Árbol {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organización: asignación de nombres, carpetas y archivado</td>
    <td><li>Utilice una convención de nombres de informes para diferenciar los informes de la pestaña Informes globales.
    <ul><li>Un ejemplo de práctica recomendada de convención de nombres es [Tipo de informe] [Etiqueta global frente a específica de la unidad de negocio] [Descripción del informe] como [Rendimiento de correo electrónico]-[Global]-[Participación de correo electrónico de 180 días].</li></ul><br>
    <li>Identifique los informes que deben compartirse con distintos grupos de usuarios de su organización (por ejemplo, equipo de ventas o liderazgo de marketing) y organice los informes por carpeta dentro de la carpeta Informes de grupo en Analytics para informes globales.</li> 
    <li>El archivado debe limitarse a la carpeta Informes globales, ya que se trata de informes siempre activos.   <ul><li>Limite el archivado a los cambios organizativos, como la reducción o adición de unidades de negocio relevantes, si realiza informes basados en una estructura de unidades de negocio.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Espacios de trabajo (si corresponde)</td>
    <td><li>Repita los informes globales y la estructura de carpetas en los espacios de trabajo para mantener la coherencia en la creación de informes para sus equipos. Estos informes se encuentran en la carpeta Informes de grupo.</li></td>
  </tr>
  <tr>
    <td>Mis informes</td>
    <td><li>Identificar y crear los informes necesarios para su uso en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Mis informes</a> sección. Utilice esta sección de informe privado como zona protegida para informes globales. Solo están disponibles para el usuario que crea el informe.</li>
    <li>Utilice la convención de nombres de su organización para identificar el informe y el uso, de modo que pueda conciliar los informes de Mis informes con los informes de Grupos.</li></td>
  </tr>
  <tr>
    <td>Informes de grupo</td>
    <td><li>Los informes de grupo son los informes globales de su organización y deben informar sobre la actividad general de su organización.</li>
    <li>Considere la posibilidad de crear <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">informes principales clonables</a> espera que cada unidad comercial utilice con mayor frecuencia para reducir el tiempo necesario para extraer el informe y garantizar la corrección de los datos. Consulte los detalles en la <a href="#global-reports">Tabla Informes globales a continuación</a>.
    <ul><li>Informe de rendimiento de personas (todo el tiempo y basado en el tiempo) por origen y mes</li>
    <li>Informe de rendimiento del programa (por mes de coste y basado en el tiempo)</li>
    <li>Informe de rendimiento del correo electrónico (basado en el tiempo)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Activar "Informes globales"</a> en la pestaña Configuración del informe para incluir los datos de todos los espacios de trabajo en los informes Rendimiento de correo electrónico y Rendimiento de los vínculos de correo electrónico. Si tiene más de un espacio de trabajo, solo necesita habilitarlo en el espacio de trabajo predeterminado.</li>
    <p><img src="assets/tip-icon.png" alt="icono de nota"> SUGERENCIA: Cree el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Lista inteligente</a> con los filtros que desee incluir en la mayoría de los informes de la sección Base de datos. Cuando necesite actualizar los criterios de la lista inteligente, puede actualizarlos en un solo lugar en lugar de hacerlo en todos los informes globales.</td>
  </tr>
</tbody>
</table>

## Suscripciones {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Suscripciones</td>
    <td><li>Alinee con su líder de marketing en cuanto a las personas que deben revisar los resultados de los informes y su cadencia durante la implementación.</li> <li>Utilice suscripciones para distribuir datos a personas de su organización que necesitan conocer sin agotar una licencia de usuario designada.</li>
    <p><img src="assets/tip-icon.png" alt="icono de nota"> SUGERENCIA: Si desea que las personas accedan a los datos de los informes en tiempo real, debe añadirlos como usuarios para que puedan ver el informe.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Configuración de suscripciones</a> en la cadencia deseada (diaria/semanal/mensual) para la monitorización continua de cada equipo. También puede <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">ver todas las suscripciones</a> en un lugar de la pestaña Suscripciones de Analytics.</li></td>
  </tr>
</tbody>
</table>

## Informes globales {#global-reports}

Identifique los informes que deben compartirse con distintos grupos de usuarios de su organización (por ejemplo, equipo de ventas o liderazgo de marketing). Cree la estructura de carpetas adecuada para cada equipo, grupo de usuarios o unidad de negocio a fin de organizar los informes clonados dentro de los informes de grupo. Considere la posibilidad de configurar informes globales como:

<table>
<thead>
  <tr>
    <th style="width:20%">Tipo de informe</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Informe de rendimiento de correo electrónico</td>
    <td><li>Cree informes globales, de espacio de trabajo/de toda la unidad de negocio con los correos electrónicos correctos seleccionados.</li>
    <li>Cree un informe de rendimiento de correo electrónico local en todas las plantillas de programa que se pueden clonar.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Utilizar un periodo de tiempo relevante</a> (por ejemplo, hasta la fecha, últimos 90 días, etc.) para que el informe proporcione una vista precisa de la participación de correo electrónico estándar y las métricas de envío.</li>
    <p><img src="assets/tip-icon.png" alt="icono de nota"> SUGERENCIA: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Activar el filtrado "Actividad de bots" en <strong>Administración &gt; Correo electrónico</strong></a> para evitar el registro o identificar si el registro está habilitado para las actividades de bots. Incluir el filtro para permitir solo <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Actividades abiertas o en las que se hizo clic con la restricción "Es actividad de bots" establecida en "Falso"</a> en la lista inteligente de los informes globales que se pueden clonar.</td>
  </tr>
  <tr>
    <td>Informe de rendimiento de personas</td>
    <td><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Se recomienda tener un adecuado <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">estrategia de canal y etiqueta</a> para cada implementación de Marketo Engage antes de poder rastrear a las personas adquiridas y el ROI de sus inversiones de marketing por canal.
    <p>
    <li>Determine los criterios que utilizará para medir el rendimiento de los programas de adquisición de posibles clientes y crear los informes estándar basados en el tiempo (año actual, última vista móvil de 12 meses o 180 días) basados en las siguientes métricas: <ul><li>Programa de Adquisición: Programa de Marketo Engage que recibe el crédito por adquirir a la persona.</li>
    <li>Origen de Persona: Categoría de origen para cómo se llegó a conocer el registro en la base de datos (según la lista de origen de los valores de CRM)
    </li></ul>
    <li>Mida las personas creadas por semana o mes. Este informe proporciona una medida de la tasa de crecimiento de la base de datos y si se está acercando al límite de tamaño de la base de datos.</li>
    <li>Filtrar las métricas de los informes de rendimiento de personas por <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">usar las listas inteligentes como columnas personalizadas.</a></li>
    <p><img src="assets/tip-icon.png" alt="icono de nota"> SUGERENCIA: Cree listas inteligentes para las columnas personalizadas que desee agregar al informe Rendimiento de personas en la base de datos en lugar de en las actividades de marketing, de modo que pueda ver el nombre de la lista inteligente de forma correcta y clara cuando esté seleccionada en el informe.</td>
  </tr>
  <tr>
    <td>Informe de rendimiento del programa</td>
    <td><p><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Este informe requiere que los canales, los estados de progresión y los pasos de éxito estén definidos en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Administrador</strong> &gt; <strong>Etiquetas</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Mida la eficacia de sus tácticas de marketing</a> dentro de programas selectivos.</li>
    <li>Administre la pertenencia al programa (mediante campañas inteligentes para actualizar el programa de adquisición, el estado y los estados de éxito) según las prácticas recomendadas dentro de las actividades de marketing.</li>
    <li>Medición basada en los costes del año en curso y móvil 12 meses.
    <ul><li>Recuerde que mantener <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Costos de período</a> es fundamental para aprovechar el informe de rendimiento del programa.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="icono de nota"> SUGERENCIA: Para agregar y ver cualquiera <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">listas importadas</a> en los Informes de rendimiento del programa, asegúrese de que sus equipos seleccionan el programa de adquisición adecuado para el etiquetado. Considerar <a href="https://experienceleague.adobe.com/es/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">creación de un programa predeterminado</a> que se va a seleccionar como programa de adquisición cuando las listas importadas no se aplican a ningún canal. Esto garantiza que cualquier persona importada tenga un programa de adquisición válido relacionado con el origen, la unidad de negocio, el canal, etc., en lugar de un valor en blanco.</td>
  </tr>
  <tr>
    <td>Informe Rendimiento de página de aterrizaje</td>
    <td><li>Cree el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Informe Rendimiento de página de aterrizaje</a> como un informe global para que pueda <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrar y revisar los números</a> de todas las páginas de aterrizaje de Design Studio/Marketing Activities en un solo lugar.</li>
    <li>Para programas con páginas de aterrizaje, tenga en cuenta lo siguiente <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">creación de un informe local dedicado dentro de la plantilla del programa</a> para que pueda revisar el rendimiento a nivel de programa.</li></td>
  </tr>
  <tr>
    <td>Informe de actividad de página web</td>
    <td><img src="assets/note-icon.png" alt="icono de nota"> NOTA: Solo las páginas web (páginas de aterrizaje externas y de Marketo) que tienen <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">el JavaScript de Munchkin</a> enabled será objeto de seguimiento en este informe. Considere la posibilidad de colocar el código JavaScript en la plataforma Tag Management, como <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, para evitar codificar el código en todas las páginas web.
    <p>
    <li>Cree el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Informe de actividad de página web</a> como un informe global para que pueda revisar los números de todas las páginas web en un solo lugar. Tenga en cuenta que las actividades de páginas web externas solo se reflejan en los informes Actividad de la página web.</li></td>
  </tr>
</tbody>
</table>

## Informes locales {#local-reports}

Algunos informes de Marketo Engage se implementan mejor como recursos locales dentro de programas específicos en Actividades de marketing, ya que su uso habitual es en un conjunto más limitado de programas y recursos. Considere la posibilidad de configurar informes básicos como:

<table>
<thead>
  <tr>
    <th style="width:20%">Tipo de informe</th>
    <th style="width:80%">Elementos de acción</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Informe de rendimiento del vínculo de correo electrónico</td>
    <td><li>Crear un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Informe de rendimiento del vínculo de correo electrónico</a> en programas que envían correos electrónicos y sus campañas de goteo para proporcionarle información sobre los vínculos que las personas hacen clic en en sus envíos de correo electrónico.</li></td>
  </tr>
  <tr>
    <td>Informe Actividad de la campaña</td>
    <td><li>Cree el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Informe Actividad de la campaña</a> y elija un periodo dentro de la carpeta operativa en Actividades de marketing.</li>
    <li>Configurar informes para monitorizar los déclencheur de cada caso de uso y <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">aplicar filtros de campaña</a> (por ejemplo, déclencheur de puntuación de comportamiento, déclencheur de calificación del ciclo vital, déclencheur de momentos interesantes).</li></td>
  </tr>
  <tr>
    <td>Informe Rendimiento del flujo de participación (si corresponde)</td>
    <td><li>Crear un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Informe Rendimiento del flujo de participación</a> para medir la eficacia del contenido y del flujo implementado dentro del programa de participación.</li>
    <li>Considere utilizar el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">Filtro "Segmentación" en la pestaña Configuración del informe</a> y agrupando los datos de informes por el <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segmento</a> (por ejemplo, origen de la persona, sector) utilizado en su programa de participación. Esto le ayudará a obtener información más detallada sobre los patrones de participación de cada segmento, lo que le guiará a realizar cambios estratégicos para mejorar su programa de participación (contenido, flujo, cadencia de flujo, etc.).</li></td>
  </tr>
</tbody>
</table>
