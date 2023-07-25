---
unique-page-id: 17727823
description: 'Notas de la versión, invierno de 2019, documentación de Marketo: documentación del producto'
title: Notas de la versión, invierno de 2019
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# Notas de la versión: Invierno de 2019 {#release-notes-winter}

Las siguientes funciones están incluidas en la versión de invierno de 1919. Compruebe la disponibilidad de las funciones en Marketo Edition.

Haga clic en los vínculos de título para ver los artículos detallados de cada función, si están disponibles.

>[!NOTE]
>
>Facebook ahora requiere una cuenta de Business Manager para aprovechar su integración de Audiencias personalizadas. Su servicio de Facebook LaunchPoint *debe* estar asociado a una cuenta de Business Manager o **La integración dejará de funcionar a partir del 14 de enero de 2019**. Para configurar una cuenta de Business Manager, consulte [Ayuda de facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft está instando a todos los clientes en línea a actualizar a la última versión de Microsoft Dynamics. Si está integrando la instancia de Marketo con Dynamics Online, deberá [actualice a la última versión de la solución Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes **31 de enero de 2019** para garantizar que la integración siga funcionando.

>[!NOTE]
>
>Marketo está actualizando la versión de OAuth para el seminario web GoTo de 1.0 a 2.0. La compatibilidad con OAuth 1.0 dejará de usarse en enero de 2019. Si es cliente de GoToWebinar, deberá volver a autenticar sus inicios de sesión a través de LaunchPoint (en el área de Administración) mediante **31 de enero de 2019** para garantizar que la integración siga funcionando. Para obtener más información, consulte nuestra [Página de comunidad](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Mejoras en la plataforma principal {#core-platform-enhancements}

**[CC de correo electrónico para correos electrónicos de Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Incluya hasta cinco direcciones CC por destinatario en los correos electrónicos enviados a través de Marketo.

**API**

* **Compatibilidad con dominios de promoción de varias marcas para la API de recursos:** La aprobación y la clonación de recursos producen los mismos resultados dentro de la API y la interfaz de usuario.
* **Compatibilidad con Email CC para la API de recursos**: Los usuarios que clonen, aprueben y procesen correos electrónicos a través de la API mantendrán la paridad con la configuración de la interfaz de usuario.

**[Munchkin v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo de solo API**: Los usuarios ahora pueden determinar cuándo y cómo rastrear miembros de su base de datos permitiendo que las aplicaciones web de una sola página llamen explícitamente a cuando deseen registrar una visita a una página web en lugar de depender del seguimiento automático de Marketo.
* **Administración de la exclusión**: Administre fácilmente las exclusiones haciendo coincidir el dominio de la cookie de exclusión con el dominio de la cookie de seguimiento de Munchkin.
* **Parámetro de decisor de nivel de dominio**: dominios de dos letras (es decir, &quot; [website.io](https://website.io)&quot;) rastreará automáticamente en Marketo sin requisitos de configuración adicionales.

## Marketo Sales Engage {#marketo-sales-engage}

* **Perfil personalizado de Salesforce**: Sales Engage ahora admite perfiles personalizados ilimitados.

* **Personalización de Salesforce**: Al eliminar los campos de actividad personalizada no críticos, los usuarios pueden configurar Sales Engage en la plataforma CRM de forma más eficaz.
* **Servicio de correo electrónico**: disfrute de una mejor capacidad de entrega, además de un seguimiento de respuestas mejorado, una funcionalidad de correo electrónico programado y una funcionalidad de correo electrónico masivo conectándose a Microsoft Outlook (a través de Office 365 o local a través de la pestaña Conexión de correo electrónico ).
* **Nueva configuración de administración**: Se han añadido dos páginas de administración para optimizar la instancia de participación en ventas

   * _Administración de equipo_ admite un proceso de configuración de cuentas sin problemas, ya que permite a los administradores editar suscripciones y equipos.
   * _Configuración de administración de Salesforce_ ayuda a los equipos a configurar la sincronización de SFDC de forma más rápida y sencilla que nunca.

* **Complemento OWA para Windows**: con un solo complemento, todos los clientes de Windows Office 365 serán compatibles con Sales Engage, lo que permite utilizar Live Feed en Outlook. El nuevo complemento estará disponible en la Tienda Microsoft.
* **Propulsor de actividades**: sincronice Sales Engage con la plataforma principal de Marketo para aprovechar las perspectivas de marketing en tiempo real.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Las liberaciones del Marketo Sky se producen en una cadencia más frecuente. Se espera que las siguientes funciones y mejoras se publiquen durante el último trimestre o principios del primer trimestre. Para obtener más información y actualizaciones, consulte nuestra [Documentación de Sky](https://help.marketo.com/).

* **Experiencia predeterminada opcional**: los usuarios de Marketo pueden establecer Marketo Sky como su experiencia predeterminada si un administrador les ha proporcionado acceso.

* **Reinventé Mi Marketo**: personalice su experiencia añadiendo widgets que proporcionen información crítica, notificaciones y vínculos a las áreas visitadas con más frecuencia.

* **Design Studio Vistas de lista y páginas de detalles**: disfrute de un mayor nivel de organización y precisión con vistas de listas de correos electrónicos, páginas de aterrizaje y formularios que se pueden filtrar y buscar. Las páginas de detalles del recurso proporcionan información clave sobre cada recurso, incluidos los programas en los que se utiliza el recurso, el número de fragmentos que se utilizan, etc.

* **Búsqueda global**: Marketo ahora ofrece una función de búsqueda global más rápida y sólida en toda la plataforma. Las consultas de búsqueda ahora se ejecutan en todos los espacios de trabajo accesibles y pueden buscar recursos (activos y archivados), etiquetas, campañas y programas. Los resultados de búsqueda se proporcionan mediante una superposición y cada resultado incluye su pista de ubicación de archivos para especificar dónde se encuentra el recurso.

* **Interfaz de usuario mejorada**: nuevos iconos, modelos y botones, junto con una nueva paleta de colores para reflejar nuestra actualización de marca y hacer que el Marketo Sky sea aún más impresionante y funcional.

* **Mejoras de uso del programa de correo electrónico**: Seguimos avanzando hacia la paridad en la funcionalidad del programa de correo electrónico entre nuestra plataforma Marketo Lead Management clásica y la nueva experiencia del Marketo Sky.
* **Programas De Seminarios Web Con Eventos**: los programas de evento con seminario web ya están disponibles en Marketo Sky (nota: en esta versión solo se admitirá GoToWebinar, con más integraciones establecidas a lo largo del tiempo).

## Account-Based Marketing {#account-based-marketing}

**[Segmentación y filtrado basados en personas de ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalice sus campañas ABM para personas específicas dentro de cuentas con nombre. La función ABM Persona crea un puesto de trabajo predeterminado basado en la segmentación de posibles clientes y permite la configuración de segmentaciones de personas adicionales.

## Analytics {#analytics}

**Bizible**

* **Campos calculados personalizados**: utilice cualquier atributo de Bizible para crear campos personalizados que se puedan usar para la segmentación y la creación de informes de tableros.

* **Certificación SOC II Tipo II**: La nueva certificación de seguridad y privacidad se basa en la acreditación Tipo I de principios de este año.

## Personalización web {#web-personalization}

**[Agregar subdominios en la configuración de la cuenta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para administrar dominios y subdominios de forma más eficaz, los usuarios ahora pueden agregar subdominios a la configuración de su cuenta RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Kit de desarrollo de software (SDK) MME actualizado para Android**

Hemos actualizado nuestro SDK para Android a un marco de trabajo más moderno, estable y escalable que contiene más flexibilidad y nuevas funciones de ingeniería. Los desarrolladores de aplicaciones de Android ahora pueden utilizar directamente el de Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) con este nuevo SDK.

* [Instrucciones para desarrolladores](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Preguntas frecuentes sobre desarrolladores](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Desarrolladores de aplicaciones **debe** actualización a la nueva versión antes del 31 de marzo de 2019. Si no actualiza el SDK antes del 31 de marzo de 2019, cualquier usuario nuevo que descargue la aplicación después de esta fecha no podrá recibir notificaciones push hasta que actualice a la última versión del SDK. La actualización del SDK no requerirá que los usuarios de la aplicación móvil existentes vuelvan a descargar una versión nueva de la aplicación.

## Actualizaciones adicionales {#additional-updates}

**Plataforma de seminarios web extensible**

Además de la versión de nuestro producto, nuestro equipo de socios está trabajando en un nuevo marco que permite a los proveedores de seminarios web crear y mantener sus propias integraciones con Marketo, proporcionando más flexibilidad para actualizar y mejorar sus soluciones, a la vez que permite a los especialistas en marketing aprovechar al máximo las integraciones que han elegido.

Planeamos implementar nuestra nueva plataforma con proveedores en base a cada caso. Para obtener más información, consulte nuestra [detalles del programa](https://www.marketo.com/why-marketo/partners/technology/) o póngase en contacto con su contacto de Marketo.
