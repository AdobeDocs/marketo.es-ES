---
description: 'Notas de la versión, enero de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# Notas de la versión: enero de 2022 {#release-notes-jan-22}

Las siguientes funciones se incluyen en la versión de enero de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **21 de enero de 2022**, con un despliegue gradual de cada característica en las semanas siguientes (a menos que se especifique lo contrario).

## Experiencia de próxima generación {#modern-ux}

* **Screens actualizado en la experiencia de próxima generación**: Estamos ofreciendo pantallas adicionales actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia:

   * Detalles del recurso de la página de aterrizaje en Design Studio
   * Detalles del recurso de la página de aterrizaje en actividades de marketing

## Integración con Microsoft Dynamics {#microsoft-dynamics-integration}

* **Sincronización del tipo de campo del conjunto de opciones de selección múltiple disponible de forma general**: sincronice el tipo de campo del conjunto de opciones de selección múltiple de Microsoft Dynamics para aprovecharlo en las listas inteligentes y las campañas inteligentes y así poder segmentar la audiencia de forma más granular. Algunos ejemplos son: temas/productos de interés, modos de comunicación preferidos y mucho más. Esta nueva sincronización está disponible para Microsoft Dynamics versión 9.X (incluida Dynamics 365 Online).

* **Autenticación de servidor a servidor para Microsoft Dynamics 365 Online**: para aumentar la seguridad, ahora se admitirá Servidor a servidor (S2S) como un modo adicional de autenticación para el usuario de sincronización de Marketo Engage en Azure Active Directory para el acceso no interactivo a Microsoft Dynamics 365 Online. Esto le permite emplear la autenticación de varios factores, ya que toda la autenticación y los inicios de sesión se basarán en OAuth (solo ID de cliente y secreto de cliente).

>[!NOTE]
>
>El modo S2S se basa en el usuario de la aplicación en lugar de en el usuario con licencia, lo que evita el uso de una licencia adicional.

## Administración {#administration}

* **[Reglas de validación de formularios](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: mantenga el estado de la base de datos con la capacidad de bloquear los dominios de correo electrónico problemáticos o no deseados para que no envíen formularios de Marketo Engage. El panel Regla de validación de formulario global permite a los administradores definir una lista de bloqueados o habilitar una lista predefinida de dominios de consumidores libres para bloquear formularios.

* **[Seguridad de encabezado de página de aterrizaje](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: los administradores pueden administrar encabezados de seguridad de transporte estricta y opciones X-Frame en los dominios de su página de aterrizaje para aplicar requisitos de seguridad estrictos.

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## Conector de destino del Marketo Engage de AEP: crear posibles clientes nuevos {#aep-marketo-engage-destination-connector}

Los clientes de Marketo Engage que también utilizan Adobe Experience Platform (AEP) pueden maximizar su base de datos con la capacidad de insertar nuevos registros de persona netos en Marketo Engage desde AEP a través del conector de destino de AEP. Al enviar segmentos de audiencia de AEP al Marketo Engage, se pueden agregar automáticamente a él las personas del segmento que no existan en la base de datos del Marketo Engage [1.](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)

## Sales Insight {#sales-insight}

![(estrella)](assets/yellow-star.png)

**Perspectiva de ventas para Salesforce CRM**

* **Nueva columna de tipo para los resultados más probables**: Los vendedores obtendrán perspectivas más rápidas con una nueva columna denominada &quot;Tipo&quot; para diferenciar entre posibles clientes y contactos en la página Resultados más probables.

* **Actualización de la API de Salesforce Platform**: En respuesta a que Salesforce se retira de las versiones 21.0 a 30.0 de la API de Salesforce Platform, el paquete de Perspectiva de ventas se ha actualizado con las API más recientes.

* **Marca actualizada**: todas las páginas de perspectiva de ventas se están actualizando para alinearse con la marca de Adobe.

**Perspectiva de ventas para Microsoft Dynamics**

* **Diseño de cuenta actualizado**: los vendedores pueden obtener una vista colectiva de las actividades principales, como las siguientes: actividades de correo electrónico, actividades web, momentos interesantes y cambios de puntuación para todos los contactos de una cuenta.

## Sales Connect {#sales-connect}

![(estrella)](assets/yellow-star.png)

* **Resultados y motivos de las llamadas**: comprende y realiza un seguimiento de los esfuerzos salientes de tus equipos de ventas con más detalle con opciones nuevas y totalmente personalizables de resultado de llamadas y motivo de llamadas. Además de estos nuevos campos, estamos introduciendo un nuevo gobierno para aplicar el motivo de la llamada y la selección de resultados mientras los vendedores realizan llamadas, un nuevo gobierno para habilitar o deshabilitar los motivos y resultados de la llamada y un nuevo campo personalizado Razón de la llamada y Actividad de Salesforce de salida de la llamada para registrar datos en Salesforce. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para obtener más información.

* **Personalización de detalles de actividad de Salesforce**: capture más datos de tareas y actividades de ventas en Salesforce al personalizar qué información se agrega al campo de asunto de tarea de Salesforce cuando se registra una actividad de ventas en Salesforce desde Sales Connect. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para obtener más información.

## Anuncios {#announcements}

* **Desaprobación del Marketo Sky**: En marzo, Marketo Sky ya no estará disponible porque centramos nuestros recursos en ofrecer la experiencia del usuario de próxima generación. Con el fin de mantener el acceso a una funcionalidad que hoy en día es exclusiva de Marketo Sky, en marzo incluimos la caducidad de los recursos y la anulación de prioridad de las campañas inteligentes en la experiencia general. [Haga clic aquí](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para obtener más información.

* **Desaprobación de extremos de formularios**: Los formularios de Marketo Engage rechazarán los POST de formulario programáticos no admitidos en el extremo leadCapture/save2. [Haga clic aquí](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para obtener más información.

**Dominios de Marketo Engage - Configuración de perspectivas de ventas**: Para los dominios de Marketo Engage que no tienen certificado SSL aprovisionado y https://, las llamadas fallarán con un error de protocolo de enlace SSL. Por lo tanto, estos dominios van a desaparecer. Como resultado, los usuarios de Sales Insight con una configuración anterior que señala a cualquiera de estos dominios pueden encontrarse con errores de llamadas del sistema en su página de cliente potencial, contacto, cuenta, paneles de oportunidad o Marketo Global. Le recomendamos que actualice la [configuración del Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) en Salesforce si se encuentra con este error. Solo es necesario actualizar las credenciales del Marketo Engage resaltadas en la sección &quot;Configuración de Marketo Sales Insight&quot; del documento.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de enero de 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
