---
description: 'Notas de la versión, enero de 2021: Documentación del producto de Marketo'
title: Notas de la versión, enero de 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Notas de la versión: Enero de 2021 {#release-notes-jan-21}

Las siguientes funciones se incluyen en la versión del 21 de enero. Compruebe la disponibilidad de las funciones en su edición de Marketo.

>[!AVAILABILITY]
>
>Las funciones denotadas por una estrella (![(star)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones se lanzarán el **15 de enero de 2021**.

## Experiencia del usuario de próxima generación {#next-generation-user-experience}

* Compatibilidad con espacios de trabajo: La Marketo Engage de la experiencia de usuario de próxima generación aúna la apariencia de Adobe Experience Cloud con innovaciones de productividad para ayudar a los profesionales de marketing a trabajar de forma más rápida y inteligente. En la última versión, hemos añadido compatibilidad total con espacios de trabajo y particiones, incluida la capacidad de compartir carpetas entre espacios de trabajo. El lienzo de la derecha ofrece un conmutador para que pueda realizar una transición sin problemas entre las experiencias antiguas y las nuevas por función sin perder contexto. [Obtenga ](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) más información de las preguntas frecuentes sobre la experiencia de próxima generación en Marketing Nation.

## Personalización multicanal {#multi-channel-personalization}

* **[Fase 3 de sincronización de audiencia de Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: La función de sincronización de audiencias de Adobe Experience Cloud (AEC) existente ahora admite la sincronización de audiencias B2B continua y bidireccional desde el Marketo Engage a otras aplicaciones de AEC, incluidas las ofertas de Adobe Experience Platform (AEP) como la plataforma de datos del cliente en tiempo real y la activación de Adobe Experience Platform.  A medida que los posibles clientes se añadan y eliminen a sus segmentos de audiencia, el Marketo Engage sincronizará automáticamente la audiencia actualizada entre sus aplicaciones de AEC conectadas. Utilícelo para aprovechar los casos de uso de orquestación, reorientación, supresión de audiencias, personalización y creación de informes de varios canales de Adobe en su pila tecnológica de AEC.
* **[Sincronización de audiencias continua con Google, Facebook y LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: La sincronización automatizada continua con una red de publicidad se puede habilitar en una lista estática, actualizando la red de publicidad como cambios de pertenencia a la lista sin necesidad de intervención del usuario.
* **[Tokens para los campos personalizados de miembro del programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Hemos ampliado las características del campo personalizado de miembros del programa para admitir el marco de tokens. Los especialistas en marketing pueden insertar tokens de campos personalizados de miembro del programa en correos electrónicos, páginas de aterrizaje, mensajes SMS, notificaciones push y enlaces web. Utilice tokens nuevos en las acciones de flujo de campaña para cambiar los valores de los datos, crear una tarea o un momento interesante.

## Páginas de aterrizaje y Forms {#landing-pages-and-forms}

* **API** de formulario: Incluya información sobre posibles clientes o campañas de déclencheur mientras extrae datos de formularios que no sean de Marketo. Los formularios que no son de Marketo se pueden integrar con Marketo Engage mediante la API de REST. La nueva API permite imitar el envío de formularios de Marketo Engage con todas las funcionalidades asociadas.
* **API** de páginas de aterrizaje: Optimice los flujos de trabajo de edición y traducción en aplicaciones integradas con la nueva API de vista previa de la página de aterrizaje. Los proveedores de terceros ahora pueden procesar vistas previas totalmente personalizadas de páginas de aterrizaje sin iniciar sesión en el Marketo Engage.  La API de vista previa de página de aterrizaje permite flujos de trabajo de edición y localización de extremo a extremo en aplicaciones integradas de terceros.

## Marketing por correo electrónico {#email-marketing}

* **[Límites de recuperación de objetos personalizados aumentados](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Los desarrolladores de Secuencias de comandos de Velocity de correo electrónico pueden aumentar rápidamente el número de objetos personalizados a 100 mediante la anulación del servidor propio. Los especialistas en marketing pueden aumentar la eficacia de las campañas inteligentes si acceden a un mayor número de objetos personalizados de primer y segundo nivel.

## Integración de Salesforce CRM {#salesforce-crm-integration}

* [Autenticación de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): El protocolo OAuth 2.0 está disponible para las operaciones de sincronización entre Marketo Engage y Salesforce CRM. Para los nuevos suscriptores, esta opción está habilitada de forma predeterminada. Los suscriptores actuales pueden solicitar esta función poniéndose en contacto con el servicio de asistencia técnica de Marketo.
* [Panel de sincronización de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Los administradores pueden revisar rápidamente el estado de sincronización de Salesforce CRM desde el panel. La sincronización de la duración del informe de rendimiento se ha aumentado de 2 a 5 días.
* **Exportación** de metadatos: Se ha mejorado para admitir atributos de objeto de oportunidad, cuentas con nombre, campos estándar y personalizados del miembro del programa.

## Administración {#administration}

* **Se ha actualizado la página** Mi cuenta: Revise la información de suscripción esencial en la página Mi cuenta . Los usuarios con cualquier nivel de acceso pueden ver el nombre de la suscripción, el identificador del centro de datos y el ID de Munchkin.

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Conocimiento de ventas {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **[Flujos de trabajo de prueba de correo electrónico mejorados (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Aumente la eficacia de su equipo de ventas con flujos de trabajo de correo electrónico de prueba de perspectivas de ventas mejorados. Los vendedores pueden enviar correos electrónicos de prueba a las direcciones de correo electrónico seleccionadas antes de enviar correos electrónicos masivos a hasta 200 destinatarios.
* **[Perspectivas del estado del correo electrónico (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Los usuarios ven un mensaje de advertencia cuando intentan enviar un correo electrónico a un ID de correo electrónico no válido o a una dirección de correo electrónico que se ha dado de baja antes de enviar un correo electrónico.  Los estados de entrega de correo electrónico se pueden revisar en la pestaña de correo electrónico de la perspectiva de ventas.
* **Enviar correos electrónicos masivos desde  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) Account and  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) OportunityPanels (Salesforce CRM)**: Mejore la eficacia del flujo de trabajo del vendedor y participe con una lista de contactos de cuenta o oportunidad completa mediante el uso de nuevas funciones de acción masiva. Envíe correos electrónicos o agregue contactos a campañas de Marketo Engage utilizando la nueva opción desplegable en las pestañas cuenta o oportunidad en lugar de trabajar con contactos individuales. Agregue contactos de cuenta a una lista de observación para recibir notificaciones cuando los posibles clientes se vuelvan activos.
* **[Perspectiva de ventas para integraciones](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)** CRM de Salesforce no nativas: Las suscripciones GA con integraciones personalizadas de Salesforce CRM pueden instalar el paquete de perspectivas de ventas y ayudar a los equipos de ventas a priorizar e interactuar con los posibles clientes y oportunidades más prometedores.
* **[Mejoras](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** recomendadas: Póngase en contacto rápidamente con posibles clientes activos desde la pestaña Best Bets enviando un correo electrónico o agregándolos a una campaña de Marketo Engage. Ver un posible cliente en el Marketo Engage o agregarlo a la lista de observación. Las acciones masivas y las opciones de ordenación en la ficha Mejor apuesta ahorran tiempo y mejoran la eficacia del equipo de ventas.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Restricción de conexión de correo electrónico (BETA)**: Mejore su capacidad de envío de correo electrónico y escale su comunicación de ventas 1:1 con la restricción de conexión de correo electrónico para conexión de ventas. Nuestra nueva tecnología de regulación administra automáticamente el tiempo de envío de correo electrónico para crear experiencias sin fisuras para los usuarios de Exchange y Gmail. Reduzca o elimine el uso de aplicaciones de envío masivo de correo electrónico de terceros.
* **Seguimiento de devoluciones de conexión de correo electrónico**: Obtenga información sobre la calidad de los posibles clientes y el rendimiento de las plantillas de correo electrónico con el nuevo informe de devoluciones de correo electrónico. Los usuarios de Exchange y Gmail pueden optar por recibir notificaciones de devoluciones que se resumirán en la fuente activa, las carpetas de correo electrónico, los análisis de plantillas y Campaign Analytics.
* **Configuración** de página de perfil: Administre las preferencias de usuario con facilidad en la nueva página de perfil. Cambie la contraseña, edite la geolocalización y la configuración de idioma, y revise los estados de integraciones en un solo lugar.
* **Administración de plantillas**: Organice las plantillas de correo electrónico de ventas en categorías con una nueva función de arrastrar y soltar para garantizar un acceso rápido a las plantillas relevantes y reducir el tiempo de búsqueda.
* **Actualizaciones** de la experiencia del usuario de Conexión de ventas: Personalice el diseño de la cuadrícula Conexión a ventas mediante el cambio de tamaño y la reordenación de columnas. Las preferencias de visualización se guardan automáticamente.

**_Anuncios y casos de finalización del soporte_**

* Todos los usuarios deben actualizar a la última versión de Sales Insight **antes del 15 de enero de 2021**. Si no ha completado la actualización, se le pedirá que lo haga al iniciar sesión en la aplicación. Siga las instrucciones [de esta guía](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La versión actualizada incluye un parche para una vulnerabilidad de seguridad identificada. El parche se publicó originalmente el 6 de abril de 2016. Nota: **Las versiones 1.4363 o superiores** no necesitan realizar una actualización.
* La desaprobación del servicio Form 1.0 entrará en vigor en la versión **de mayo de 2021**. El servicio Forms 1.0 quedará totalmente obsoleto, lo que provocará la pérdida de funcionalidad de los recursos restantes de Forms 1.0 que aún estén en uso. Además, se rechazarán los envíos de formularios realizados mediante métodos no compatibles, como los formularios programáticos POSTs a los extremos leadCapture/save y leadCapture/save2. Para obtener más información y corrección, consulte [nuestra publicación en Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* En 2021, Marketo Engage realizará cambios en la estructura de la URL para páginas de aterrizaje, formularios, imágenes y recursos de archivos. Para las suscripciones de Marketo Engage existentes, comenzaremos el lanzamiento gradual el 1 de abril de 2021. En marzo de 2021 se publicarán más detalles sobre el calendario de lanzamiento. Para obtener más información sobre cómo cambiará cada tipo de recurso afectado, consulte [nuestra publicación en Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Seminario web sobre la versión del producto_**

¿Quiere obtener más información sobre estas funciones y mejoras? Asegúrese de [registrarse ahora](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) para unirse a nosotros el 21 de enero a las 13:00 PT / 4:00 PM ET para un seminario web en vivo con nuestro equipo de productos para profundizar en estas innovaciones.
