---
description: Notas de la versión actuales - Documentos de Marketo - Documentación del producto
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 49b1bd707b8394ceeea0984c4c11d3ac88ab81b6
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# Notas de la versión: Enero de 2022 {#release-notes-jan-22}

La versión del 22 de enero incluye las siguientes funciones. Consulte la edición para Marketo Engage de Adobe si hay disponibilidad de funcionalidades.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones se lanzarán en **21 de enero de 2022**.

## Experiencia de próxima generación {#next-generation-experience}

* **Pantallas actualizadas en la experiencia de próxima generación**: Ofrecemos pantallas adicionales y actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso mediante el conmutador:

   * Detalles de los recursos de la página de aterrizaje en Design Studio
   * Detalles del recurso de la página de aterrizaje en actividades de marketing
   * Vista de lista de correo electrónico en Design Studio (incluidas las nuevas acciones masivas)

* **Control de administración para el conmutador de experiencias de próxima generación**: Los administradores pueden seleccionar qué tipos de usuarios pueden acceder al conmutador para ver las pantallas en la experiencia de próxima generación.

## Integración de Microsoft Dynamics {#microsoft-dynamics-integration}

* **Sincronización del tipo de campo Multiselect Optionset Disponible de forma general**: Sincronice el tipo de campo multiselect optionset de Microsoft Dynamics para aprovecharlo en listas inteligentes y campañas inteligentes para una segmentación de audiencia más granular. Algunos ejemplos son: temas/productos de interés, modos de comunicación preferidos, etc. Esta nueva sincronización está disponible para Microsoft Dynamics versión 9.X (incluida Dynamics 365 Online).

* **Autenticación de servidor a servidor para Microsoft Dynamics 365 Online**: Para aumentar la seguridad, ahora admitiremos Servidor a Servidor (S2S) como un modo de autenticación adicional para el usuario de sincronización de Marketo Engage en Azure Active Directory para el acceso no interactivo a Microsoft Dynamics 365 Online. Esto le permite utilizar la autenticación multifactor, ya que todos los inicios de sesión y autenticación se basarán en OAuth (solo el ID de cliente y el secreto de cliente).

>[!NOTE]
>
>El modo S2S se basa en el usuario de la aplicación en lugar de en el usuario con licencia, lo que ahorra el uso de una licencia adicional.

## Administración {#administration}

* **Reglas de validación del formulario**: Mantenga el estado de la base de datos con la capacidad de bloquear los dominios de correo electrónico problemáticos o no deseados para que no envíen formularios de Marketo Engage. El panel Regla de validación de formulario global permite que los administradores definan una lista de bloqueados o habiliten una lista predefinida de dominios de consumo libres para bloquear los formularios.

* **Seguridad del encabezado de la página de aterrizaje**: Los administradores pueden administrar los encabezados Seguridad de transporte estricta y Opciones de X-Frame en sus dominios de página de aterrizaje para aplicar requisitos de seguridad estrictos.

**_Publicación durante el trimestre_**

Las siguientes funciones se encuentran en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Conector de destino del Marketo Engage AEP: Crear nuevos posibles clientes que faltan {#aep-marketo-engage-destination-connector}

Los clientes Marketo Engage que también utilizan Adobe Experience Platform (AEP) pueden maximizar su base de datos con la capacidad de insertar registros de personas nuevas en el Marketo Engage desde AEP a través del conector de destino de AEP. Al enviar segmentos de audiencia de AEP a Marketo Engage, se agregarán automáticamente a él las personas dentro del segmento que no existan en la base de datos de Marketo Engage.

## Conocimiento de ventas {#sales-insight}

![(estrella)](assets/yellow-star.png)

* **Perspectiva de ventas para Salesforce CRM**

* **Nueva columna Tipo para las mejores apuestas**: Los vendedores obtendrán perspectivas más rápidas con una nueva columna etiquetada como &quot;Tipo&quot; para diferenciar entre posibles clientes y contactos en la página Mejores apuestas.

* **Actualización de la API de la plataforma de Salesforce**: En respuesta a las versiones 21.0 a 30.0 de la API de Salesforce Platform que se retira de Salesforce, el paquete de perspectivas de ventas se ha actualizado con las API más recientes.

* **Promoción de marca actualizada**: Todas las páginas de perspectivas de ventas se actualizan para ajustarse a la marca de Adobe.

**Perspectiva de ventas para Microsoft Dynamics**

* **Diseño de cuenta actualizado**: Los vendedores pueden obtener una vista colectiva de las principales actividades, como: actividades de correo electrónico, actividades web, momentos interesantes y cambios de puntuación para todos los contactos de una cuenta.

## Conexión de ventas {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Llamar a resultados y motivos**: Comprenda y rastree los esfuerzos salientes de sus equipos de ventas en más detalle con las opciones nuevas y totalmente personalizables de resultados de llamadas y motivos de llamadas. Además de estos nuevos campos, estamos introduciendo un nuevo gobierno para aplicar el motivo de la llamada y la selección de resultados mientras los vendedores realizan llamadas, un nuevo gobierno para habilitar o deshabilitar los motivos y resultados de la llamada, y un nuevo campo personalizado Razón de la llamada y Actividad de Salesforce de resultados de llamada para registrar datos en Salesforce. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para obtener más información.

* **Personalización de detalles de actividad de Salesforce**: Captura más datos de actividad y tarea de ventas en Salesforce personalizando la información que se agrega al campo de asunto de la tarea de Salesforce cuando se registra una actividad de ventas en Salesforce desde Sales Connect. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para obtener más información.

## Anuncios {#announcements}

* **Apertura del Marketo Sky**: El 11 de marzo, Marketo Sky dejará de estar disponible, ya que centraremos nuestros recursos en ofrecer la experiencia de usuario de próxima generación. En un esfuerzo por mantener el acceso a la funcionalidad que es exclusiva del Marketo Sky actual, incorporamos la caducidad de los recursos y la anulación de la prioridad de las campañas inteligentes en la experiencia principal de marzo.

* **Finalizaciones de formulario en desuso**: Los formularios Marketo Engage rechazarán los POST de formulario programáticos no compatibles con el extremo leadCapture/save2. [Haga clic aquí](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para obtener más información.

* **Verificación de correo electrónico**: A partir de esta versión, las suscripciones de Marketo Engage empezarán a hacer que los usuarios que no sean API solo verifiquen las direcciones de correo electrónico. Los usuarios autenticados del servicio de directorio tendrán automáticamente sus correos electrónicos verificados cuando su suscripción esté habilitada con Verificación de correo electrónico. La verificación de correo electrónico para los usuarios que utilizan la función &quot;Iniciar sesión en el cuadro de diálogo de invitación de usuario&quot; o los que tienen suscripciones que tienen un solo correo electrónico asociado a varios usuarios dentro de la suscripción se retrasará y coincidirá con la obsolescencia de la función en marzo.

* **Iniciar sesión en el cuadro de diálogo Invitar a usuario**: En marzo, la función existente y opcional &quot;Iniciar sesión en el cuadro de diálogo de invitación de usuario&quot; quedará obsoleta. La función &quot;Iniciar sesión en el cuadro de diálogo de invitación de usuario&quot; está anulada por la función de ID universal, que es necesaria para la próxima integración del sistema de Identity Management de Adobe y se habilitó en agosto de 2021 en todas las suscripciones. Como resultado de la desaprobación, el Marketo Engage aplicará todos los ID de usuario (inicios de sesión) para que coincidan con la dirección de correo electrónico del usuario y solo permitirá que un usuario se asocie por dirección de correo electrónico dentro de una suscripción.
