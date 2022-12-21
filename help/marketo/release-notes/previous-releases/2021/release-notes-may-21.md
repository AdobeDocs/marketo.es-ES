---
description: 'Notas de la versión, mayo de 2021: Documentación del producto de Marketo'
title: Notas de la versión, mayo de 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
source-git-commit: 115b6e97978778a1d1e13478adf6fee625aa5257
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# Notas de la versión: Mayo de 2021 {#release-notes-may-21}

Las siguientes funciones se incluyen en la versión del 21 de mayo. Compruebe la disponibilidad de las funciones en su edición de Marketo.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones se lanzarán en **7 de mayo de 2021**.

## Experiencias basadas en cuentas {#Account-based-eaperiences}

* **Listas inteligentes de cuentas (disponibilidad general)** ![](assets/yellow-star.png): Identifique y califique dinámicamente cuentas con atributos de cuenta y persona deseados para dirigirse a campañas de marketing multicanal y envíe alertas oportunas a Ventas para cerrar ofertas más rápido. Esta nueva capacidad permite una automatización sólida de las estrategias de marketing basadas en cuentas. Las listas inteligentes de cuentas están disponibles para los clientes con administración de cuentas de Target que estén en la experiencia de usuario de próxima generación.

## Experiencia del usuario de próxima generación {#next-generation-user-experience}

Con la vista previa de la búsqueda global, los especialistas en marketing pueden ver rápidamente dónde existe un recurso compartido en su instancia. Las fichas del explorador muestran la ubicación para mejorar la navegación en las actividades de marketing o en Design Studio. Los filtros de búsqueda globales y de árbol adicionales le ayudan a refinar sus criterios de búsqueda. La funcionalidad de arrastrar y soltar dentro del árbol se ha restablecido, lo que le permite mover carpetas y recursos de forma rápida y eficaz dentro de las áreas de la aplicación principal. Los iconos recién actualizados (que cumplen los estándares de accesibilidad de Adobe) y los distintivos de estado permiten a los especialistas en marketing distinguir entre carpetas y recursos de forma rápida y sencilla en el árbol e identificar el estado de los programas y recursos.

## Automatización de la experiencia {#experience-automation}

* **Ejecución de pasos de flujo de campaña**: Optimice los flujos de trabajo de creación de campañas y mejore el rendimiento de las campañas con un nuevo paso de flujo para campañas inteligentes. Cree y guarde campañas de plantilla centralizadas para tareas repetitivas en su espacio de trabajo, como la normalización del código de país, a las que se llamará y se ejecutará desde cualquier campaña inteligente a través del nuevo paso de flujo &quot;Ejecutar campaña&quot;. Las campañas vinculadas se ejecutarán en el orden designado y se asegurarán de que la tarea finalice antes de pasar al siguiente paso de flujo. Edite rápidamente el flujo en una sola campaña centralizada para actualizar todas las campañas inteligentes que lo utilicen con el fin de optimizar la gestión de datos, la puntuación de posibles clientes y los flujos de trabajo de enrutamiento.

## Organización en canales múltiples {#cross-channel-orchestration}

* **Campos de datos confidenciales en Forms**: La información de identificación personal (PII) del cliente de Protect no se muestra en los formularios de Adobe Marketo Engage definiendo los campos de datos como confidenciales y restringiendo el rellenado previo de dichos campos. Cada vez que un visitante vea un formulario en la página de aterrizaje, los campos definidos como confidenciales no mostrarán ningún dato previamente rellenado.

* **Bloquear envíos de formularios de correo no deseado**: Protect la base de datos de Adobe Marketo Engage a partir de datos no deseados que pueden provocar alertas no válidas para ventas, déclencheur de los registros de campañas y crear actividades no deseadas. El nuevo mecanismo de validación rechaza los envíos de formularios no válidos y detiene los ataques de bots. Los datos están más limpios y las campañas de marketing se ejecutan según lo previsto, lo que minimiza el riesgo de enviar posibles clientes no calificados a las ventas.

