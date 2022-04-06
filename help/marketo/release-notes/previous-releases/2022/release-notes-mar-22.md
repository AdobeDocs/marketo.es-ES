---
description: 'Notas de la versión, marzo de 2022: Documentos de Marketo: Documentación del producto'
title: Notas de la versión, marzo de 2022
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# Notas de la versión: Marzo de 2022 {#release-notes-mar-22}

La versión del 22 de marzo incluye las siguientes funciones. Consulte la edición para Marketo Engage de Adobe si hay disponibilidad de funcionalidades.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones empezarán a lanzarse en **11 de marzo de 2022**, con una implementación por fases de cada función en las semanas siguientes (a menos que se especifique lo contrario).

## Organización en canales múltiples {#cross-channel-orchestration}

* **Chat dinámico**: Maximice todas las oportunidades en su sitio web centrándose tanto en posibles clientes como en cuentas con conversaciones dinámicas, atractivas y personalizadas 1:1. [Chat dinámico](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} permite a los usuarios Marketo Engage empezar a aprovechar el chat como parte clave de las experiencias entre canales integradas para casos de uso de ventas y marketing B2B. Las funciones incluyen: la capacidad de reservar reuniones directamente dentro del chat, enrutamiento de posibles clientes, plantillas de inicio, creación de conversaciones de arrastrar y soltar, y mucho más. El Chat Dinámico está incluido en todos los paquetes de Marketo Engage y será implementado para todos los usuarios Marketo Engage este año.

* **Mejora del filtrado de actividades de bots de correo electrónico**: Como mejora de la versión anterior [Filtrado de actividades de bots de correo electrónico](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md)función {target=&quot;_blank&quot;}, ahora puede incluirse en las actividades de registro que están identificadas como bots. A continuación, puede filtrar y almacenar en déclencheur las acciones basadas en actividades que los bots identifiquen como realizadas.

## Experiencia de próxima generación {#next-generation-experience}

* **Pantallas actualizadas en la experiencia de próxima generación**: Ofrecemos pantallas adicionales y actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador:

   * Vista de lista de formularios en Design Studio (incluidas las nuevas acciones masivas)

* **Importar actualización del flujo de trabajo del programa**: El flujo de trabajo del programa de importación se está entregando en la experiencia de próxima generación con un diseño actualizado y mejoras de uso. Esto será un cambio automático sin un interruptor de alternancia.

* **Control de administración para el conmutador de experiencias de próxima generación**: Administre el despliegue de la experiencia de próxima generación de forma que funcione para los usuarios con la capacidad de los administradores de seleccionar qué tipos de usuarios pueden acceder al conmutador.

## Automatización de la experiencia {#experience-automation}

* **Pasos de flujo de autoservicio (Beta)**: Amplíe la conectividad entre el Marketo Engage y el resto de la pila con la capacidad de crear pasos de flujo personalizados para utilizarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas por lotes y ejecutables, a diferencia de los enlaces web, que solo se pueden utilizar en campañas de déclencheur.

* **Caducidad del recurso**: Mantenga el control de sus campañas y activos que diferencian el tiempo con la capacidad de programar su desactivación automática en una fecha y hora especificadas en la experiencia del usuario de Classic.

* **Anulación de prioridad de campaña inteligente**: Asegúrese de que las campañas inteligentes de déclencheur de alta prioridad se ejecuten lo antes posible con la capacidad de anular la clasificación de prioridad de campaña estándar. Las campañas inteligentes de déclencheur de menor prioridad también se pueden reducir en prioridad para liberar recursos de procesamiento para otras tareas de alta prioridad.

## Mejoras de API {#api-enhancements}

* **Devolver Desactivar el estado de seguimiento abierto de los correos electrónicos**: Permite leer el estado de seguimiento abierto de los correos electrónicos a través de la API
* **Recuperar líneas del asunto de contenido dinámico desde el correo electrónico**: Permite a los especialistas en marketing realizar análisis de las líneas de asunto dinámicas en las herramientas de BI
* **Campos personalizados de miembro del programa CRUD**: Permite a los especialistas en marketing crear mediante programación campos personalizados de miembros del programa
* **Exportación de objetos personalizados masiva actualizadaEn filtro**: Permite a los especialistas en marketing sincronizar mediante programación objetos personalizados
* **Exponer la configuración de inicio del cabezal para programas de correo electrónico**: Permite a los especialistas en marketing configurar programas de correo electrónico con inicio de cabezal mediante API
* **Actualización selectiva de la etiqueta del programa**: Permite a los especialistas en marketing insertar actualizaciones de etiquetas selectivas sin pulsar todas las etiquetas al mismo tiempo
* **Campo Extracción masiva de actividadResultado**: Permite a los especialistas en marketing identificar qué actividades se omitieron o fallaron

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Bizible {#bizible}

![(estrella)](assets/yellow-star.png)

* **Plantillas BI**: Ahora, Bizible proporcionará artefactos de informes y muestras para Tableau e informes básicos descargables para permitir un rápido desarrollo de informes personalizados adaptados a sus necesidades empresariales específicas.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Restricción de conexión de correo electrónico (GA)**: La limitación de la conexión de correo electrónico permite a los administradores de Conexión de ventas configurar la tasa de envío de correos electrónicos al utilizar Gmail o Exchange como canal de envío, de modo que la tasa a la que se entregan los correos electrónicos al proveedor de canales de envío no supere los límites impuestos.

## Anuncios {#announcements}

* **Marketo Sky en desuso**: En marzo, Marketo Sky dejará de estar disponible, ya que centraremos nuestros recursos en ofrecer la experiencia de usuario de próxima generación. En un esfuerzo por mantener el acceso a la funcionalidad que es exclusiva del Marketo Sky actual, incorporamos la caducidad de los recursos y la anulación de la prioridad de las campañas inteligentes en la experiencia clásica. [Haga clic aquí](https://nation.marketo.com/t5/the-next-generation-experience/marketo-sky-deprecation-notice/ba-p/320115#M33) para obtener más información.

**_Seminario web sobre la versión del producto_**

Únase a nosotros el 11 de mayo de 2022, a las 9:00 AM PT / 12:00 PM ET para un [seminario web en directo](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html) alojado por nuestro equipo de productos, donde podrá aprender a utilizar las últimas innovaciones de productos.
