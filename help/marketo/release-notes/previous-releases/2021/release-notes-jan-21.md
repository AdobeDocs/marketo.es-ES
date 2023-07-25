---
description: 'Notas de la versión, enero de 2021, Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Notas de la versión: enero de 2021 {#release-notes-jan-21}

En la versión de enero de 2021 se incluyeron las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![(estrella)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones se lanzarán el **15 de enero de 2021**.

## Experiencia del usuario de próxima generación {#next-generation-user-experience}

* Compatibilidad con espacios de trabajo: la experiencia de usuario Marketo Engage de próxima generación aúna la apariencia de Adobe Experience Cloud con innovaciones productivas para ayudar a los profesionales de marketing a trabajar de forma más rápida e inteligente. En la última versión, se ha añadido compatibilidad total con espacios de trabajo y particiones, incluida la capacidad de compartir carpetas entre espacios de trabajo. El lienzo derecho ofrece un conmutador para permitirle realizar la transición sin problemas entre experiencias antiguas y nuevas por función sin perder contexto. [Más información](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) de las preguntas frecuentes sobre la experiencia de próxima generación en Marketing Nation.

## Personalización multicanal. {#multi-channel-personalization}

* **[Sincronización de audiencias de Adobe Experience Cloud fase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: la capacidad existente de sincronización de audiencias de Adobe Experience Cloud (AEC) ahora admite la sincronización de audiencias B2B continua y bidireccional desde Marketo Engage a otras aplicaciones de AEC, incluidas las ofertas de Adobe Experience Platform (AEP) como Real-time Customer Data Platform y Adobe Experience Platform Activation.  A medida que se agregan y eliminan posibles clientes en los segmentos de audiencia, Marketo Engage sincronizará automáticamente la audiencia actualizada en las aplicaciones de AEC conectadas. Utilícelo para aprovechar las ventajas de la orquestación multicanal de Adobe, la reorientación, la supresión de audiencias, la personalización y los casos de uso de creación de informes en su pila tecnológica de AEC.
* **[Sincronización continua de audiencias con Google, Facebook y LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: la sincronización automatizada y continua con una red de anuncios se puede habilitar en una lista estática, lo que actualiza la red de anuncios como cambios de pertenencia a listas sin necesidad de la intervención del usuario.
* **[Tokens para campos personalizados de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: hemos ampliado las funciones de campo personalizado de los miembros del programa para que admitan el marco de token. Los especialistas en marketing pueden insertar tokens de campos personalizados de miembros de programas en correos electrónicos, páginas de aterrizaje, mensajes SMS, notificaciones push y ganchos web. Utilice nuevos tokens en las acciones de flujo de la campaña para cambiar los valores de los datos, crear una tarea o un momento interesante.

## Páginas de aterrizaje y Forms {#landing-pages-and-forms}

* **API de formulario**: extraiga información sobre posibles clientes o campañas de nutrición de déclencheur mientras extrae datos de formularios que no son de Marketo. Los formularios que no son de Marketo se pueden integrar con Marketo Engage a través de la API de REST. La nueva API permite imitar el envío del formulario de Marketo Engage con todas las funcionalidades asociadas.
* **API de páginas de aterrizaje**: optimice los flujos de trabajo de edición y traducción en aplicaciones integradas con la nueva API de vista previa de la página de aterrizaje. Los proveedores externos ahora pueden procesar vistas previas totalmente personalizadas de páginas de aterrizaje sin iniciar sesión en Marketo Engage.  La API de vista previa de la página de aterrizaje permite flujos de trabajo de edición y localización completos en aplicaciones integradas de terceros.

## Marketing por correo electrónico {#email-marketing}

* **[Límites de recuperación de objetos personalizados aumentados](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: los desarrolladores de scripts de velocidad de correo electrónico pueden aumentar rápidamente el número de objetos personalizados a 100 mediante la anulación de autoservicio. Los especialistas en marketing pueden aumentar la eficacia de las campañas inteligentes accediendo a un mayor número de objetos personalizados de primer y segundo nivel.

## Integración de Salesforce CRM {#salesforce-crm-integration}

* [Autenticación de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): el protocolo OAuth 2.0 está disponible para sincronizar operaciones entre Marketo Engage y Salesforce CRM. Para los nuevos suscriptores, esta opción está activada de forma predeterminada. Los suscriptores actuales pueden solicitar esta función poniéndose en contacto con el Soporte técnico de Marketo.
* [Tablero de sincronización de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): los administradores pueden revisar rápidamente el estado de sincronización de CRM de Salesforce desde el panel. El intervalo de tiempo para sincronizar los informes de rendimiento ha aumentado de 2 horas a 5 días.
* **Exportación de metadatos**: mejorado para admitir atributos de objeto de oportunidad, cuentas con nombre, campos estándar y personalizados del miembro del programa.

## Administration {#administration}

* **Se actualizó la página Mi cuenta**: revise la información de suscripción esencial en la página Mi cuenta. Los usuarios con cualquier nivel de acceso pueden ver el nombre de la suscripción, el identificador del centro de datos y el ID de Munchkin.

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **[Flujos de trabajo de prueba de correo electrónico mejorados (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: aumente la eficacia de su equipo de ventas con flujos de trabajo de correo electrónico de prueba de perspectivas de ventas mejorados. Los vendedores pueden enviar correos electrónicos de prueba a las direcciones de correo electrónico seleccionadas antes de enviar correos electrónicos masivos a un máximo de 200 destinatarios.
* **[Perspectivas del estado del correo electrónico (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Los usuarios ven un mensaje de advertencia cuando intentan enviar un correo electrónico a un ID de correo electrónico no válido o a una dirección de correo electrónico sin suscribirse antes de enviar un correo electrónico.  Los estados de entrega de los correos electrónicos se pueden revisar en la pestaña correo electrónico de Sales Insight.
* **Envío de correos electrónicos masivos desde [Cuenta](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) y [Oportunidad](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) Paneles (Salesforce CRM)**: mejora la eficacia del flujo de trabajo del vendedor y activa una cuenta completa o una lista de contactos de oportunidad con las nuevas funciones de acción masiva. Envíe correos electrónicos o agregue contactos a campañas de Marketo Engage utilizando la nueva opción desplegable en las pestañas de cuenta o oportunidad en lugar de trabajar con contactos individuales. Agregar contactos de cuenta a una lista de observación para recibir notificaciones cuando los posibles clientes se vuelvan activos.
* **[Perspectiva de ventas para integraciones de CRM de Salesforce no nativas](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: las suscripciones de GA con integraciones de CRM de Salesforce personalizadas pueden instalar el paquete de Perspectiva de ventas y ayudar a los equipos de ventas a priorizar e interactuar con los posibles clientes y las oportunidades más prometedoras.
* **[Mejoras recomendadas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Póngase en contacto rápidamente con los posibles clientes desde la pestaña Resultados más probables enviándolos por correo electrónico o añadiéndolos a una campaña de Marketo Engage. Ver un posible cliente en Marketo Engage o agregarlo a la lista de seguimiento. Las acciones masivas y las opciones de clasificación de la pestaña Resultados más probables ahorran tiempo y mejoran la eficacia del equipo de ventas.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Aceleración de la conexión de correo electrónico (BETA)**: Mejore su capacidad de envío de correo electrónico y escale su comunicación de ventas 1:1 con la limitación de la conexión de correo electrónico para Sales Connect. Nuestra nueva tecnología de regulación administra automáticamente el tiempo de envío de los correos electrónicos para crear experiencias sin problemas para los usuarios de Exchange y Gmail. Reduzca o elimine el uso de aplicaciones de envío masivo de correo electrónico de terceros.
* **Seguimiento de rechazos de conexión de correo electrónico**: obtenga información sobre la calidad del posible cliente y el rendimiento de las plantillas de correo electrónico con el nuevo informe de devoluciones de correo electrónico. Los usuarios de Exchange y Gmail pueden optar por recibir notificaciones de rechazo que se acumularán en Live Feed, carpetas de correo electrónico, análisis de plantillas y Campaign Analytics.
* **Configuración de página de perfil**: Administre las preferencias de usuario con facilidad en la nueva página de perfil. Cambie la contraseña, edite la geolocalización y la configuración de idioma y revise los estados de las integraciones en un solo lugar.
* **Administración de plantillas**: organice las plantillas de correo electrónico de ventas en categorías con una nueva función de arrastrar y soltar para garantizar un acceso rápido a las plantillas relevantes y reducir el tiempo de búsqueda.
* **Actualizaciones de experiencia del usuario de Sales Connect**: personalice el diseño de cuadrícula de Sales Connect mediante el cambio de tamaño y la reordenación de columnas. Las preferencias de visualización se guardan automáticamente.

**_Anuncios y desaprobaciones_**

* Todos los usuarios deben actualizar a la última versión de Sales Insight **antes del 15 de enero de 2021**. Si no ha completado la actualización, se le pedirá que lo haga al iniciar sesión en la aplicación. Siga las instrucciones [en esta guía](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La versión actualizada incluye un parche para una vulnerabilidad de seguridad identificada. El parche se publicó originalmente el 6 de abril de 2016. Nota: **Versión 1.4363 o superior** no es necesario realizar una actualización.
* La obsolescencia del servicio Form 1.0 entrará en vigor en **Mayo de 2021** versión. El servicio Forms 1.0 quedará totalmente obsoleto, lo que resultará en la pérdida de funcionalidad de cualquier recurso Forms 1.0 restante que aún se esté utilizando. Además, se rechazarán los envíos de formularios realizados mediante métodos no admitidos, como POST de formularios programáticos a los extremos leadCapture/save y leadCapture/save2. Para obtener más información y correcciones, consulte [Nuestra publicación en Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* En 2021, Marketo Engage realizará cambios en la estructura de la URL para las páginas de aterrizaje, los formularios y los recursos de imágenes y archivos. Para las suscripciones de Marketo Engage existentes, empezaremos el despliegue gradual el 1 de abril de 2021. En marzo de 2021 se publicarán más detalles sobre la cronología del despliegue. Para obtener más información sobre cómo cambiará cada tipo de recurso afectado, consulte [Nuestra publicación en Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Seminario web sobre lanzamiento de productos_**

¿Quiere obtener más información sobre estas funciones y mejoras? Asegúrese de [regístrese ahora](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) Únase a nosotros el 21 de enero a la 1:00 p.m. PT / 4:00 p.m. ET para asistir a un seminario web en directo con nuestro equipo de productos con el fin de profundizar en estas innovaciones.