* **Advertencia de aprobación de programa de correo electrónico**: Impida enviar correos electrónicos erróneos cuando las nuevas ediciones se hayan realizado en un programa aprobado anteriormente.  La advertencia actúa como protección cuando un especialista en marketing aplica cambios a un correo electrónico que ya ha sido aprobado, pero luego olvida aprobar los cambios más recientes y envía el correo electrónico a una audiencia grande sin contenido, contenido incorrecto o contenido antiguo.

* **Filtrar la actividad de bots de correo electrónico**: Impida las alertas de ventas no deseadas y los informes de correo electrónico inexactos a través de la nueva capacidad de filtrado de actividades de bots de correo electrónico. Identifique y filtre las aperturas y los clics que se pueden asociar a bots de correo electrónico que inspeccionan los vínculos que conducen a falsos déclencheur y alertas de ventas, o a informes incorrectos.

## Mejoras de API {#api-enhancements}

Varias actualizaciones críticas de las API de posibles clientes y de lotes, incluida la capacidad de exportar datos de objetos personalizados de forma masiva, asociar empresas con posibles clientes de forma masiva, la capacidad de filtrar extracciones de actividades masivas en función de un atributo principal y la capacidad de crear y actualizar la pertenencia al programa.

* **Anidar programas de eventos**: En Adobe Marketo Engage puede crear, clonar o mover programas de eventos en otros tipos de programas. Esta funcionalidad ahora está permitida en la API de recursos.

* **API de programa de eliminación mejorada**: Permite que las aplicaciones integradas eliminen programas que contengan tipos de recursos adicionales, sin que sea necesario que los usuarios lo hagan manualmente desde Adobe Marketo Engage.

* **Pertenencia al programa**: Los especialistas en marketing pueden consultar todos los registros de miembros del programa para un programa seleccionado con criterios diferentes, como el estado de miembro del programa. Comparta esta información con una aplicación externa, una herramienta de inteligencia empresarial o Adobe Experience Cloud para mejorar la segmentación y crear una participación más dirigida.

* **Extracción de objetos personalizados en lotes**: La exportación masiva de datos complementa las funciones de importación que los analistas de datos ya están disfrutando en Adobe Marketo Engage. Ahora pueden extraer de forma masiva datos almacenados en objetos personalizados de Adobe Marketo Engage de primer nivel, cargarlos en otra aplicación, almacén de datos o herramienta BI (Business Intelligence) para obtener mejores perspectivas sobre los datos de la instancia de Adobe Marketo Engage.  El movimiento de datos masivo de objetos personalizados es bidireccional y se puede programar a una hora conveniente.

* **API de metadatos de campos personalizados**: Ahorre tiempo automatizando la creación de campos personalizados al configurar las integraciones de Adobe Marketo Engage con una aplicación de terceros. Esta automatización beneficia especialmente a los clientes con varias instancias de Adobe Marketo Engage que ahora pueden optimizar la creación de campos personalizados que solían requerir trabajo manual en cada instancia. Optimice la creación de campos personalizados y ahorre tiempo en esta actividad que consume recursos.

* **API de extracción de actividad masiva**: Obtenga control sobre la cantidad y el tipo de datos al realizar extracciones masivas. Filtre los puntos de datos innecesarios y controle el número de llamadas de API necesarias para extraer de forma masiva datos de actividad.  Por ejemplo, seleccione abrir correos electrónicos, visite una página web o cambie la puntuación de posibles clientes y deje otros cambios en el valor que no desea analizar. Optimice el proceso para reducir el número de llamadas a la API y la limpieza de datos.

* **API de posible cliente**: Identifique posibles clientes en Adobe Marketo Engage que tengan un ECID de Adobe (ID de Experience Cloud) asociado a ellos.  Los clientes de Adobe Marketo Engage pueden crear una lista de posibles clientes a partir de una determinada campaña y utilizar los ECID (ID de Experience Cloud) para crear informes en Adobe Analytics para esa lista específica. La integración entre Adobe Marketo Engage y Adobe Experience Cloud abre oportunidades ilimitadas de segmentación, establecimiento de objetivos y creación de informes.

