---
unique-page-id: 37357276
description: 'Notas de la versión, junio de 2020: Documentos de Marketo: documentación del producto'
title: Notas de la versión, junio de 2020
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---

# Notas de la versión: 20 de junio {#release-notes-june}

Las siguientes funciones se incluyen en la versión de junio de 2020. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_** Las siguientes características se lanzarán el **5 de junio de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **[Audiencias predictivas](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=es#predictive-audiences)** ![(estrella)](assets/yellow-star.png): los nuevos filtros de listas inteligentes y campañas inteligentes con tecnología Adobe Sensei le permiten crear segmentos de audiencia con tecnología de IA para programas de marketing por correo electrónico, eventos y seminarios web. Utilice la IA para segmentar audiencias en función de la probabilidad de que el posible cliente se registre en un evento, asista a un evento o cancele la suscripción. Cree audiencias similares basadas en programas anteriores para replicar de forma eficaz el éxito anterior. Alcance los objetivos de conversión con el seguimiento predictivo de objetivos y obtenga recomendaciones sobre cómo refinar los segmentos de audiencia para programas de eventos.
* **Aumento del correo electrónico por lotes** ![(estrella)](assets/yellow-star.png): Mejora de nuestra capacidad de marketing por correo electrónico que le permite enviar hasta 3 millones de correos electrónicos por lotes por hora. Hemos rediseñado nuestra campaña por lotes y el procesamiento de informes por correo electrónico para mejorar el rendimiento de los programas de correo electrónico y las campañas por lotes. Esto reduce el tiempo de espera para el envío y mejora el tiempo de finalización. Configure los envíos de correo electrónico como lo haría normalmente, no hay complejidad añadida. Esta mejora está disponible como complemento del producto que también incluye un paquete de inicio de servicios de envío, herramientas de envío de correo electrónico y varias direcciones IP dedicadas.
* **[Integración de audiencias con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: nueva integración de Adobe Experience Cloud (AEC) que le permite sincronizar listas estáticas de posibles clientes conocidos de Marketo Engage con varias aplicaciones de AEC para mejorar los programas existentes, desbloquear nuevos casos de uso y organizar campañas multicanal. Esta integración incluye Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager y Adobe Advertising Cloud.
* **[Campos personalizados de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: Capture y utilice campos personalizados sobre un miembro del programa. Utilice estos nuevos campos en los formularios de Marketo Engage, visualícelos en la lista de miembros de un programa, aproveche estos campos en los déclencheur y filtros de las listas inteligentes e inclúyalos en una nueva acción de flujo de la campaña inteligente para mejorar la automatización y una personalización más granular. También se pueden importar y exportar mediante la interfaz de usuario y las API de. Mejora de la capacidad de campos y objetos de datos personalizados.
* **Describir el miembro del programa**: recupere los metadatos del miembro del programa, lo que le permitirá importar y exportar los datos del campo personalizado del miembro del programa mediante la API de REST. Mejora de nuestra API.
* **[Crear tarea en Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: cree tareas para ventas dentro de Microsoft Dynamics con una nueva acción de flujo basada en el comportamiento del cliente capturado en Marketo Engage. Mejora de nuestra integración nativa con Microsoft Dynamics CRM.
* **Obtener formulario utilizado por el extremo de API de recursos de lista**: recupere una lista de recursos que dependen de un formulario. Mejora de nuestra API.
* **Establecer encabezado previo de correo electrónico mediante API**: habilita la traducción y localización automáticas de los campos de encabezado previo de correo electrónico. Mejora de nuestra API.
* **Almacenamiento en caché de imágenes y archivos**: estamos mejorando la estabilidad del servidor Marketo Engage al ofrecer recursos de imagen y archivo desde una memoria caché de 60 segundos.

## Account-Based Marketing {#account-based-marketing}

![(estrella)](assets/yellow-star.png)

* **Nueva detección de cuentas disponible en general**

   * La detección de nuevas cuentas es una mejora de nuestra capacidad de generación de perfiles de cuenta que le permite descubrir nuevas cuentas de destino netas para su estrategia ABM en función de su modelo de perfil de cliente ideal con tecnología de IA. Ver, seleccionar e importar nuevas cuentas recomendadas, junto con sus indicadores de datos de ajuste e intención basados en IA.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Bizible {#bizible}

![(estrella)](assets/yellow-star.png)

* **Integración de programas de Marketo Engage**: Extraiga los datos del programa directamente del Marketo Engage para crear puntos de contacto a lo largo del recorrido de atribución en Bizible y así acreditar adecuadamente los programas de correo electrónico y participación. Mejora de la integración de nuestro Marketo Engage.
* **Integración de actividades del Marketo Engage (BETA)**: Incluya datos de actividades del Marketo Engage directamente en Bizible para crear puntos de contacto en el recorrido del cliente y en todos los modelos de atribución. Algunos ejemplos son cambios en la puntuación de posibles clientes, momentos interesantes, clics en correos electrónicos o cualquier actividad personalizada. Mejora de la integración de nuestro Marketo Engage.
* **Integración de atributos del cliente de Bizible B2B (BETA)**: se trata de una integración de Adobe Experience Cloud con Adobe Analytics que le permite incorporar datos de Bizible seleccionados directamente en Adobe Analytics para un análisis más detallado. Algunos ejemplos son el tráfico del sitio basado en cuentas y el análisis de contenido por nombre de compañía, atributos de cuenta, oportunidades de CRM e individuos de alto valor según se definen en la etapa de ingresos y embudo atribuidos a Bizible.
* **Filtros y mejoras de Bizible Discover**: Analice sus datos con filtros de canal, subcanal, campaña y segmento en los paneles. Refuerce la visibilidad de los datos con más atributos de desglose. Esto supone una mejora para nuestros paneles de Discover.
* **Sincronización de actividades para Microsoft Dynamics**: Atribuya las interacciones de ventas al llevar las actividades de Microsoft Dynamics CRM al recorrido de puntos de contacto y realice un seguimiento de eventos como llamadas, citas o tareas asociadas con sus posibles clientes o contactos. Mejora de la integración de Microsoft Dynamics CRM.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **[Tablero de perspectivas para Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: Estamos reinventando nuestra capacidad de perspectiva de ventas con nueva visibilidad de próximos eventos y campañas de marketing para ofrecer a los vendedores la capacidad de hacer recomendaciones más relevantes para los clientes y clientes potenciales en función de sus necesidades e intereses. Los vendedores también pueden ver la actividad de la cuenta y el contacto en el cronograma y acceder fácilmente a detalles adicionales sobre la actividad. Encuentre más detalles sobre cómo actualizar su paquete [aquí](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Anuncios {#announcements}

* **Actualización de ITP 2.1+ RTP**: Debido a los cambios en la directiva de cookies de Safari, ITP limitará la capacidad de las cookies RTP de rastrear a los usuarios en varias sesiones del mismo dominio a 1 o 7 días, según la versión del explorador que utilice el visitante. Para tener en cuenta esto, estamos implementando un nuevo servicio web para permitir que las cookies RTP se configuren con un encabezado Set-Cookie a través de una respuesta HTTP. Encontrará más información [aquí](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Cambios en la infraestructura de campañas por lotes**: vamos a actualizar nuestros servicios de campañas por lotes durante el resto del año. Esta será una actualización perfecta que no afectará a ninguna campaña por lotes en curso y no dará como resultado un cambio de comportamiento. No se requiere ninguna acción. Encuentra más detalles en esta [publicación nacional](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## En desuso {#deprecations}

* **[Posible cliente asociado de Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: a partir de la versión 159 de Munchkin JS, se registrará una advertencia de obsolescencia en la consola del explorador cuando se invoque el método de Posible cliente asociado, lo que indica que la característica se eliminará en una versión futura.  El calendario completo de desaprobación se anunciará más adelante.

**_Seminario web sobre la versión del producto_** [Vea la grabación](https://engage.marketo.com/June-Release-2020-On-Demand.html) de nuestro Seminario web sobre innovaciones en la versión del producto de junio de 2020.
