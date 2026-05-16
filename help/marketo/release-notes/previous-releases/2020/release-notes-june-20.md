---
unique-page-id: 37357276
description: 'Notas de la versión, junio de 2020: Documentos de Marketo: documentación del producto'
title: Notas de la versión, junio de 2020
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
TQID: https://experienceleague.adobe.com/HqmRqpmJ9HipbkC2SWTM7RaxYgp04IAbz9cOiDsuGiY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a8c137b3-8aa5-433e-bdc9-0a216c2a11c1
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 1099
ht-degree: 1%

---

# Notas de la versión: junio de 2020 {#release-notes-june}

Las siguientes funciones se incluyen en la versión de junio de 2020. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_** Las siguientes características se lanzarán el **5 de junio de 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **[Audiencias predictivas](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=es#predictive-audiences)** ![(estrella)](assets/yellow-star.png): los nuevos filtros de listas inteligentes y campañas inteligentes con tecnología Adobe AI le permiten crear segmentos de audiencia con tecnología de IA para programas de marketing por correo electrónico, eventos y seminarios web. Utilice la IA para segmentar audiencias en función de la probabilidad de que el posible cliente se registre en un evento, asista a un evento o cancele la suscripción. Cree audiencias similares basadas en programas anteriores para replicar de forma eficaz el éxito anterior. Alcance los objetivos de conversión con el seguimiento predictivo de objetivos y obtenga recomendaciones sobre cómo refinar los segmentos de audiencia para programas de eventos.
* **Aumento del correo electrónico por lotes** ![(estrella)](assets/yellow-star.png): Mejora de nuestra capacidad de marketing por correo electrónico que le permite enviar hasta 3 millones de correos electrónicos por lotes por hora. Hemos rediseñado nuestra campaña por lotes y el procesamiento de informes por correo electrónico para mejorar el rendimiento de los programas de correo electrónico y las campañas por lotes. Esto reduce el tiempo de espera para el envío y mejora el tiempo de finalización. Configure los envíos de correo electrónico como lo haría normalmente, no hay complejidad añadida. Esta mejora está disponible como complemento del producto que también incluye un paquete de inicio de servicios de envío, herramientas de envío de correo electrónico y varias direcciones IP dedicadas.
* **[Integración de audiencias con Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: nueva integración de Adobe Experience Cloud (AEC) que le permite sincronizar listas estáticas de posibles clientes conocidos de Marketo Engage con varias aplicaciones de AEC para mejorar los programas existentes, desbloquear nuevos casos de uso y organizar campañas multicanal. Esta integración incluye Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager y Adobe Advertising Cloud.
* **[Campos personalizados de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: Capture y utilice campos personalizados sobre un miembro del programa. Utilice estos nuevos campos en los formularios de Marketo Engage, visualícelos en la lista de miembros de un programa, aproveche estos campos en los déclencheur y filtros de las listas inteligentes e inclúyalos en una nueva acción de flujo de la campaña inteligente para mejorar la automatización y una personalización más granular. También se pueden importar y exportar mediante la interfaz de usuario y las API de. Mejora de la capacidad de campos y objetos de datos personalizados.
* **Describir el miembro del programa**: recupere los metadatos del miembro del programa, lo que le permitirá importar y exportar los datos del campo personalizado del miembro del programa mediante la API de REST. Mejora de nuestra API.
* **[Crear tarea en [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: cree tareas para las ventas dentro de [!DNL Microsoft Dynamics] con una nueva acción de flujo basada en el comportamiento del cliente capturado en Marketo Engage. Mejora de nuestra integración nativa de [!DNL Microsoft Dynamics] CRM.
* **Obtener formulario utilizado por el extremo de API de recursos de lista**: recupere una lista de recursos que dependen de un formulario. Mejora de nuestra API.
* **Establecer encabezado previo de correo electrónico mediante API**: habilita la traducción y localización automáticas de los campos de encabezado previo de correo electrónico. Mejora de nuestra API.
* **Almacenamiento en caché de imágenes y archivos**: estamos mejorando la estabilidad del servidor de Marketo Engage al ofrecer recursos de imagen y archivo desde una caché de 60 segundos.

## Account-Based Marketing {#account-based-marketing}

![(estrella)](assets/yellow-star.png)

* **Nueva detección de cuentas disponible en general**

   * La detección de nuevas cuentas es una mejora de nuestra capacidad de generación de perfiles de cuenta que le permite descubrir nuevas cuentas de destino netas para su estrategia ABM en función de su modelo de perfil de cliente ideal con tecnología de IA. Ver, seleccionar e importar nuevas cuentas recomendadas, junto con sus indicadores de datos de ajuste e intención basados en IA.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## [!DNL Bizible] {#bizible}

![(estrella)](assets/yellow-star.png)

* **Integración de programas de Marketo Engage**: extraiga datos de programas directamente de Marketo Engage para crear puntos de contacto a lo largo del recorrido de atribución en [!DNL Bizible] y así acreditar correctamente los programas de correo electrónico y participación. Mejora de nuestra integración con Marketo Engage.
* **Integración de actividades de Marketo Engage (BETA)**: lleve los datos de la actividad de Marketo Engage directamente a [!DNL Bizible] para crear puntos de contacto en el recorrido del cliente y en todos los modelos de atribución. Algunos ejemplos son cambios en la puntuación de posibles clientes, momentos interesantes, clics en correos electrónicos o cualquier actividad personalizada. Mejora de nuestra integración con Marketo Engage.
* **[!DNL Bizible]Integración de atributos del cliente B2B (BETA)**: Se trata de una integración de Adobe Experience Cloud con Adobe Analytics que le permite llevar datos de Bizible seleccionados directamente a Adobe Analytics para un análisis más detallado. Algunos ejemplos son el tráfico del sitio basado en cuentas y el análisis de contenido por nombre de compañía, atributos de cuenta, oportunidades de CRM e individuos de alto valor según se definen en los ingresos atribuidos de [!DNL Bizible] y la fase de funnel.
* **[!DNL Bizible]descubrir filtros y mejoras**: Analice los datos con filtros de canal, subcanal, campaña y segmento en los paneles. Refuerce la visibilidad de los datos con más atributos de desglose. Esto supone una mejora para nuestros paneles de Discover.
* **Sincronización de actividades para[!DNL Microsoft Dynamics]**: atribuye las interacciones de ventas al llevar [!DNL Microsoft Dynamics] actividades de CRM al recorrido del punto de contacto y realiza un seguimiento de eventos como llamadas, citas o tareas asociadas con tus posibles clientes o contactos. Mejora de nuestra integración de CRM [!DNL Microsoft Dynamics].

## [!DNL Sales Insight] {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **[Tablero de perspectivas para Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: estamos reinventando nuestra capacidad [!DNL Sales Insight] con nueva visibilidad de próximos eventos de marketing y campañas para ofrecer a los vendedores la capacidad de hacer recomendaciones más relevantes para los clientes y clientes potenciales en función de sus necesidades e intereses. Los vendedores también pueden ver la actividad de la cuenta y el contacto en el cronograma y acceder fácilmente a detalles adicionales sobre la actividad. Encuentre más detalles sobre cómo actualizar su paquete [aquí](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Anuncios {#announcements}

* **Actualización de ITP 2.1+ RTP**: Debido a los cambios en la directiva de cookies de [!DNL Safari], ITP limitará la capacidad de las cookies RTP de rastrear usuarios en varias sesiones del mismo dominio a 1 o 7 días según la versión del explorador que use el visitante. Para tener en cuenta esto, estamos implementando un nuevo servicio web para permitir que las cookies RTP se configuren con un encabezado Set-Cookie a través de una respuesta HTTP. Encontrará más información [aquí](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Cambios en la infraestructura de campañas por lotes**: vamos a actualizar nuestros servicios de campañas por lotes durante el resto del año. Esta será una actualización perfecta que no afectará a ninguna campaña por lotes en curso y no dará como resultado un cambio de comportamiento. No se requiere ninguna acción. Encuentra más detalles en esta [publicación nacional](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## En desuso {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: A partir de la versión 159 de [!DNL Munchkin] JS, se registrará una advertencia de obsolescencia en la consola del explorador cuando se invoque el método Associate Lead, lo que indica que la característica se eliminará en una versión futura. La programación de obsolescencia completa se anunciará más adelante.

**_Seminario web sobre la versión del producto_** [Vea la grabación](https://engage.marketo.com/June-Release-2020-On-Demand.html) de nuestro Seminario web sobre innovaciones en la versión del producto de junio de 2020.
