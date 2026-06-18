---
title: 2019
description: '2019: Documentos de Marketo: documentación del producto'
feature: Release Information
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
  - id: de9e3aa9-f002-4fe1-897b-09ee3c55114b
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 5247efff11566852d4c7271f1d212cc233593c19
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 0%

---

# 2019

## Invierno de 2019 {#winter}

Las siguientes funciones están incluidas en la versión de invierno de 1919. Compruebe la disponibilidad de las funciones en Marketo Edition.

Haga clic en los vínculos de título para ver los artículos detallados de cada función, si están disponibles.

>[!NOTE]
>
>[!DNL Facebook] ahora requiere una cuenta de Business Manager para aprovechar su integración de Audiencia personalizada. El servicio *LaunchPoint [!DNL Facebook] debe* estar asociado con una cuenta de Business Manager o **su integración dejará de funcionar después del 14 de enero de 2019**. Para configurar una cuenta de Business Manager, consulta [[!DNL Facebook] Ayuda](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft está empujando a todos los clientes en línea para actualizar a la última versión de [!DNL Microsoft Dynamics]. Si está integrando su instancia de Marketo con [!DNL Dynamics Online], deberá [actualizar a la última versión de la solución de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes del **31 de enero de 2019** para asegurarse de que su integración seguirá funcionando.

>[!NOTE]
>
>Marketo está actualizando la versión de OAuth para el seminario web GoTo de 1.0 a 2.0. La compatibilidad con OAuth 1.0 dejará de usarse en enero de 2019. Si es cliente de GoToWebinar, deberá volver a autenticar sus inicios de sesión a través de LaunchPoint (en el área de Administración) antes del **31 de enero de 2019** para garantizar que su integración siga funcionando. Para obtener más información, consulte nuestra [página de la comunidad](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Mejoras en la plataforma principal

**[Correo electrónico CC para correos electrónicos de Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Incluya hasta cinco direcciones CC por destinatario en los correos electrónicos enviados a través de Marketo.

**API**

* **Compatibilidad con dominios de promoción de varias marcas para la API de recursos:** La aprobación y la clonación de recursos producen los mismos resultados dentro de la API y la interfaz de usuario.
* **Compatibilidad con Email CC para la API de Asset**: Los usuarios que clonen, aprueben y procesen correos electrónicos a través de la API mantendrán la paridad con la configuración de la interfaz de usuario.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo de solo API**: Los usuarios ahora pueden determinar cuándo y cómo rastrear miembros de su base de datos permitiendo que las aplicaciones web de una sola página llamen explícitamente cuando quieran registrar una visita a una página web en lugar de depender del seguimiento automático de Marketo.
* **Administración de exclusión**: Administre fácilmente las exclusiones haciendo coincidir el dominio de cookie de exclusión con el dominio de cookie de seguimiento [!DNL Munchkin].
* **Parámetro de decisor de nivel de dominio**: Los dominios de dos letras (por ejemplo, &quot;[website.io](https://website.io)&quot;) se rastrearán automáticamente en Marketo sin requisitos de configuración adicionales.

## Marketo Sales Engage

* **[!DNL Salesforce]perfil personalizado**: Sales Engage ahora admite perfiles personalizados ilimitados.

* Personalización **[!DNL Salesforce]**: al eliminar los campos de actividad personalizada no críticos, los usuarios pueden configurar el participación de ventas en la plataforma CRM de forma más eficaz.
* **Servicio de correo electrónico**: disfruta de una mejor capacidad de envío, además de un seguimiento de respuestas mejorado, funcionalidad de correo electrónico programado y funcionalidad de correo electrónico masivo al conectarte a [!DNL Microsoft Outlook] (ya sea a través de Office365 o en la ubicación local a través de la pestaña Conexión de correo electrónico).
* **Nueva configuración de administración**: se han agregado dos páginas de administración para optimizar la instancia de participación en ventas

   * *Team Management* admite un proceso de configuración de cuenta sin problemas, ya que permite a los administradores editar suscripciones y equipos.
   * *Configuración de administración de Salesforce* ayuda a los equipos a configurar la sincronización de SFDC de forma más rápida y sencilla que nunca.

* **Complemento de OWA para[!DNL Windows]**: con un solo complemento, se admitirán todos los clientes de [!DNL Windows Office365] en Sales Engage, lo que permitirá usar Live Feed en Outlook. El nuevo complemento estará disponible en la Tienda Microsoft.
* **Propulsor de actividades**: sincronice el compromiso de ventas con la plataforma principal de Marketo para aprovechar las perspectivas de marketing en tiempo real.

## [!DNL Marketo Sky]

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

## Account-Based Marketing

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

Hemos actualizado nuestro SDK para Android a un marco más moderno, estable y escalable que contiene más flexibilidad y nuevas funciones de ingeniería. Los desarrolladores de aplicaciones de Android ahora pueden usar directamente [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) de Google con este nuevo SDK.

* [Instrucciones para desarrolladores](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Preguntas frecuentes sobre desarrolladores](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Los desarrolladores de aplicaciones **deben** actualizar a la nueva versión antes del 31 de marzo de 2019. Si no actualiza el SDK antes del 31 de marzo de 2019, cualquier usuario nuevo que descargue la aplicación después de esta fecha no podrá recibir notificaciones push hasta que actualice a la última versión de SDK. La actualización de SDK no requerirá que los usuarios de su aplicación móvil actual vuelvan a descargar una versión nueva de su aplicación.

## Actualizaciones adicionales {#additional-updates}

**Plataforma de seminarios web ampliable**

Además de la versión de nuestro producto, nuestro equipo de socios está trabajando en un nuevo marco que permite a los proveedores de seminarios web crear y mantener sus propias integraciones con Marketo, proporcionando más flexibilidad para actualizar y mejorar sus soluciones, a la vez que permite a los especialistas en marketing aprovechar al máximo las integraciones que han elegido.

Planeamos implementar nuestra nueva plataforma con proveedores en base a cada caso. Para obtener más información, consulta nuestros [detalles del programa](https://www.marketo.com/why-marketo/partners/technology/) o ponte en contacto con tu contacto de Marketo.

## Primavera de 2019 {#spring}

Las siguientes funciones se incluyen en la versión de primavera de 1919. Compruebe la disponibilidad de las funciones en Marketo Edition.

Haga clic en los vínculos de título para ver los artículos detallados de cada función, si están disponibles.

***Versiones trimestrales_**

Las siguientes funciones se lanzaron el 15 de marzo de 2019.

## Mejoras en la plataforma principal

* **En lista de espera:** Nuevo estado de programa/evento para poner en lista de espera a un miembro cuando quieras [ponerlo en espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) hasta que se abra una vacante. Esto se aplica a los canales asociados con los programas de eventos en Marketo Classic, así como a los eventos y eventos con los programas de seminarios web de [!DNL Marketo Sky]. De forma predeterminada, Lista de espera tiene el mismo valor de paso que Registrado.
* **[Límite de comunicación personalizada](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**: los administradores ahora pueden establecer límites de comunicación diarios o semanales personalizados.
* **[API de recursos de campaña inteligente](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**: enriquece tu análisis fuera de Marketo con la recuperación del registro de campaña inteligente por fecha e ID actualizados.
* **Vínculos de seguimiento HTTPS para correo electrónico:** Para los clientes que han adquirido &quot;Dominios seguros para el seguimiento de vínculos&quot;, los vínculos de seguimiento de marca ahora se pueden mostrar en sus correos electrónicos como HTTPS.
* **Actualizaciones del Powerpack de envío de correo electrónico**: capacidad para marcar y comentar resultados de pruebas específicas, compartir resultados con partes interesadas a través de una dirección URL y realizar un seguimiento de los cambios para ver la evolución de un correo electrónico a medida que las partes interesadas editan el contenido.

Account-Based Marketing

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)** ahora disponible de forma general. AccountAI utiliza inteligencia artificial para revelar las cuentas que debe orientar para su estrategia ABM.

<br> 

**_Versiones no trimestrales_**

Se espera que las siguientes funciones se publiquen durante el primer trimestre natural y al comienzo del segundo trimestre de 2019.

## [!DNL Marketo Sky]

* **Funcionalidad completa del programa de correo electrónico**: Envíe correos electrónicos, cree pruebas A/B y realice un seguimiento de los resultados para disfrutar de una experiencia fácil de usar.
* **Funcionalidad de campañas inteligentes**: Disfruta de una mayor estabilidad en una nueva interfaz de usuario a medida que la funcionalidad de campañas inteligentes continúa desplegándose en Sky.
* **Administrar Assets de Design Studio**: Se ha agregado la capacidad de administrar plantillas, imágenes, Forms, fragmentos de código, archivos, correos electrónicos y páginas de aterrizaje de forma masiva desde las vistas de lista de Design Studio.
* **Tablero de zona horaria de entrega a destinatario**: Comprenda el comportamiento de los clientes con los informes de los correos electrónicos enviados mediante la función de zona horaria de entrega a destinatario en Sky.

## Marketo Sales Engage

* **Auditoría mejorada**: Nueva visibilidad de todas las personas, correos electrónicos y [contenido](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md) en una instancia con capacidad agregada para [finalizar campañas existentes](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)creadas por otros usuarios.
* **[Administración de cancelación de suscripción](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**: Maximice la capacidad de entrega y el cumplimiento con la capacidad de [bloquear los dominios de correo electrónico](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md) para que no se pongan en contacto con ellos. Marketo también hará referencia cruzada a la base de datos de posibles clientes para las cancelaciones de suscripción antes de enviar un correo electrónico.

## [!DNL Bizible] por Marketo

* **[!DNL Bizible]Discover Mejoras en la característica**: Las nuevas capacidades de segmentación de tableros permiten a los especialistas en marketing comprender mejor el rendimiento.
* **Compatibilidad con múltiples monedas**: cambie entre su moneda corporativa y cualquier moneda local con la nueva funcionalidad de conversión de moneda automática de [!DNL Bizible] creada en tablas de moneda CRM.
* **Costos de campaña de CRM**: mida el gasto y el ROI de las actividades de marketing sin conexión con la capacidad de extraer automáticamente los datos de costo del objeto de campaña de CRM.

## Junio de 2019 {#june}

Las siguientes funciones se incluyen en la versión de junio de 2019. Compruebe la disponibilidad de las funciones en Marketo Edition.

**_Versiones trimestrales_**

Las siguientes funciones se lanzaron el 14 de junio de 2019.

## Servicios principales de Marketo {#marketo-core-services}

* **Suma de comprobación de archivos de extracción masiva**: compruebe que se recuperó un archivo completo comparando el hash de archivo con la cadena de suma de comprobación de los trabajos de extracción completados.
* **Migración automatizada del correo electrónico 1.0 al correo electrónico 2.0**: El correo electrónico 2.0 es totalmente compatible con los correos electrónicos y las plantillas de correo electrónico 1.0. Disfrute de nuevas funciones, como la capacidad de agrupar elementos de contenido (imágenes, texto, etc.) En módulos, defina variables como Cadena, Color, Imagen, etc. en las plantillas y aproveche las plantillas de inicio totalmente adaptables. También incluye un Selector de plantillas de correo electrónico visual.

>[!CAUTION]
>
>Desde el 18 de junio de 2019, el correo electrónico 1.0 ya no está disponible. Puede obtener más información sobre el correo electrónico 2.0 y la obsolescencia del correo electrónico 1.0 [aquí](https://nation.marketo.com/docs/DOC-7038).

## Account-Based Marketing

* **[!DNL LinkedIn]Coincidencia de cuenta (BETA)** : Una nueva funcionalidad ABM ya está disponible en versión beta, lo que le ofrece la capacidad de enviar listas de cuentas conocidas y de espacio en blanco directamente desde Marketo a LinkedIn. Esta funcionalidad se incluye automáticamente para todos los clientes de Marketo ABM.

<br> 

**_Lanzamiento durante todo el trimestre_**

Se espera que las siguientes funciones se publiquen durante el segundo trimestre natural y a principios del tercer trimestre de 2019.

## [!DNL Marketo Sky]

* **Límites para eventos** y **Objetivos de eventos** están disponibles generalmente en [!DNL Marketo Sky] bajo el complemento Eventos Premium.

   * Límites de eventos: optimice la experiencia del cliente con sus eventos y seminarios web con límites de registro, redirecciones de páginas y funciones de listas de espera.
   * Objetivos del evento: establezca los objetivos de registro y asistencia del evento y realice un seguimiento del progreso en tiempo real.

* **Vínculos de navegación completos**: Hemos habilitado la navegación en todas las aplicaciones con permisos, como Hootsuite, Calendar y más.
* **Vistas de correo electrónico, página de aterrizaje, fragmento, formulario, imagen y lista de archivos**: vea, busque y realice acciones masivas en cualquiera de sus recursos en Design Studio.
* **Página de detalles de imagen, archivo y fragmento**: obtenga detalles rápidos sobre sus recursos con metadatos como _creados en/por_ y acciones como _eliminar_ y _aprobar_.
* **Widget de publicaciones de blog de la comunidad**: Acceda a las publicaciones recientes de la comunidad en Mi Marketo.
* **Widget que caduca pronto**: agregue el widget &quot;caducará pronto&quot; a su panel de My Marketo para ver qué campañas y páginas de aterrizaje están configuradas para caducar a continuación.
* **Más tarjetas de listas inteligentes**: Segmente y oriente correctamente con tarjetas de listas inteligentes adicionales, incluidos el paso de flujo &quot;Crear tarea&quot;, las reglas de listas inteligentes de CRM y mucho más.
* **Página de detalles del campeón/aspirante de correo electrónico**: vea datos como criterios ganadores, creados en, etc., de sus pruebas de campeón/aspirante de correo electrónico.

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* **Acciones masivas en la personalización de [!DNL Salesforce]**: Maximice la productividad enviando correos electrónicos y agregando contactos a las campañas de forma masiva con la personalización de [!DNL Salesforce].
* **Configuración - [!DNL Salesforce] página para administradores y no administradores**: administre su instancia de [!DNL Sales Connect] con una vista clara de la instancia de [!DNL Salesforce] conectada a [!DNL Sales Connect], así como Mi correo electrónico a [!DNL Salesforce] actualizaciones. La configuración de sincronización mejorada para Administradores, No administradores y Sincronización en todo el equipo se lanzará en los próximos meses.
* **Configuración - Página de integración**: una tienda integral para todas sus integraciones, para que pueda aprovechar al máximo nuestro ecosistema abierto.
* **Configuración - Página de perfil**: vea y actualice los detalles de su cuenta, cambie la contraseña y compruebe el estado de implementación de su instancia en esta nueva página de perfil.

* **Plantillas de correo electrónico del sistema**: Funciones actualizadas de diseño, capacidad de respuesta e internacionalización.

## [!DNL Bizible] por Marketo

* **Compatibilidad con múltiples monedas para[!DNL Dynamics]**: [!DNL Bizible] ahora se adapta a [!DNL Microsoft Dynamics] tablas de moneda, de modo que puede cambiar fácilmente entre las monedas corporativas y locales. (Nota: La compatibilidad con SFDC se publicó en el primer trimestre de 2019).
* **Integración de Drift**: Entienda cómo las conversaciones de Drift afectan el recorrido de su cliente. [!DNL Bizible] también extraerá direcciones de correo electrónico de las conversaciones para crear un posible cliente nuevo o conectar el punto de contacto a un posible cliente existente.
* **Localización**: [!DNL Bizible] ya está disponible en todos los idiomas compatibles con Marketo (inglés, japonés, alemán, español, francés y portugués).

_&#x200B;**Seminario web sobre la versión del producto**&#x200B;_ Vea la grabación de nuestro seminario web sobre innovaciones en la versión de junio de 2019 [aquí](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html).

## Agosto de 2019 {#august}

Las siguientes funciones están incluidas en la versión de agosto de 1919. Compruebe la disponibilidad de las funciones en Marketo Edition.

**_Versiones trimestrales_**

Las siguientes funciones se lanzaron el 16 de agosto de 2019.

## Core Marketo Engage {#core-marketo-engage}

* **Ampliable Webinar Framework**: Ahorre tiempo con el nuevo módulo de seminarios web incorporado de Marketo (introducido en las notas de la versión de invierno de 2019) que pasa sin problemas los datos de los proveedores de seminarios web a Marketo y viceversa. Cvent y Zoom ya están disponibles en este nuevo marco.
* **Actualización de la API de Smart Campaign**: administre las capacidades del ciclo de vida de las campañas inteligentes a medida que redondeamos la interfaz CRUD (crear, leer, actualizar, eliminar).
* **Actualizar cambio de API de encabezados de correo electrónico**: la API de actualización de encabezados de correo electrónico ya no requiere que un correo electrónico tenga una plantilla adjunta para actualizar los campos de encabezado, como la línea de asunto.

**Account-Based Marketing** ![(estrella)](assets/yellow-star.png)

* **[!DNL LinkedIn]La coincidencia de cuentas**, que antes estaba en la versión beta, ya está disponible de forma general.
* **AccountAI** se está convirtiendo oficialmente en **perfil de cuenta**.

<br> 

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante el tercer trimestre natural y a principios del cuarto trimestre de 2019.

**[!DNL Marketo Sales Connect]** ![(estrella)](assets/yellow-star.png)

* **Mejora del diseño de página de personas:** Administre a sus personas y grupos mediante importaciones de listas y acciones masivas en el diseño de página de nuevas personas.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![(estrella)](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo para obtener más información.

>[!NOTE]
>
>**Desuso de TLS 1.0 y 1.1**: Para alinearnos con el estándar de seguridad de primer nivel de Adobe, dejaremos de admitir TLS 1.0 y 1.1 a partir del 13 de diciembre de 2019. Los sistemas integrados con Marketo que no cumplan con el protocolo 1.2 podrían perder el acceso a los servicios de Marketo Engage.
>
>**Para mantener su acceso a Marketo Engage, asegúrese de que todos los sistemas cliente sean compatibles con TLS 1.2 antes del 13 de diciembre de 2019**. Encontrará información más detallada [aquí](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).

**_Seminario web sobre la versión del producto_** [Únase a nosotros](https://engage.marketo.com/August_19_Release_Webinar.html) el 28 de agosto a las 1:00PM PT / 4:00PM ET para asistir a un seminario web en directo organizado por nuestro equipo de productos y obtener más información sobre las funciones incluidas en esta versión.

