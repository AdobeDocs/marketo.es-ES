---
unique-page-id: 37357276
description: 'Notas de la versión, junio del 2020: Documentos de Marketo: Documentación del producto'
title: Notas de la versión, junio de 2020
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 0%

---

# Notas de la versión: Junio de 20 {#release-notes-june}

Las siguientes funciones se incluyen en la versión del 20 de junio. Compruebe la disponibilidad de las funciones en su edición de Marketo.

>[!AVAILABILITY]
>
>Las funciones identificadas por una estrella ( ![(star)](assets/star-yellow.svg)) pueden ser complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestralesLas siguientes_** funciones se lanzarán el 5 de  **junio de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![ (estrella)](assets/star-yellow.svg): Los nuevos filtros de listas inteligentes y campañas inteligentes con tecnología de Adobe Sensei le permiten crear segmentos de audiencia con tecnología de IA para programas de marketing por correo electrónico, eventos y seminarios web. Utilice AI para segmentar audiencias en función de la probabilidad de posible cliente para registrarse en un evento, asistir a un evento o cancelar la suscripción. Cree audiencias parecidas basadas en programas anteriores para reproducir de forma eficaz los éxitos anteriores. Alcance los objetivos de conversión con seguimiento de objetivos predictivo y obtenga recomendaciones sobre cómo refinar los segmentos de audiencia para los programas de eventos.
* **Aumento del correo electrónico por lotes** ![ (estrella)](assets/star-yellow.svg): Mejora de nuestra capacidad de marketing por correo electrónico que le permite enviar hasta 3 millones de correos electrónicos por lotes por hora. Hemos rediseñado el procesamiento de informes de correo electrónico y campañas por lotes para mejorar el rendimiento de los programas de correo electrónico y las campañas de correo electrónico por lotes. Esto reduce el tiempo de envío y mejora el tiempo de finalización. Configure los envíos de correo electrónico como lo haría normalmente, no hay complejidad añadida. Esta mejora está disponible como complemento de producto que también incluye un paquete de lanzamiento de servicios de envío, herramientas de envío de correo electrónico y varias direcciones IP dedicadas.
* **[Integración de audiencias con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Nueva integración de Adobe Experience Cloud (AEC) que le permite sincronizar listas estáticas de posibles clientes conocidos de Marketo Engage con varias aplicaciones AEC para mejorar los programas existentes, desbloquear nuevos casos de uso y organizar campañas multicanal. Esta integración incluye Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager y Adobe Advertising Cloud.
* **[Campos personalizados de miembro del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: Captura y uso de campos personalizados sobre un miembro del programa. Utilice estos campos nuevos en los formularios de Marketo Engage, véalos en la lista de miembros de un programa, utilícelos en los déclencheur y filtros de listas inteligentes e inclúyalos en una nueva acción de flujo de campaña inteligente para una automatización mejorada y una personalización más granular. También se pueden importar y exportar mediante la interfaz de usuario y las API. Mejora de la capacidad de campos y objetos de datos personalizados.
* **Describir a un miembro** del programa: Recupere los metadatos de miembro del programa, lo que le permite importar y exportar datos de campo personalizado de miembro del programa mediante la API de REST. Mejora de nuestra API.
* **[Crear tarea en Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: Cree tareas para ventas dentro de Microsoft Dynamics mediante una nueva acción de flujo basada en el comportamiento del cliente capturado en el Marketo Engage. Mejora de nuestra integración nativa de Microsoft Dynamics CRM.
* **Obtener formulario utilizado por el extremo** de la API de recursos de lista: Recupere una lista de recursos que dependen de un formulario. Mejora de nuestra API.
* **Configure el encabezado previo del correo electrónico mediante API**: Habilite la traducción automática y la localización de campos de encabezado previo de correo electrónico. Mejora de nuestra API.
* **Almacenamiento en caché de imágenes y archivos**: Mejoramos la estabilidad del servidor Marketo Engage al servir recursos de imagen y archivo desde una caché de 60 segundos.

## Marketing basado en cuentas {#account-based-marketing}

![(estrella)](assets/star-yellow.svg)

* **Descubrimiento de nueva cuenta disponible de forma general**

   * La nueva detección de cuentas es una mejora de nuestra capacidad de creación de perfiles de cuentas que le permite descubrir nuevas cuentas de destino para su estrategia ABM basada en su modelo de perfil de cliente ideal con tecnología de IA. Ver, seleccionar e importar cuentas nuevas recomendadas, junto con los indicadores de datos de ajuste e intención basados en IA.

<br> 

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Bizible {#bizible}

![(estrella)](assets/star-yellow.svg)

* **Integración de programas de Marketo Engage**: Extraiga los datos del programa directamente del Marketo Engage para crear puntos de contacto a lo largo del recorrido de atribución en Bizible y así acreditar adecuadamente los programas de correo electrónico y participación. Mejora de la integración de Marketo Engage.
* **Integración de actividades de Marketo Engage (BETA)**: Incluya los datos de actividad del Marketo Engage directamente en Bizible para crear puntos de contacto en el recorrido del cliente y en todos los modelos de atribución. Algunos ejemplos son cambios en la puntuación de los posibles clientes, momentos interesantes, clics en correos electrónicos o cualquier actividad personalizada. Mejora de la integración de Marketo Engage.
* **Integración de atributos del cliente Bizible B2B (BETA)**: Se trata de una integración de Adobe Experience Cloud con Adobe Analytics que le permite incluir datos seleccionados de Bizible directamente en Adobe Analytics para un análisis más detallado. Algunos ejemplos son el tráfico del sitio basado en cuentas y el análisis de contenido por nombre de empresa, atributos de cuenta, oportunidades de CRM y personas de alto valor, tal como se define en la etapa de ingresos y canal atribuidos a Bizible.
* **Filtros y mejoras** de Discover Bizible: Analice sus datos con filtros de canal, subcanal, campaña y segmento entre tableros. Fortalezca la visibilidad de los datos con más atributos de desglose. Esta es una mejora de nuestros tableros de Discover.
* **Sincronización de actividades para Microsoft Dynamics**: Las interacciones de ventas de atributos al llevar las actividades de Microsoft Dynamics CRM al recorrido de puntos de contacto y rastrear eventos como llamadas, citas o tareas asociadas con sus posibles clientes o contactos. Mejora de nuestra integración con Microsoft Dynamics CRM.

## Perspectiva de ventas {#sales-insight}

![(estrella)](assets/star-yellow.svg)

* **[Panel de perspectivas para Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: Estamos reinventando nuestra capacidad de perspectiva de ventas con una nueva visibilidad de los próximos eventos y campañas de marketing para ofrecer a los vendedores la capacidad de hacer recomendaciones más relevantes para los clientes y clientes potenciales según sus necesidades e intereses. Los vendedores también pueden ver la Actividad de Contacto y Cuenta dentro de la cronología y acceder fácilmente a detalles adicionales de la actividad. Encuentre más detalles sobre cómo actualizar su paquete [aquí](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md).

<br> 

## Anuncios {#announcements}

* **Actualización** de RTP de ITP 2.1+: Debido a los cambios en la política de cookies para Safari, la capacidad de las cookies RTP para rastrear usuarios entre sesiones en el mismo dominio se verá limitada por ITP a 1 o 7 días según el explorador y la versión del explorador que use el visitante. Para tener en cuenta esto, estamos implementando un nuevo servicio web para permitir que las cookies RTP se configuren con un encabezado Set-Cookie a través de una respuesta HTTP. Puede encontrar más información [aquí](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Cambios en la infraestructura de campañas por lotes**: Estamos actualizando nuestros servicios de campañas por lotes durante el resto de este año. Será una actualización perfecta que no afectará a ninguna campaña por lotes en curso y que no provocará un cambio de comportamiento. No se requiere ninguna acción. Encuentre más detalles en este [Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Obsolescencia {#deprecations}

* **[Asociado de Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: A partir de la versión 159 de Munchkin JS, se registrará una advertencia de desaprobación en la consola del explorador cuando se invoque el método Associate Lead , lo que indica que la función se eliminará en una versión futura.  La programación de desaprobación completa se anunciará más adelante.

**_Seminario_** [web sobre versiones de productosVea la ](https://engage.marketo.com/June-Release-2020-On-Demand.html) grabación de nuestro seminario web sobre innovaciones en versiones de productos del 20 de junio.
