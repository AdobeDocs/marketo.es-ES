---
description: 'Notas de la versión, enero de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Notas de la versión: enero de 2022 {#release-notes-jan-22}

Las siguientes funciones se incluyen en la versión de enero de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **21 de enero de 2022**, con un despliegue gradual de cada característica en las semanas siguientes (a menos que se especifique lo contrario).

## Experiencia de próxima generación {#modern-ux}

* **Screens actualizado en la experiencia de próxima generación**: Estamos ofreciendo pantallas adicionales actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia:

   * Detalles del recurso de la página de aterrizaje en [!UICONTROL Design Studio]
   * Detalles del recurso de la página de aterrizaje en [!UICONTROL actividades de marketing]

## Integración de [!DNL Microsoft Dynamics] {#microsoft-dynamics-integration}

* **Sincronización del tipo de campo de conjunto de opciones de selección múltiple disponible de forma general**: sincronice el tipo de campo de conjunto de opciones de selección múltiple de [!DNL Microsoft Dynamics] para aprovecharlo en las listas inteligentes y las campañas inteligentes para una segmentación de audiencia más granular. Algunos ejemplos son: temas/productos de interés, modos de comunicación preferidos y mucho más. Esta nueva sincronización está disponible para [!DNL Microsoft Dynamics] versión 9.X (incluida Dynamics 365 Online).

* **Autenticación de servidor a servidor para[!DNL Microsoft Dynamics 365 Online]**: para aumentar la seguridad, ahora se admitirá Servidor a servidor (S2S) como un modo de autenticación adicional para el usuario de sincronización de Marketo Engage en Azure Active Directory para el acceso no interactivo a [!DNL Microsoft Dynamics 365 Online]. Esto le permite emplear la autenticación de varios factores, ya que toda la autenticación y los inicios de sesión se basarán en OAuth (solo ID de cliente y secreto de cliente).

>[!NOTE]
>
>El modo S2S se basa en el usuario de la aplicación en lugar de en el usuario con licencia, lo que evita el uso de una licencia adicional.

## Administración {#administration}

* **[Reglas de validación de formularios](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: mantenga el estado de la base de datos con la capacidad de bloquear los dominios de correo electrónico problemáticos o no deseados para que no envíen formularios de Marketo Engage. El panel Regla de validación de formulario global permite a los administradores definir una lista de bloqueados o habilitar una lista predefinida de dominios de consumidores libres para bloquear formularios.

* **[Seguridad de encabezado de página de aterrizaje](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: los administradores pueden administrar encabezados de seguridad de transporte estricta y opciones X-Frame en los dominios de su página de aterrizaje para aplicar requisitos de seguridad estrictos.

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Conector de destino de AEP Marketo Engage: crear posibles clientes nuevos {#aep-marketo-engage-destination-connector}

Los clientes de Marketo Engage que también utilizan Adobe Experience Platform (AEP) pueden maximizar su base de datos con la capacidad de insertar nuevos registros de personas en Marketo Engage desde AEP a través del conector de destino de AEP. Al enviar segmentos de audiencia de AEP a Marketo Engage, se pueden agregar automáticamente a las personas del segmento que no existan en la base de datos de Marketo Engage [1.](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)

## [!DNL Sales Insight] {#sales-insight}

![(estrella)](assets/yellow-star.png)

**[!DNL Sales Insight]para [!DNL Salesforce] CRM**

* **Nueva columna de tipo para [!UICONTROL Lo más probable]**: Los vendedores obtendrán perspectivas más rápidas con una nueva columna denominada &quot;Tipo&quot; para diferenciar entre posibles clientes y contactos en la página [!UICONTROL Lo más probable].

* **[!DNL Salesforce]Actualización de la API de plataforma**: En respuesta a [!DNL Salesforce] que retira las versiones 21.0 a 30.0 de la API de plataforma [!DNL Salesforce], el paquete [!DNL Sales Insight] se ha actualizado con las API más recientes.

* **Marca actualizada**: se están actualizando todas las páginas de [!DNL Sales Insight] para alinearlas con la marca de Adobe.

**[!DNL Sales Insight]para[!DNL Microsoft Dynamics]**

* **Diseño de cuenta actualizado**: los vendedores pueden obtener una vista colectiva de las actividades principales, como las siguientes: actividades de correo electrónico, actividades web, momentos interesantes y cambios de puntuación para todos los contactos de una cuenta.

## [!DNL Sales Connect] {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Resultados y motivos de las llamadas**: comprende y rastrea los esfuerzos salientes de tus equipos de ventas con más detalle con opciones nuevas y totalmente personalizables de resultado de llamadas y motivo de llamadas. Además de estos nuevos campos, estamos introduciendo un nuevo control para aplicar el motivo de la llamada y la selección de resultados mientras los vendedores realizan llamadas, un nuevo control para habilitar o deshabilitar los motivos y resultados de la llamada y un nuevo campo personalizado de actividad Razón de la llamada y Resultado de la llamada [!DNL Salesforce] para registrar datos en [!DNL Salesforce]. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para obtener más información.

* **[!DNL Salesforce]Personalización de detalles de actividad**: capture más datos de tareas y actividades de ventas en [!DNL Salesforce] personalizando qué información se agrega al campo de asunto de tarea [!DNL Salesforce] cuando se registra una actividad de ventas en [!DNL Salesforce] desde [!DNL Sales Connect]. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para obtener más información.

## Anuncios {#announcements}

* **Desaprobación de Marketo Sky**: En marzo, Marketo Sky dejará de estar disponible, ya que centramos nuestros recursos en ofrecer la experiencia de usuario de próxima generación. Con el fin de mantener el acceso a una funcionalidad exclusiva de Marketo Sky hoy en día, en marzo incluimos la caducidad de los recursos y la anulación de prioridad de las campañas inteligentes en la experiencia general. [Haga clic aquí](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para obtener más información.

* **Desaprobación de extremos de formularios**: Los formularios de Marketo Engage Forms rechazarán los POST de formulario programáticos no admitidos en el extremo leadCapture/save2. [Haga clic aquí](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para obtener más información.

* **Diálogo para iniciar sesión en el usuario de invitación**: en marzo, la función opcional existente &quot;Iniciar sesión en el cuadro de diálogo para invitar a usuarios&quot; quedará obsoleta. La funcionalidad &quot;[!UICONTROL Iniciar sesión en el cuadro de diálogo de usuario de invitación]&quot; se sobrescribe con la función de identificador universal, que es necesaria para la próxima integración del sistema de Adobe Identity Management y se habilitó en agosto de 2021 en todas las suscripciones. Como resultado de la desuso, Marketo Engage exige que solo se asocie un usuario por dirección de correo electrónico dentro de una suscripción.

**Dominios de Marketo Engage - [!DNL Sales Insight] Configuración**: Para los dominios de Marketo Engage que no tienen certificado SSL aprovisionado y https://, las llamadas fallarán con un error de protocolo de enlace SSL. Por lo tanto, estos dominios van a desaparecer. Como resultado, [!DNL Sales Insight] usuarios con una configuración anterior que señala a cualquiera de estos dominios podrían encontrarse con errores de llamadas del sistema en su página de Posible cliente, Contacto, Cuenta, Paneles de oportunidad o Marketo Global. Le recomendamos que actualice la [configuración de Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) en [!DNL Salesforce] si se encuentra con este error. Solo necesita actualizar las credenciales de Marketo Engage resaltadas en la sección &quot;[!DNL Marketo Sales Insight] Config&quot; del documento.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de enero de 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
