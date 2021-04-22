---
unique-page-id: 17727823
description: Notas de la versión - Invierno '19 - Marketo Docs - Documentación del producto
title: Notas de la versión - Invierno '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# Notas de la versión: Invierno &#39;19 {#release-notes-winter}

Las siguientes funciones están incluidas en la versión de invierno de 2019. Compruebe la disponibilidad de las funciones en su edición de Marketo.

Haga clic en los vínculos de título para ver los artículos detallados de cada función, si están disponibles.

>[!NOTE]
>
>Facebook ahora requiere una cuenta de Business Manager para aprovechar la integración de Audiencia personalizada. El servicio de Facebook LaunchPoint *debe* asociarse con una cuenta de Business Manager o **su integración dejará de funcionar después del 14 de enero de 2019**. Para configurar una cuenta de Business Manager, consulte [Ayuda de Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft está presionando a todos los clientes en línea para que actualicen a la versión más reciente de Microsoft Dynamics. Si está integrando su instancia de Marketo con Dynamics Online, deberá [actualizar a la última versión de la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes del **31 de enero de 2019** para asegurarse de que la integración seguirá funcionando.

>[!NOTE]
>
>Marketo está actualizando la versión de OAuth para GoToWebinar de 1.0 a 2.0. La compatibilidad con OAuth 1.0 dejará de usarse en enero de 2019. Si es cliente de GoToWebinar, deberá volver a autenticar sus inicios de sesión a través de LaunchPoint (en el área de administración) antes del **31 de enero de 2019** para asegurarse de que su integración seguirá funcionando. Para obtener más información, consulte nuestra [página de la comunidad](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Mejoras en la plataforma principal {#core-platform-enhancements}

**[Email CC para correos electrónicos de Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Incluya hasta cinco direcciones CC por destinatario en correos electrónicos enviados a través de Marketo.

**API**

* **Compatibilidad de dominios de marca múltiple con la API de recursos:** la aprobación y clonación de recursos produce los mismos resultados en la API y la IU.
* **Compatibilidad con Email CC para la API** de recursos: Los usuarios que clonen, aprueben y procesen correos electrónicos a través de la API mantendrán la paridad con la configuración de la interfaz de usuario.

**[Munchkin v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo** de solo API: Los usuarios ahora pueden determinar cuándo y cómo rastrear miembros de su base de datos permitiendo que las aplicaciones web de una sola página llamen explícitamente cuando desean registrar una visita de página web en lugar de depender del seguimiento automático de Marketo.
* **Administración de exclusión**: Administre fácilmente las exclusiones al hacer coincidir el dominio de la cookie de exclusión con el dominio de la cookie de seguimiento de Munchkin.
* **Parámetro** de decisor de nivel de dominio: Dominios de dos letras (p. ej. &quot;  [website.io](https://website.io)&quot;) rastreará automáticamente en Marketo sin requisitos de configuración adicionales.

## Participación de ventas de Marketo {#marketo-sales-engage}

* **Perfil** personalizado de Salesforce: El compromiso de ventas ahora admite perfiles personalizados ilimitados.

* **Personalización de Salesforce**: Al eliminar los campos de actividad personalizados no críticos, los usuarios pueden configurar el compromiso de ventas en la plataforma CRM de forma más eficaz.
* **Servicio** de correo electrónico: Disfrute de una mejor capacidad de envío, además de un mejor seguimiento de respuestas, una funcionalidad de correo electrónico programado y una funcionalidad de correo electrónico masivo al conectarse a Microsoft Outlook (a través de Office365 o local a través de la pestaña Conexión de correo electrónico).
* **Nueva configuración** de administración: Se han agregado dos páginas de administración para optimizar la instancia de participación en ventas

   * _Team_ Management admite un proceso de configuración de cuentas fluido al permitir que los administradores editen suscripciones y equipos.
   * _Los equipos de Salesforce Admin_ Settings configuran su sincronización SFDC más rápido y fácil que nunca.

* **Complemento OWA para Windows**: Con un solo complemento, todos los clientes de Windows Office365 serán compatibles con el compromiso de ventas, lo que proporciona la capacidad de usar Live Feed en Outlook. El nuevo complemento estará disponible en Microsoft Store.
* **Pusher** de actividades: Sincronice el compromiso de ventas con la plataforma principal de Marketo para aprovechar las perspectivas de marketing en tiempo real.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Las versiones de Marketo Sky se producen en una cadencia más frecuente. Se espera que las siguientes funciones y mejoras se publiquen a finales del cuarto trimestre o principios del primer trimestre. Para obtener más información y actualizaciones, consulte nuestra [Documentación de Sky](https://help.marketo.com/).

* **Experiencia** predeterminada opcional: Los usuarios de Marketo pueden establecer el Marketo Sky como su experiencia predeterminada si un administrador les ha proporcionado acceso.

* **Se reinventó Mi Marketo**: Personalice su experiencia agregando utilidades que proporcionen información crítica, notificaciones y vínculos a las áreas más visitadas.

* **Vistas de lista y páginas de detalles de Design Studio**: Disfrute de un mayor nivel de organización y precisión con vistas de lista filtrables y con capacidad de búsqueda de correos electrónicos, páginas de aterrizaje y formularios. Las páginas de detalles de los recursos proporcionan información clave sobre cada recurso, incluidos los programas por los que se utiliza el recurso, el número de fragmentos que se utilizan, etc.

* **Búsqueda global**: Marketo ahora ofrece una función de búsqueda global más rápida y sólida en toda la plataforma. Las consultas de búsqueda ahora se ejecutan en todos los espacios de trabajo accesibles y pueden buscar recursos (tanto activos como archivados), etiquetas, campañas y programas. Los resultados de la búsqueda se proporcionan mediante una superposición y cada resultado incluye su pista de ubicación de archivo para especificar dónde se encuentra el recurso.

* **Interfaz** de usuario mejorada: Nuevos iconos, modales y botones, junto con una nueva paleta de colores que refleja la actualización de nuestra marca y hace que el Marketo Sky sea aún más impresionante y funcional.

* **Mejoras en el uso del programa de correo electrónico**: Seguimos avanzando hacia la paridad en la funcionalidad del Programa de correo electrónico entre nuestra plataforma clásica de gestión de posibles clientes de Marketo y la nueva experiencia de Marketo Sky.
* **Programas de Evento Con Seminario Web**: Los programas de Evento con seminario web ya están disponibles en Marketo Sky (nota: solo se admitirá GoToWebinar en esta versión, con más integraciones establecidas a lo largo del tiempo).

## Marketing basado en cuentas {#account-based-marketing}

**[Segmentación y filtrado basados en el personal de ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalice sus campañas ABM para personas específicas dentro de cuentas con nombre. La función ABM Persona crea un título de trabajo predeterminado basado en la segmentación de clientes potenciales y permite la configuración de segmentaciones de personal adicionales.

## Analytics {#analytics}

**Bizible**

* **Campos** calculados personalizados: Utilice cualquier atributo Bizible para crear campos personalizados que se puedan utilizar para la segmentación y los informes del panel.

* **Certificación** SOC II Tipo II: La nueva certificación de seguridad y privacidad se basa en la acreditación de tipo I de principios de este año.

## Personalización web {#web-personalization}

**[Agregar subdominios en la configuración de la cuenta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para administrar los dominios y subdominios de forma más eficaz, los usuarios ahora pueden agregar subdominios a la configuración de su cuenta RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Kit de desarrollo de software (SDK) MME actualizado para Android**

Hemos actualizado nuestro SDK para Android a un marco más moderno, estable y escalable que contiene más flexibilidad y nuevas funciones de ingeniería. Los desarrolladores de aplicaciones de Android ahora pueden utilizar directamente [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) de Google con este nuevo SDK.

* [Instrucciones para desarrolladores](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Preguntas más frecuentes sobre desarrolladores](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Los desarrolladores de aplicaciones **deben** actualizar a la nueva versión antes del 31 de marzo de 2019. Si no actualiza el SDK antes del 31 de marzo de 2019, cualquier usuario nuevo que descargue la aplicación después de esta fecha no podrá recibir notificaciones push hasta que actualice el SDK a la última versión. La actualización del SDK no requerirá que los usuarios de la aplicación móvil existentes vuelvan a descargar una nueva versión de la aplicación.

## Actualizaciones adicionales {#additional-updates}

**Plataforma de seminarios web extensible**

Además de nuestra versión del producto, nuestro equipo de socios está trabajando en un nuevo marco que permite a los proveedores de seminarios web crear y mantener sus propias integraciones con Marketo, lo que proporciona más flexibilidad para actualizar y mejorar sus soluciones, al tiempo que permite a los especialistas en marketing sacar el máximo partido de las integraciones que elijan.

Planeamos implementar nuestra nueva plataforma con proveedores caso por caso. Para obtener más información, consulte nuestros [detalles del programa](https://www.marketo.com/why-marketo/partners/technology/) o póngase en contacto con su contacto de Marketo.
