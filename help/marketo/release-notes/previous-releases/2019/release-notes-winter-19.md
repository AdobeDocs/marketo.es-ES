---
unique-page-id: 17727823
description: 'Notas de la versión, invierno de 2019, documentación de Marketo: documentación del producto'
title: Notas de la versión, invierno de 2019
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# Notas de la versión: Invierno de 2019 {#release-notes-winter}

Las siguientes funciones están incluidas en la versión de invierno de 1919. Compruebe la disponibilidad de las funciones en Marketo Edition.

Haga clic en los vínculos de título para ver los artículos detallados de cada función, si están disponibles.

>[!NOTE]
>
>[!DNL Facebook] ahora requiere una cuenta de Business Manager para aprovechar su integración de Audiencia personalizada. El servicio [!DNL Facebook]LaunchPoint *debe* estar asociado con una cuenta de Business Manager o **su integración dejará de funcionar después del 14 de enero de 2019**. Para configurar una cuenta de Business Manager, consulta [[!DNL Facebook] Ayuda](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft está empujando a todos los clientes en línea para actualizar a la última versión de [!DNL Microsoft Dynamics]. Si está integrando su instancia de Marketo con [!DNL Dynamics Online], deberá [actualizar a la última versión de la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes del **31 de enero de 2019** para asegurarse de que su integración seguirá funcionando.

>[!NOTE]
>
>Marketo está actualizando la versión de OAuth para el seminario web GoTo de 1.0 a 2.0. La compatibilidad con OAuth 1.0 dejará de usarse en enero de 2019. Si es cliente de GoToWebinar, deberá volver a autenticar sus inicios de sesión a través de LaunchPoint (en el área de Administración) antes del **31 de enero de 2019** para garantizar que su integración siga funcionando. Para obtener más información, consulte nuestra [página de la comunidad](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Mejoras en la plataforma principal {#core-platform-enhancements}

**[Correo electrónico CC para correos electrónicos de Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Incluya hasta cinco direcciones CC por destinatario en los correos electrónicos enviados a través de Marketo.

**API**

* **Compatibilidad con dominios de promoción de varias marcas para la API de recursos:** La aprobación y la clonación de recursos producen los mismos resultados dentro de la API y la interfaz de usuario.
* **Compatibilidad con Email CC para la API de Asset**: Los usuarios que clonen, aprueben y procesen correos electrónicos a través de la API mantendrán la paridad con la configuración de la interfaz de usuario.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo de solo API**: Los usuarios ahora pueden determinar cuándo y cómo rastrear miembros de su base de datos permitiendo que las aplicaciones web de una sola página llamen explícitamente cuando quieran registrar una visita a una página web en lugar de depender del seguimiento automático de Marketo.
* **Administración de exclusión**: Administre fácilmente las exclusiones haciendo coincidir el dominio de cookie de exclusión con el dominio de cookie de seguimiento [!DNL Munchkin].
* **Parámetro de decisor de nivel de dominio**: Los dominios de dos letras (por ejemplo, &quot;[website.io](https://website.io)&quot;) se rastrearán automáticamente en Marketo sin requisitos de configuración adicionales.

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]perfil personalizado**: Sales Engage ahora admite perfiles personalizados ilimitados.

* Personalización **[!DNL Salesforce]**: al eliminar los campos de actividad personalizada no críticos, los usuarios pueden configurar el participación de ventas en la plataforma CRM de forma más eficaz.
* **Servicio de correo electrónico**: disfruta de una mejor capacidad de envío, además de un seguimiento de respuestas mejorado, funcionalidad de correo electrónico programado y funcionalidad de correo electrónico masivo al conectarte a [!DNL Microsoft Outlook] (ya sea a través de Office365 o en la ubicación local a través de la pestaña Conexión de correo electrónico).
* **Nueva configuración de administración**: se han agregado dos páginas de administración para optimizar la instancia de participación en ventas

   * *Team Management* admite un proceso de configuración de cuenta sin problemas, ya que permite a los administradores editar suscripciones y equipos.
   * *Configuración de administración de Salesforce* ayuda a los equipos a configurar la sincronización de SFDC de forma más rápida y sencilla que nunca.

* **Complemento de OWA para[!DNL Windows]**: con un solo complemento, se admitirán todos los clientes de [!DNL Windows Office365] en Sales Engage, lo que permitirá usar Live Feed en Outlook. El nuevo complemento estará disponible en la Tienda Microsoft.
* **Propulsor de actividades**: sincronice el compromiso de ventas con la plataforma principal de Marketo para aprovechar las perspectivas de marketing en tiempo real.

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>[!DNL Marketo Sky] versiones se producen en una cadencia más frecuente. Se espera que las siguientes funciones y mejoras se publiquen durante el último trimestre o principios del primer trimestre. Para obtener más detalles y actualizaciones, consulta nuestra [documentación de Sky](https://help.marketo.com/).

* **Experiencia predeterminada opcional**: Los usuarios de Marketo pueden establecer [!DNL Marketo Sky] como su experiencia predeterminada si un administrador les ha proporcionado acceso.

* **Reimaginé mi Marketo**: personaliza tu experiencia agregando widgets que proporcionen información crítica, notificaciones y enlaces a las áreas que visitas con más frecuencia.

* **Vistas de listas y páginas de detalles de Design Studio**: disfrute de un mayor nivel de organización y precisión con vistas de listas de correos electrónicos, páginas de aterrizaje y formularios que se pueden filtrar y buscar. Las páginas de detalles del recurso proporcionan información clave sobre cada recurso, incluidos los programas en los que se utiliza el recurso, el número de fragmentos que se utilizan, etc.

* **Búsqueda global**: Marketo ahora ofrece una función de búsqueda global más rápida y sólida en toda la plataforma. Las consultas de búsqueda ahora se ejecutan en todos los espacios de trabajo accesibles y pueden buscar recursos (activos y archivados), etiquetas, campañas y programas. Los resultados de búsqueda se proporcionan mediante una superposición y cada resultado incluye su pista de ubicación de archivos para especificar dónde se encuentra el recurso.

* **Interfaz de usuario mejorada**: nuevos iconos, modelos y botones, junto con una nueva paleta de colores para reflejar nuestra actualización de marca y hacer que [!DNL Marketo Sky] sea aún más impresionante y funcional.

* **Mejoras en la usabilidad del programa de correo electrónico**: Seguimos avanzando hacia la paridad en la funcionalidad del programa de correo electrónico entre nuestra plataforma clásica de Marketo Lead Management y la nueva experiencia [!DNL Marketo Sky].
* **Programas de seminarios web con eventos**: Los programas de seminarios web con eventos ya están disponibles en [!DNL Marketo Sky] (nota: en esta versión solo se admitirá GoToWebinar, con integraciones posteriores establecidas a lo largo del tiempo).

## Account-Based Marketing {#account-based-marketing}

**[Segmentación y filtrado basados en personas ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalice sus campañas ABM para personas específicas dentro de cuentas con nombre. La función ABM Persona crea un puesto de trabajo predeterminado basado en la segmentación de posibles clientes y permite la configuración de segmentaciones de personas adicionales.

## Analytics {#analytics}

**[!DNL Bizible]**

* **Campos calculados personalizados**: use cualquier atributo [!DNL Bizible] para generar campos personalizados que se puedan usar para informes y segmentación de tableros.

* **Certificación SOC II de tipo II**: La nueva certificación de seguridad y privacidad se basa en la acreditación de tipo I de principios de este año.

## [!DNL Web Personalization] {#web-personalization}

**[Agregar subdominios en la configuración de la cuenta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para administrar dominios y subdominios de forma más eficaz, los usuarios ahora pueden agregar subdominios a la configuración de su cuenta RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Kit de desarrollo de software (SDK) MME actualizado para Android**

Hemos actualizado SDK para Android a un marco más moderno, estable y escalable que contiene más flexibilidad y nuevas funciones de ingeniería. Los desarrolladores de aplicaciones de Android ahora pueden usar directamente [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) de Google con este nuevo SDK.

* [Instrucciones para desarrolladores](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Preguntas frecuentes para desarrolladores](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Los desarrolladores de aplicaciones **deben** actualizar a la nueva versión antes del 31 de marzo de 2019. Si no actualiza el SDK antes del 31 de marzo de 2019, cualquier usuario nuevo que descargue la aplicación después de esta fecha no podrá recibir notificaciones push hasta que actualice a la última versión de SDK. La actualización de SDK no requerirá que los usuarios de su aplicación móvil actual vuelvan a descargar una versión nueva de su aplicación.

## Actualizaciones adicionales {#additional-updates}

**Plataforma de seminarios web ampliable**

Además de la versión de nuestro producto, nuestro equipo de socios está trabajando en un nuevo marco que permite a los proveedores de seminarios web crear y mantener sus propias integraciones con Marketo, proporcionando más flexibilidad para actualizar y mejorar sus soluciones, a la vez que permite a los especialistas en marketing aprovechar al máximo las integraciones que han elegido.

Planeamos implementar nuestra nueva plataforma con proveedores en base a cada caso. Para obtener más información, consulta nuestros [detalles del programa](https://www.marketo.com/why-marketo/partners/technology/) o ponte en contacto con tu contacto de Marketo.
