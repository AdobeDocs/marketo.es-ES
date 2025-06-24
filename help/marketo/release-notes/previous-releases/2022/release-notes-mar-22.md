---
description: 'Notas de la versión, marzo de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, marzo de 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Notas de la versión: marzo de 2022 {#release-notes-mar-22}

Las siguientes funciones se incluyen en la versión de marzo de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **11 de marzo de 2022**, con un despliegue gradual de cada característica en las semanas siguientes (a menos que se especifique lo contrario).

## Orquestación entre canales {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**: Maximice todas las oportunidades en su sitio web al segmentar tanto los posibles clientes como las cuentas con conversaciones proactivas, atractivas y personalizadas 1:1. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permite a los usuarios de Marketo Engage empezar a aprovechar el chat como parte clave de las experiencias integradas en canales múltiples para los casos prácticos de ventas y marketing B2B. Las funciones incluyen: la capacidad de reservar reuniones directamente dentro del chat, enrutamiento de posibles clientes, plantillas de inicio, creación de conversaciones de arrastrar y soltar y mucho más. Dynamic Chat está incluido en todos los paquetes de Marketo Engage y se implementará para todos los usuarios de Marketo Engage este año.

* **Mejora del filtrado de actividades de bots de correo electrónico**: como mejora de la característica [Filtrado de actividades de bots de correo electrónico](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} lanzada anteriormente, ahora puede optar por registrarse en las actividades identificadas como bots. A continuación, puede filtrar y almacenar en déclencheur las acciones basadas en actividades identificadas como realizadas por bots.

## Experiencia de próxima generación {#modern-ux}

* **Screens actualizado en la experiencia de próxima generación**: Estamos ofreciendo pantallas adicionales actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia:

   * Vista de lista de formularios en [!UICONTROL Design Studio] (incluidas las nuevas acciones masivas)

* **Actualización del flujo de trabajo del programa de importación**: El flujo de trabajo del programa de importación se está entregando en la experiencia de próxima generación con un diseño actualizado y mejoras de uso. Se trata de un cambio automático sin conmutador.

* **Control de administración para el conmutador de alternancia de experiencia de próxima generación**: administre el despliegue de la experiencia de próxima generación de una manera que funcione para los usuarios con la capacidad para que los administradores seleccionen qué tipos de usuarios pueden acceder al conmutador de alternancia.

## Automatización de experiencias {#experience-automation}

* **Pasos de flujo de autoservicio (Beta)**: expanda la conectividad entre Marketo Engage y el resto de su pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas por lotes y ejecutables, a diferencia de los webhooks, que solo se pueden utilizar en campañas de déclencheur.

* **Caducidad de recursos**: mantenga el control de sus campañas y recursos en los que el tiempo es un factor importante con la capacidad de programar su desactivación automática en una fecha y hora especificadas en la experiencia del usuario de Classic.

* **Anulación de prioridad de campaña inteligente**: Asegúrese de que las campañas inteligentes de déclencheur de alta prioridad se ejecuten lo antes posible con la capacidad de anular la clasificación de prioridad de campaña estándar. Las campañas inteligentes de déclencheur de menor prioridad también se pueden reducir en prioridad para liberar recursos de procesamiento para otras tareas de alta prioridad.

## Mejoras de API {#api-enhancements}

* **Devolver Deshabilitar estado de seguimiento abierto de correos electrónicos**: permite leer el estado de seguimiento abierto de los correos electrónicos a través de la API
* **Recuperar líneas de asunto de contenido dinámico del correo electrónico**: permite a los especialistas en marketing realizar análisis de las líneas de asunto dinámicas en las herramientas de BI
* **Campos personalizados de miembros de programa CRUD**: permite a los especialistas en marketing crear mediante programación campos personalizados de miembros de programa
* **Exportación masiva de objetos personalizados actualizadaEn el filtro**: permite a los especialistas en marketing sincronizar objetos personalizados mediante programación
* **Exponer la configuración de Head Start para programas de correo electrónico**: permite a los especialistas en marketing configurar programas de correo electrónico con Head Start a través de API
* **Actualización selectiva de etiquetas de programa**: permite a los especialistas en marketing insertar actualizaciones selectivas de etiquetas sin insertar todas las etiquetas al mismo tiempo
* **Campo actionResult de extracción masiva de actividades**: permite a los especialistas en marketing identificar qué actividades se omitieron o fallaron

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## [!DNL Bizible] {#bizible}

![(estrella)](assets/yellow-star.png)

* **Plantillas de BI**: [!DNL Bizible] ahora proporcionará artefactos de informes básicos descargables e informes de muestra para Tableau y Power BI para permitir el desarrollo rápido de informes personalizados adaptados a sus necesidades comerciales específicas.

## [!DNL Sales Connect] {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Restricción de conexión de correo electrónico (GA)**: la restricción de conexión de correo electrónico permite a los administradores de [!DNL Sales Connect] configurar la tasa de envío de correos electrónicos al usar Gmail o [!DNL Exchange] como canal de envío, de modo que la tasa a la que se entregan los correos electrónicos al proveedor del canal de envío no supere los límites forzados.

## Anuncios {#announcements}

* **Desaprobación de Marketo Sky**: En marzo, Marketo Sky dejará de estar disponible, ya que centramos nuestros recursos en ofrecer la experiencia de usuario de próxima generación. Con el fin de mantener el acceso a una funcionalidad exclusiva de Marketo Sky hoy en día, hemos incorporado la caducidad de los recursos y la anulación de prioridad de las campañas inteligentes a la experiencia clásica. [Haga clic aquí](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para obtener más información.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de marzo y mayo de 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