* **API de importación masiva de posibles clientes**: Controle la importación masiva de posibles clientes y los recursos que necesita. Esta mejora crea una asociación entre el cliente potencial y la empresa durante el proceso de importación de posibles clientes en masa. Aumente la eficacia y el uso de los datos y disminuya el uso si se realizan llamadas de API.

* **Integración basada en API web para clientes de Microsoft Dynamics Online**: La API web de MS Dynamics se introdujo con el protocolo REST versión 8.0 e implementa OData (Open Data Protocol) v4. OData es un estándar de OASIS (Organización para el Desarrollo de Estándares de Información Estructurada) para crear y consumir servicios RESTful sobre datos enriquecidos. Los clientes de Adobe Marketo Engage que requieren integración con Microsoft Dynamics mediante este método se están migrando actualmente a una conexión basada en API web desde SOAP (Protocolo simple de acceso a objetos).

## Entorno de datos de marketing {#marketing-data-environment}

* **Exportación XLSX**: Hemos actualizado las capacidades de exportación en todo el producto para admitir XLSX en lugar de XLS. Esto significa que en cualquier lugar del producto en el que se admita actualmente la exportación XLS, esta opción se reemplazará por una opción para exportar a XLSX en su lugar. Este cambio afectará a los nombres de archivo de todas las exportaciones de Excel de informes y otros datos de Adobe Marketo Engage.

* **Búsqueda por ID de posible cliente**: Acceda rápidamente a la búsqueda de registros de posibles clientes mediante el ID de posible cliente de Adobe Marketo Engage en la base de datos de posibles clientes o en la lista estática. En la ventana Búsqueda rápida, simplemente escriba `[id]` con el número correspondiente, se muestra la información del posible cliente. Los usuarios pueden revisar rápidamente los detalles del posible cliente, la empresa o la oportunidad.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integración con LinkedIn Lead Gen Forms (Beta)**: Obtenga una gran visibilidad de su inversión en el canal de LinkedIn y del ROI con la solución de atribución de Bizible Premium. Con la integración más reciente con la Generación de posibles clientes de LinkedIn Forms, Bizible obtiene información sobre los formularios que se han enviado en la plataforma LinkedIn. Estos rellenos de formulario se comparan con posibles clientes de su instancia de CRM (Administración de la relación con los clientes) o Adobe Marketo Engage para que puedan atribuirse y se puedan rastrear en relación con sus otras participaciones de marketing.

## Anuncios {#announcements}

* **Plataformas de cambio de documentos de producto de Marketo**: Nos complace anunciar que Marketo Product Docs se unió a Adobe Experience League el viernes 7 de mayo. Aún podrá usar la URL: docs.marketo.com, y si ya tiene cualquier artículo marcado, se le redirigirá. Todos los documentos de producto están disponibles en la nueva plataforma, con mejoras planificadas para finales de este año.

* **Administración de usuarios optimizada e inicio de sesión único con tecnología del sistema de identidad de Adobe**: A partir de julio de 2021, los nuevos clientes de Adobe Marketo Engage se incorporarán mediante las credenciales de usuario de Adobe. La migración de los clientes actuales al sistema de identidad integrado no se producirá hasta mediados de 2022 y no se requiere ninguna acción por parte del cliente hasta nuevo aviso. El inicio de sesión único permite a los administradores de TI/seguridad administrar varias instancias de producto de Adobe Marketo Engage junto con otras soluciones de Experience Cloud, así como configurar SSO (Shared Services Organization) a través de una consola común. Los administradores pueden administrar fácilmente los grupos de usuarios y las autorizaciones de los usuarios a través de un Admin Console común.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión para Marketo Engage de mayo de 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
