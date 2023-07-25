---
description: 'Notas de la versión, mayo de 2021: Documentos de Marketo: documentación del producto'
title: Notas de la versión, mayo de 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# Notas de la versión: mayo de 2021 {#release-notes-may-21}

Las siguientes funciones se incluyen en la versión de mayo de 2021 de. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones se lanzarán el **7 de mayo de 2021**.

## Experiencias basadas en cuentas {#Account-based-eaperiences}

* **Listas inteligentes de cuenta (disponibilidad general)** ![](assets/yellow-star.png): identifique y califique de forma dinámica las cuentas con los atributos de cuenta y persona deseados para segmentar campañas de marketing en canales múltiples y enviar alertas oportunas a Ventas para cerrar acuerdos más rápido. Esta nueva capacidad permite una automatización sólida de las estrategias de marketing basadas en cuentas. Las listas inteligentes de cuentas están disponibles para los clientes con Administración de cuentas de Target que están en la experiencia del usuario de próxima generación.

## Experiencia del usuario de próxima generación {#next-generation-user-experience}

Con la vista previa de búsqueda global, los especialistas en marketing pueden ver rápidamente dónde existe un recurso compartido en su instancia. Las pestañas del explorador muestran la ubicación para mejorar la navegación en las actividades de marketing o Design Studio. Los filtros de búsqueda globales y de árbol adicionales ayudan a restringir los criterios de búsqueda. Se ha restablecido la funcionalidad de arrastrar y soltar dentro del árbol, lo que le permite mover carpetas y recursos de forma rápida y eficaz dentro de las áreas principales de la aplicación. Los iconos recién actualizados (que cumplen con los estándares de accesibilidad del Adobe) y los distintivos de estado permiten a los especialistas en marketing distinguir entre carpetas y recursos de forma rápida y sencilla en el árbol e identificar el estado de los programas y recursos.

## Automatización de experiencias {#experience-automation}

* **Pasos para ejecutar el flujo de campaña**: Optimice los flujos de trabajo de creación de campañas y mejore el rendimiento de las campañas con un nuevo paso de flujo para las campañas inteligentes. Cree y guarde campañas de plantilla centralizadas para tareas repetitivas en su espacio de trabajo, como la normalización del código de país, para que se llamen y ejecuten desde cualquier campaña inteligente a través del nuevo paso de flujo &quot;Ejecutar campaña&quot;. Las campañas vinculadas se ejecutarán en el orden designado y garantizarán la finalización de las tareas antes de pasar al siguiente paso del flujo. Edite rápidamente el flujo en una sola campaña centralizada para actualizar todos los flujos de trabajo de campañas inteligentes que lo utilicen para optimizar la administración de datos, la puntuación de posibles clientes y el enrutamiento.

## Orquestación entre canales {#cross-channel-orchestration}

* **Campos de datos confidenciales en Forms**: la información de identificación personal (PII) del cliente de Protect se muestra en los formularios de Adobe Marketo Engage al definir los campos de datos como confidenciales y restringir el relleno previo de formulario para esos campos. Cada vez que un visitante vea un formulario en la página de aterrizaje, los campos definidos como confidenciales no mostrarán datos rellenados previamente.

* **Bloquear envíos de formularios de spam**: Protect su base de datos de Adobe Marketo Engage a partir de datos no deseados que pueden provocar alertas no válidas en las ventas, déclencheur los trabajos pendientes de las campañas y crear actividades no deseadas. El nuevo mecanismo de validación rechaza los envíos de formularios no válidos y detiene los ataques de bots. Sus datos son más limpios y sus campañas de marketing se ejecutan según lo previsto, lo que minimiza el riesgo de enviar posibles clientes no cualificados a las ventas.

* **Advertencia de aprobación del programa de correo electrónico**: Impida el envío de correos electrónicos erróneos cuando se realicen nuevas ediciones en un programa aprobado anteriormente.  La advertencia actúa como barrera cuando un experto en marketing aplica cambios a un correo electrónico que ya está aprobado, pero luego olvida aprobar los cambios más recientes y envía el correo electrónico a una audiencia grande sin contenido, contenido incorrecto o contenido antiguo.

* **Filtrar la actividad de bots de correo electrónico**: Impida las alertas de ventas no deseadas y los informes de correo electrónico inexactos a través de la nueva capacidad de filtrado de actividades de bots de correo electrónico. Identificar y filtrar las aperturas y los clics que pueden asociarse con bots de correo electrónico que inspeccionan vínculos que generan déclencheur falsos y alertas de ventas o informes incorrectos.

## Mejoras de API {#api-enhancements}

Varias actualizaciones críticas de las API de Bulk y Lead, incluida la capacidad de exportar datos de objetos personalizados de forma masiva, asociar la empresa con el posible cliente de forma masiva, la capacidad de filtrar la extracción de actividades de forma masiva en función de un atributo principal y la capacidad de crear y actualizar la pertenencia al programa.

* **Anidar programas de eventos**: en Adobe Marketo Engage puede crear, clonar o mover programas de eventos en otros tipos de programas. Esta funcionalidad ahora se permite en la API de recursos.

* **API de programa de eliminación mejorada**: permite a las aplicaciones integradas eliminar programas que contienen tipos adicionales de recursos, sin que sea necesario que los usuarios lo hagan manualmente desde Adobe Marketo Engage.

* **Suscripción al programa**: los especialistas en marketing pueden consultar todos los registros de miembros de un programa determinado según diferentes criterios, como el estado de miembro del programa. Comparta esta información con una aplicación externa, una herramienta de inteligencia empresarial o Adobe Experience Cloud para mejorar la segmentación y crear una participación más dirigida.

