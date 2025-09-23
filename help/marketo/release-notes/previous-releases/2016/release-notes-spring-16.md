---
unique-page-id: 11370952
description: Notas de la versión, primavera de 2016, documentación de Marketo, documentación del producto
title: Notas de la versión, primavera de 2016
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---

# Notas de la versión: primavera de 2016 {#release-notes-spring}

En la versión de primavera de 16 se incluyen las siguientes funciones. Haga clic en los vínculos del título para ver los artículos detallados de cada función.

## [Perspectivas de correo electrónico](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

Perspectivas de correo electrónico es una nueva experiencia histórica de análisis de datos agregados de correo electrónico. Se ha rediseñado de extremo a extremo para ofrecer un rendimiento increíblemente rápido. Cuenta con un diseño de interfaz de usuario completamente nuevo, optimizado para adaptarse a las necesidades y al flujo de trabajo de los especialistas en marketing por correo electrónico.

>[!NOTE]
>
>A partir del 3 de junio, publicaremos por lotes las perspectivas de correo electrónico para los clientes. Nuestro objetivo es completar esto en los próximos meses. Le avisaremos por correo electrónico cuando esté activado.

![](assets/two.png)

## [Selector de plantilla de correo electrónico](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Cree correos electrónicos atractivos con nuestras nuevas plantillas de inicio. Además, localice rápidamente las plantillas desde sus miniaturas en directo.

>[!NOTE]
>
>El Editor de correo electrónico 2.0 (con el Selector de plantillas) se implementará gradualmente a partir del 3 de junio. Completaremos el despliegue antes del 30 de junio. A diferencia de las Perspectivas de correo electrónico, no se le notificará cuando tenga acceso. Para ver si lo hace, siga los pasos de [este artículo](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [Edición por correo electrónico: reinventado](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

Así es, un nuevo editor de correo electrónico! Utilice la funcionalidad ligera de arrastrar y soltar para añadir y reordenar contenido. Los nuevos elementos, incluidas imágenes, vídeos, variables y módulos, seguramente mejorarán su experiencia de edición. Compruebe también la compatibilidad actualizada con el editor de código, el previsualizador y el preencabezado.

![](assets/17a-29-modules-next.png)

## [Mensajes móviles en la aplicación](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Cree impresionantes mensajes en la aplicación para su aplicación directamente en Marketo. Defina exactamente quién debe verlo y cuándo con el programa de mensajes en la aplicación. Monitorice fácilmente su rendimiento con el panel del programa.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [No hay fragmentos de borrador](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Se acabaron los días en los que tenía que volver a aprobar todo cada vez que se actualizaba un fragmento. Con la opción Sin borrador, todos los correos electrónicos y páginas de aterrizaje que utilicen un fragmento de código recibirán las actualizaciones del fragmento y mantendrán su estado anterior. Cada vez que apruebe un fragmento, tendrá la opción de ejecutar Sin borrador y actualizar todo, o crear borradores. ¡Depende de ti! La opción Sin borrador estará disponible para todos los clientes y controlada por un nuevo permiso en Administración.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [Página de aterrizaje, Plantilla de página de aterrizaje y API de formulario](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Las API de REST de Marketo ahora admiten el control sobre páginas de aterrizaje de Marketo, plantillas de páginas de aterrizaje y formularios. Los usuarios ahora pueden crear, actualizar contenido, aprobar y eliminar estos recursos directamente a través de la API de REST de Marketo.

## [Inclusión en la lista de permitidos IP para acceso a API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

Al igual que la función de inclusión en la lista de permitidos de IP para los inicios de sesión de usuarios de Marketo, los administradores de Marketo ahora pueden configurar una lista de permitidos de direcciones IP que pueden acceder a las API de Marketo SOAP y REST, bloqueando así el acceso desde direcciones IP no autorizadas. Esto proporciona un nivel adicional de seguridad a la instancia de Marketo y garantiza que el acceso a la API solo pueda producirse desde la red de la organización. Encontrará detalles sobre cómo configurarlo en el [sitio de documentación de Marketo](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [Nuevo conector de sincronización de Microsoft Dynamics de alta velocidad](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

El nuevo conector de alta velocidad de Dynamics ofrece velocidades de hasta 20 veces más rápidas para la sincronización inicial y hasta 5 veces más rápidas para la sincronización incremental. Todos los clientes nuevos incorporarán este conector en la fecha de lanzamiento y lo implementaremos gradualmente para los clientes existentes durante el periodo de lanzamiento de verano.

**Actualizar datos para nuevos campos**: Ahora puede habilitar nuevos campos de sincronización en cualquier momento y todos los valores de datos de ese campo se actualizarán de [!DNL Dynamics] CRM a Marketo. Ya no hay que preocuparse por seleccionar todos los campos durante la configuración inicial. Si deshabilita un campo de sincronización existente y lo vuelve a habilitar más adelante, todos los valores de datos de ese campo se actualizarán de [!DNL Dynamics] CRM a Marketo.

**Sincronizar posible cliente como contacto**: La acción de flujo de [!UICONTROL Sincronizar posible cliente con Microsoft] tiene una nueva opción para sincronizarse como posible cliente o contacto.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Ficha de administración de errores de sincronización**: examinar, buscar o exportar posibles clientes (y otros objetos) que no se pudieron sincronizar con detalles como la operación, la dirección, el código de error y el mensaje de error.

![](assets/sync-errors.png)

**[!DNL Microsoft Dynamics]2016**: El conector está completamente certificado para [!DNL Dynamics] versiones de [!DNL Online] y [!DNL On-premise] de 2016.

**Ya se han documentado las actualizaciones de complementos:** Consulte el [artículo de documentos sobre actualizaciones de complementos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [Nombre descriptivo de instancia](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

Hoy en día, es difícil diferenciar entre instancias de Marketo, por ejemplo, instancias de zona protegida y de producción. Esta función le permite saber en qué instancias está trabajando actualmente.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Acceso de tiempo limitado para suscripciones](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

Hoy en día, los usuarios están invitados a la suscripción de Marketo por un período de tiempo indefinido. Esta función permite a los administradores invitar a usuarios a suscripciones durante un período de tiempo limitado, por ejemplo, 2 semanas o 1 mes.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Cuadrícula de objetos personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Ahora puede ver el número de registros y campos de todos los objetos personalizados publicados.

![](assets/custom-objects-grid.png)

## Actividades personalizadas {#custom-activities}

Los administradores de Marketo ahora pueden definir y administrar sus tipos de actividades personalizadas mediante el modelador de definición de actividad personalizada de Marketo. De forma similar a (y junto con) Marketo Custom Object Modeler, los administradores ahora pueden ampliar el modelo de datos para adaptarlo a sus necesidades comerciales exactas. Encontrará detalles sobre cómo usar esta funcionalidad en el [sitio de documentación de Marketo](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
