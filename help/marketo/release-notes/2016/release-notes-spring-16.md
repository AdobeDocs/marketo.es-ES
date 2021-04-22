---
unique-page-id: 11370952
description: Notas de la versión - Primavera 16 - Documentos de Marketo - Documentación del producto
title: Notas de la versión - Primavera de 2016
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Notas de la versión: Primavera &#39;16 {#release-notes-spring}

Las siguientes funciones están incluidas en la versión de primavera del 2016. Haga clic en los vínculos de título para ver los artículos detallados de cada función.

## [Perspectivas de correo electrónico](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

Email Insights es una experiencia de análisis de correo electrónico de datos agregados históricos completamente nueva, rediseñada de principio a fin para ofrecer un rendimiento rápido como parte del proyecto Orion. Incluye un diseño de interfaz de usuario completamente nuevo y optimizado para adaptarse a las necesidades y al flujo de trabajo de los especialistas en marketing por correo electrónico.

>[!NOTE]
>
>A partir del 3 de junio, se lanzarán por lotes Perspectivas de correo electrónico a los clientes. Nuestro objetivo es completarlo en los próximos meses. Le notificaremos por correo electrónico cuando esté habilitado.

![](assets/two.png)

## [Selector de plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Cree correos electrónicos bonitos con nuestras nuevas plantillas de inicio. Además, localice rápidamente sus plantillas desde sus miniaturas en vivo.

>[!NOTE]
>
>El Editor de correo electrónico 2.0 (con el Selector de plantilla) se implementará gradualmente a partir del 3 de junio. Completaremos el despliegue para el 30 de junio. A diferencia de las perspectivas de correo electrónico, no se le notificará cuando tenga acceso. Para ver si lo hace, siga los pasos en [este artículo](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [Edición de correo electrónico: reinventado](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

¡Eso es, un nuevo editor de correo electrónico! Utilice la sencilla funcionalidad de arrastrar y soltar para añadir y reordenar contenido. Los nuevos elementos, como imágenes, vídeos, variables y módulos, seguramente mejorarán su experiencia de edición. Consulte también la actualización del editor de código, la vista previa y la compatibilidad con el encabezado previo.

![](assets/17a-29-modules-next.png)

## [Mensajes en la aplicación móviles](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Cree impresionantes mensajes en la aplicación directamente en Marketo. Defina exactamente quién debe verlo y cuándo con el programa de mensajes en la aplicación. Monitorice fácilmente su rendimiento con el panel del programa.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [Sin recortes de borrador](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Ya no están los días en los que tiene que volver a aprobar todo cada vez que se actualiza un fragmento. Con Sin borrador, todos los correos electrónicos y páginas de aterrizaje que utilicen un fragmento de código recibirán las actualizaciones de fragmento y mantendrán sus estados anteriores. Cada vez que apruebe un fragmento, tendrá la opción de ejecutar Sin borrador y actualizar todo, o crear borradores. ¡Depende de ti! No-Draft estará disponible para todos los clientes y controlado por un nuevo permiso en Administración.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [Página de aterrizaje, plantilla de página de aterrizaje y API de formulario](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Las API de REST de Marketo ahora admiten el control sobre páginas de aterrizaje, plantillas de página de aterrizaje y formularios de Marketo. Los usuarios ahora pueden crear, actualizar contenido, aprobar y eliminar estos recursos directamente a través de la API de REST de Marketo.

## [INCLUSIÓN EN LA LISTA DE PERMITIDOS IP para acceso a API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

Al igual que la función de inclusión en la lista de permitidos de IP para los inicios de sesión de usuario de Marketo, los administradores de Marketo ahora pueden configurar una lista de permitidos de direcciones IP que puedan acceder a las API SOAP y REST de Marketo, bloqueando así el acceso desde direcciones IP no autorizadas. Esto proporciona una capa adicional de seguridad a la instancia de Marketo y garantiza que el acceso a la API solo pueda producirse desde la red de la organización. Los detalles sobre cómo configurarlo están disponibles en el [sitio de documentación de Marketo](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [Nuevo conector de sincronización de Microsoft Dynamics de alta velocidad](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

Construido sobre la arquitectura Orion, el nuevo conector de dinámica de alta velocidad proporciona velocidades hasta 20 veces más rápidas para la sincronización inicial y hasta 5 veces más rápidas para la sincronización incremental. Todos los clientes nuevos se incorporarán a este conector en la fecha de lanzamiento y lo implementaremos gradualmente para los clientes existentes en el lapso de tiempo de lanzamiento del verano.

**Actualización de datos para campos** nuevos: Ahora puede habilitar nuevos campos de sincronización en cualquier momento y todos los valores de datos de ese campo se actualizarán de Dynamics CRM a Marketo. Ya no te preocupes por tener que seleccionar todos los campos durante la configuración inicial. Si desactiva un campo de sincronización existente y lo vuelve a habilitar más tarde, todos los valores de datos de ese campo se actualizarán de Dynamics CRM a Marketo.

**Sincronizar posible cliente como contacto**: La acción de flujo Sincronizar posible cliente con Microsoft tiene una nueva opción para sincronizar como posible cliente o contacto.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Pestaña** de administración de errores de sincronización: Examinar, buscar o exportar posibles clientes (y otros objetos) que no se hayan sincronizado con detalles como operación, dirección, código de error y mensaje de error.

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**: El conector está completamente certificado para las versiones en línea y locales de Dynamics 2016.

**Las actualizaciones de complementos ya están documentadas:** consulte el artículo  [de los documentos de actualizaciones de complementos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [Nombre de instancia reconocible](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

En la actualidad, es difícil diferenciar entre instancias de Marketo, por ejemplo, entornos limitados y instancias de producción. Esta función le permite saber en qué instancias está trabajando.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Acceso a tiempo limitado para suscripciones](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

En la actualidad, se invita a los usuarios a la suscripción a Marketo durante un período de tiempo indefinido. Esta función permite a los administradores invitar a los usuarios a suscripciones durante un período de tiempo limitado, por ejemplo, 2 semanas o 1 mes.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Cuadrícula de objetos personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Ahora puede ver el número de registros y campos de todos los objetos personalizados publicados.

![](assets/custom-objects-grid.png)

## Actividades personalizadas {#custom-activities}

Los administradores de Marketo ahora pueden definir y administrar sus tipos de actividades personalizados mediante el modelador de definición de actividad personalizada de Marketo. Al igual que (y junto con) el Modelador de objetos personalizados de Marketo, los administradores ahora pueden ampliar el modelo de datos para adaptarlo a sus necesidades empresariales exactas. Los detalles sobre cómo utilizar esta funcionalidad están disponibles en el [sitio de documentación de Marketo](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