* **Extracción masiva de objetos personalizados**: la exportación de datos en lote complementa las funciones de importación que los analistas de datos ya están disfrutando en Adobe Marketo Engage. Ahora pueden extraer datos almacenados en los objetos personalizados de Adobe Marketo Engage de primer nivel de forma masiva y cargarlos en otra aplicación, almacén de datos o herramienta de BI (Business Intelligence) para obtener una mejor perspectiva de los datos en la instancia de Adobe Marketo Engage.  El movimiento masivo de datos de objetos personalizados es bidireccional y se puede programar en un momento conveniente.

* **API de metadatos de campos personalizados**: Ahorre tiempo automatizando la creación de campos personalizados al configurar las integraciones de Adobe Marketo Engage con una aplicación de terceros. Esta automatización beneficia especialmente a los clientes con varias instancias de Adobe Marketo Engage, que ahora pueden optimizar la creación de campos personalizados que solían requerir trabajo manual en cada instancia. Optimice la creación de campos personalizados y ahorre tiempo en esta actividad que consume recursos.

* **API de extracción masiva de actividades**: Obtenga control sobre la cantidad y el tipo de datos al realizar extracciones masivas. Filtre los puntos de datos innecesarios y controle el número de llamadas de API necesarias para extraer datos de actividad de forma masiva.  Por ejemplo, seleccione correos electrónicos abiertos, visite una página web o cambie la puntuación del posible cliente y deje atrás otros cambios en el valor que no desea analizar. Optimice el proceso para reducir el número de llamadas a la API y la limpieza de datos.

* **API de cliente potencial**: identifique los posibles clientes en Adobe Marketo Engage que tengan un ECID de Adobe (ID de Experience Cloud) asociado a ellos.  Los clientes de Adobe Marketo Engage pueden crear una lista de posibles clientes a partir de una campaña determinada y utilizar los ECID (ID de Experience Cloud) para crear informes en Adobe Analytics para esa lista específica. La integración entre Adobe Marketo Engage y Adobe Experience Cloud ofrece oportunidades ilimitadas de segmentación, direccionamiento y creación de informes.

* **API de importación masiva de posibles clientes**: Controle la importación masiva de posibles clientes y los recursos que necesita. Esta mejora crea una asociación entre el posible cliente y la empresa durante el proceso de importación masiva de posibles clientes. Aumentar la eficacia y la eficacia del trabajo con datos y reducir el uso si la API llama a.

* **Integración basada en API web para los clientes en línea de Microsoft Dynamics**: la API web de MS Dynamics se introdujo con el protocolo REST versión 8.0 e implementa OData (Open Data Protocol) v4. OData es un estándar de OASIS (Organización para el Avance de los Estándares de Información Estructurada) para crear y consumir servicios RESTful sobre datos enriquecidos. Los clientes de Adobe Marketo Engage que necesitan integrarse con Microsoft Dynamics mediante este método se están migrando actualmente a una conexión basada en API web desde SOAP (Protocolo simple de acceso a objetos).

## Entorno de datos de marketing {#marketing-data-environment}

* **Exportación XLSX**: Hemos actualizado las funciones de exportación en todo el producto para que admitan XLSX en lugar de XLS. Esto significa que en cualquier parte del producto donde la exportación XLS sea compatible actualmente, esta opción será reemplazada por una opción para exportar a XLSX. Este cambio afectará a los nombres de archivo de todas las exportaciones de Excel de informes y otros datos de Adobe Marketo Engage.

* **Buscar por ID de posible cliente**: Acceda rápidamente a la búsqueda de registros de posibles clientes por ID de posible cliente de Adobe Marketo Engage en la base de datos de posibles clientes o lista estática. En la ventana Búsqueda rápida, simplemente escriba `[id]` con el número correspondiente, se mostrará la información del posible cliente. Los usuarios pueden revisar rápidamente los detalles del posible cliente, la empresa o la oportunidad.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integración con LinkedIn Lead Gen Forms (Beta)**: Obtenga una visibilidad profunda del gasto y el ROI de su canal de LinkedIn con la solución de atribución premium de Bizible. A través de la última integración con Forms de generación de clientes potenciales de LinkedIn, Bizible obtiene una perspectiva de los formularios que se han enviado dentro de la plataforma LinkedIn. Estos rellenos de formulario se comparan con los posibles clientes de su CRM (administración de la relación con los clientes) o instancia de Adobe Marketo Engage, de modo que son aptos para la atribución y se pueden rastrear en relación con sus otras participaciones de marketing.

## Anuncios {#announcements}

* **Plataformas de conmutación de documentos de producto de Marketo**: Nos complace anunciar que la documentación del producto de Marketo se ha unido a Adobe Experience League el viernes 7 de mayo. Podrá seguir utilizando la URL: docs.marketo.com y, si tiene algún artículo existente marcado, se le redirigirá. Todos los documentos del producto están disponibles en la nueva plataforma y se prevé realizar mejoras más adelante este año.

* **Administración de usuarios optimizada e inicio de sesión único con tecnología de Adobe Identity System**: a partir de julio de 2021, los nuevos clientes de Adobe Marketo Engage se incorporarán con las credenciales de usuario de Adobe. La migración de los clientes actuales al sistema de identidad integrado no se producirá hasta mediados de 2022 y no se requiere ninguna acción por parte del cliente hasta nuevo aviso. El inicio de sesión único permite a los administradores de TI/seguridad administrar varias instancias de producto de Adobe Marketo Engage junto con otras soluciones de Experience Cloud, así como configurar el SSO (organización de servicios compartidos) a través de una consola común. Los administradores pueden administrar de forma práctica los grupos de usuarios y las autorizaciones de usuario a través de un Admin Console común.

**_Seminario web sobre lanzamiento de productos_**

[Seminario web sobre la publicación de Marketo Engage en mayo de 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
