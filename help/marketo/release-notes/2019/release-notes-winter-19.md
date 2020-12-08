---
unique-page-id: 17727823
description: Notas de la versión - Winter '19 - Marketo Docs - Documentación del producto
title: Notas de la versión - Invierno '19
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# Notas de la versión: Invierno &#39;19 {#release-notes-winter}

Las siguientes funciones se incluyen en la versión de invierno de 2019. Compruebe la disponibilidad de las funciones en la edición de marketing.

Haga clic en los vínculos de título para vista de artículos detallados para cada función, si están disponibles.

>[!NOTE]
>
>Facebook ahora requiere una cuenta de Business Manager para aprovechar la integración de Audiencias personalizadas. El servicio LaunchPoint de Facebook *debe* estar asociado a una cuenta de Business Manager o **su integración dejará de funcionar después del 14 de enero de 2019**. Para configurar una cuenta de Business Manager, consulte la Ayuda [de](https://www.facebook.com/business/help/1710077379203657)Facebook.

>[!NOTE]
>
>Microsoft está impulsando a todos los clientes en línea a actualizar a la versión más reciente de Microsoft Dynamics. Si está integrando la instancia de Marketing con Dynamics Online, deberá [actualizar a la versión más reciente de la solución](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md) de Marketing Cloud antes del 31 **de enero de 2019** para asegurarse de que la integración seguirá funcionando.

>[!NOTE]
>
>Marketo está actualizando la versión de OAuth para GoToWebinar de 1.0 a 2.0. La compatibilidad con OAuth 1.0 dejará de utilizarse en enero de 2019. Si es cliente de GoToWebinar, deberá volver a autenticar sus inicios de sesión a través de LaunchPoint (en el área de administración) antes del 31 **de enero de 2019** para asegurarse de que su integración seguirá funcionando. Para más detalles, diríjase a nuestra página [de comunidad](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Mejoras en la plataforma principal {#core-platform-enhancements}

** [Correo electrónico CC para correos electrónicos](../../product-docs/email-marketing/general/email-cc.md)de marketing**

Incluya hasta cinco direcciones CC por destinatario en los correos electrónicos enviados a través de Marketing.

**API**

* **Compatibilidad con dominios de marca múltiple para API de recursos:** La aprobación y clonación de recursos produce los mismos resultados en la API y la interfaz de usuario.
* **Compatibilidad con CC de correo electrónico para API** de recursos: Los usuarios que clonen, aprueben y procesen correos electrónicos mediante la API mantendrán la paridad con la configuración de la interfaz de usuario.

** [Munchkin v155 (Beta)](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo** solo API: Ahora los usuarios pueden determinar cuándo y cómo rastrear a los miembros de su base de datos permitiendo que las aplicaciones web de una sola página llamen explícitamente cuando deseen grabar una visita a una página web en lugar de depender del seguimiento automático de Marketing.
* **Administración** de exclusión: Administre fácilmente las exclusiones al hacer coincidir el dominio de cookies de exclusión con el dominio de cookies de seguimiento de Munchkin.
* **Parámetro** de decisor de nivel de dominio: Dominios de dos letras (p. ej. &quot; [website.io](http://website.io)&quot;) rastreará automáticamente en Marketing sin requisitos de configuración adicionales.

## Compromiso de ventas de marketing {#marketo-sales-engage}

* **Perfil** personalizado de Salesforce: El compromiso de ventas ahora admite perfiles personalizados ilimitados.

* **Personalización** de Salesforce: Al eliminar los campos de actividad personalizados no críticos, los usuarios pueden configurar el compromiso de ventas en la plataforma CRM de forma más eficaz.
* **Servicio** de correo electrónico: Disfrute de una mejor capacidad de entrega, además de un mejor seguimiento de respuestas, una funcionalidad de correo electrónico programado y una funcionalidad de correo electrónico masivo al conectarse a Microsoft Outlook (ya sea a través de Office365 o en espera a través de la ficha Conexión de correo electrónico).
* **Nueva configuración** de administración: Se han agregado dos páginas de administración para optimizar la instancia de compromiso de ventas

   * *Team Management* admite un proceso de configuración de cuentas sin fisuras al permitir que los administradores editen suscripciones y equipos.
   * *La Configuración* de administración de Salesforce ayuda a los equipos a configurar su sincronización SFDC más rápida y fácilmente que nunca.

* **Complemento OWA para Windows**: Con un solo complemento, todos los clientes de Windows Office365 serán compatibles con el compromiso de ventas, lo que permite usar Live Feed en Outlook. El nuevo complemento estará disponible en la Tienda Microsoft.
* **Actividades Pusher**: Sincronice el compromiso de ventas con la plataforma principal de marketing para aprovechar las perspectivas de marketing en tiempo real.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Las liberaciones de Marketo Sky se producen con una cadencia más frecuente. Se espera que las siguientes funciones y mejoras se publiquen a finales del cuarto trimestre o principios del primer trimestre. Para más detalles y actualizaciones, consulte nuestra documentación [de](https://help.marketo.com/hc/en-us/articles/360012858573)Sky.

* **Experiencia** predeterminada opcional: Los usuarios de marketing pueden establecer Marketo Sky como su experiencia predeterminada si un administrador les ha proporcionado acceso.

* **Se reinventó My Marketo**: Personalice su experiencia agregando utilidades que proporcionan información crítica, notificaciones y vínculos a las áreas más visitadas.

* **Vistas de Lista y páginas** de detalles de Design Studio: Disfrute de un mayor nivel de organización y precisión con vistas de lista de correos electrónicos, páginas de aterrizaje y formularios que se pueden filtrar y en las que se pueden buscar. Las páginas de detalles de recursos proporcionan información clave sobre cada recurso, incluidos los programas por los que se utiliza el recurso, el número de fragmentos que se utilizan y mucho más.

* **Búsqueda** global: Marketing ahora oferta una función de búsqueda global más rápida y sólida en toda la plataforma. Las consultas de búsqueda ahora se ejecutan en todos los espacios de trabajo accesibles y pueden buscar recursos (tanto activos como archivados), etiquetas, campañas y programas. Los resultados de la búsqueda se proporcionan mediante una superposición y cada resultado incluye su seguimiento de ubicación de archivos para especificar dónde vive el recurso.

* **Interfaz** de usuario mejorada: Nuevos iconos, modelos y botones, junto con una nueva paleta de colores para reflejar la actualización de nuestra marca y hacer que el Marketo Sky sea aún más impresionante y funcional.

* **Mejoras** en el uso del Programa de correo electrónico: Seguimos avanzando hacia la paridad en la funcionalidad de Programa de correo electrónico entre nuestra plataforma clásica de administración de posibles clientes de Marketing to y la nueva experiencia de Marketo Sky.
* **Programas** de evento con seminario web: Los programas de evento con seminario web ya están disponibles en Marketo Sky (nota: solo GoToWebinar será compatible con esta versión, con más integraciones establecidas a lo largo del tiempo).

## Marketing basado en cuentas {#account-based-marketing}

** [Segmentación y filtrado](../../product-docs/account-based-marketing/using-personas.md)basados en el personal de ABM**

Personalice sus campañas ABM para personas específicas dentro de cuentas con nombre. La función ABM Persona crea un título de trabajo predeterminado basado en la segmentación de posibles clientes y permite la configuración de segmentaciones personales adicionales.

## Analytics {#analytics}

**Biselable**

* **Campos** calculados personalizados: Utilice cualquier atributo Bizsible para crear campos personalizados que se puedan utilizar para el sistema de informes y la segmentación de paneles.

* **Certificación** SOC II Tipo II: La nueva certificación de seguridad y privacidad se basa en la acreditación de tipo I de principios de este año.

## Personalización web {#web-personalization}

**[Añadir subdominios en la configuración de la cuenta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para administrar los dominios y subdominios de forma más eficaz, los usuarios pueden agregar subdominios a la configuración de su cuenta RTP.

## Compromiso con dispositivos móviles de Marketing to (MME) {#marketo-mobile-engagement-mme}

**Kit de desarrollo de software (SDK) MME actualizado para Android**

Hemos actualizado nuestro SDK para Android a un marco de trabajo más moderno, estable y escalable que contiene más flexibilidad y nuevas funciones de ingeniería. Los desarrolladores de aplicaciones de Android ahora pueden utilizar directamente [Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/) (FCM) de Google con este nuevo SDK.

* [Instrucciones para desarrolladores](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Preguntas más frecuentes para desarrolladores](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Los desarrolladores de aplicaciones **deben** actualizar a la nueva versión antes del 31 de marzo de 2019. Si no actualiza el SDK antes del 31 de marzo de 2019, cualquier usuario nuevo que descargue la aplicación después de esta fecha no podrá recibir notificaciones push hasta que actualice a la versión más reciente del SDK. La actualización del SDK no requerirá que los usuarios actuales de la aplicación móvil vuelvan a descargar una nueva versión de la aplicación.

## Actualizaciones adicionales {#additional-updates}

**Extensible plataforma de seminario web**

Además de nuestro lanzamiento de productos, nuestro equipo de socios está trabajando en un nuevo marco que permite a los proveedores de seminarios web crear y mantener sus propias integraciones con Marketing, proporcionando mayor flexibilidad en la actualización y mejora de sus soluciones y permitiendo a los especialistas en mercadotecnia aprovechar al máximo las integraciones elegidas.

Planeamos desplegar nuestra nueva plataforma con proveedores caso por caso. Para obtener más información, consulte los detalles [de nuestro](https://www.marketo.com/why-marketo/partners/technology/) programa o póngase en contacto con su representante de Marketing.
