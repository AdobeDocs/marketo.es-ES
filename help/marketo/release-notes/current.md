---
description: Notas de la versión actuales - Documentos de Marketo - Documentación del producto
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 538622707eec53e9a137e9aed7ec448d379efe43
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Notas de la versión: Octubre de 2022 {#release-notes-oct-22}

A continuación encontrará todas las funciones incluidas en la versión del 22 de octubre. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

Las siguientes funciones empezarán a lanzarse en **14 de octubre de 2022**, con un despliegue gradual de las funciones restantes en las semanas siguientes (a menos que se especifique lo contrario). Las funciones de la versión y las fechas exactas están sujetas a cambios.

## Organización en canales múltiples {#cross-channel-orchestration}

* **Organizar automáticamente los flujos de diálogo para la conversación dinámica**: Mejore su lienzo de diálogo lleno organizando todo en el lienzo en un formato limpio y fácil de leer con la pulsación de un botón a través de la organización automática.

* **Compatibilidad con tipos de datos adicionales para Dynamic Chat**: Tres nuevos tipos de datos (booleano, entero, flotante) le permiten aprovechar los campos de Marketo Engage existentes en Dynamic Chat para cosas como el targeting basado en puntuaciones o preguntar a los visitantes sí/no preguntas.

* **Vínculos de reunión para Dynamic Chat**: Opción para incluir automáticamente un vínculo de equipos o reunión para Google y Outlook en cada invitación de calendario que se envíe a los visitantes.

* **Notificaciones de reuniones programadas para chat dinámico**: Los representantes de ventas reciben notificaciones automatizadas por correo electrónico con respecto a las reuniones programadas, así como cualquier información relevante sobre la interacción de bots de chat del visitante.

* **Roles y permisos para Dynamic Chat**: Los administradores pueden utilizar permisos granulares para controlar la visibilidad y el uso de la aplicación y crear funciones de usuario personalizadas.

   * Acceso total: los usuarios pueden aprovechar al máximo la función (p. ej., publicar cuadros de diálogo, cambiar esquema de colores, etc.)
   * Acceso de solo lectura: los usuarios pueden ver información, pero no pueden realizar cambios (por ejemplo, consulte Criterios de audiencia o Diseñador de flujo, pero no modificar)
   * Acceso restringido: los usuarios no pueden ver ni acceder a las secciones Configuración o Integraciones

## Experiencia de próxima generación {#next-generation-experience}

* **Pantallas actualizadas en la experiencia de próxima generación**: Ofrecemos pantallas adicionales y actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador:

   * Detalles de la plantilla de página de aterrizaje
   * Lista de plantillas de correo electrónico

* **Mejora utilizada por la pestaña en Detalles de plantilla de correo electrónico**: En la nueva experiencia, verá información adicional relacionada con los recursos que utilizan la plantilla de correo electrónico, incluidos Estado del recurso, Última modificación y Última modificación por. También puede buscar, ordenar y filtrar la lista de recursos que usan.

* **Modelos del filtro de recursos de informes**: Nuevo diseño para los modelos de configuración de informes que muestran un nuevo árbol de recursos en el menú de configuración y un filtro para Fecha de creación y modificación.

## Entorno de datos de marketing {#marketing-data-environment}

* **Integración del Privacy Service de Adobe**: Armonice con el Privacy Service para automatizar el cumplimiento de las normas de privacidad de datos en todos los productos de Experience Cloud. Actualmente, este servicio solo está disponible para los clientes Marketo Engage que hayan incorporado al [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target=&quot;_blank&quot;} Sistema.

## Mejoras de API {#api-enhancements}

* **Importación masiva de posibles clientes: Asociación de vendedores**: Paridad con la API de Lead REST para poder asociar posibles clientes con los vendedores durante el proceso de importación de posibles clientes en masa, lo que reduce la complejidad y el número de llamadas de API necesarias.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **[Integración de perspectivas de ventas con Dynamic Chat](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target=&quot;_blank&quot;}**: El panel de perspectivas ahora incluye actividades de chat dinámico en la cuadrícula inteligente junto con un resumen semanal y tarjetas de detalle.

## Anuncios {#announcements}

* **Forms 1.0**: La desaprobación de Forms 1.0 se completará con la versión de octubre. Los recursos de Forms 1.0 ya no podrán enviar datos al Marketo Engage y devolverán errores si se intenta hacerlo.

* **Forms sin script**: Forms dejará de funcionar cuando Javascript esté deshabilitado en el explorador. El envío de formularios requerirá que Javascript esté habilitado.
