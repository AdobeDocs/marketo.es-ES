---
title: 2022
description: '2022: Documentos de Marketo: documentación del producto'
feature: Release Information
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714id: d0251300-e25f-466f-9856-7e11ce8fa7aaid: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: babcd0bfb6c16165488cabd075a9d75d2952016b
workflow-type: tm+mt
source-wordcount: 4311
ht-degree: 7%

---

# 2022

## Enero de 2022 {#january}

Las siguientes funciones se incluyen en la versión de enero de 2022. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **21 de enero de 2022**, con un despliegue gradual de cada característica en las semanas siguientes (a menos que se especifique lo contrario).

## Experiencia de próxima generación

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

## [!DNL Sales Insight]

![(estrella)](assets/yellow-star.png)

**[!DNL Sales Insight]para [!DNL Salesforce] CRM**

* **Nueva columna de tipo para [!UICONTROL Lo más probable]**: Los vendedores obtendrán perspectivas más rápidas con una nueva columna denominada &quot;Tipo&quot; para diferenciar entre posibles clientes y contactos en la página [!UICONTROL Lo más probable].

* **[!DNL Salesforce]Actualización de la API de plataforma**: En respuesta a [!DNL Salesforce] que retira las versiones 21.0 a 30.0 de la API de plataforma [!DNL Salesforce], el paquete [!DNL Sales Insight] se ha actualizado con las API más recientes.

* **Marca actualizada**: se están actualizando todas las páginas de [!DNL Sales Insight] para alinearlas con la marca de Adobe.

**[!DNL Sales Insight]para[!DNL Microsoft Dynamics]**

* **Diseño de cuenta actualizado**: los vendedores pueden obtener una vista colectiva de las actividades principales, como las siguientes: actividades de correo electrónico, actividades web, momentos interesantes y cambios de puntuación para todos los contactos de una cuenta.

## [!DNL Sales Connect]

![(estrella)](assets/yellow-star.png)

* **Resultados y motivos de las llamadas**: comprende y realiza un seguimiento de los esfuerzos salientes de tus equipos de ventas con más detalle con opciones nuevas y totalmente personalizables de resultado de llamadas y motivo de llamadas. Además de estos nuevos campos, estamos introduciendo un nuevo control para aplicar el motivo de la llamada y la selección de resultados mientras los vendedores realizan llamadas, un nuevo control para habilitar o deshabilitar los motivos y resultados de la llamada y un nuevo campo personalizado de actividad Razón de la llamada y Resultado de la llamada [!DNL Salesforce] para registrar datos en [!DNL Salesforce]. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para obtener más información.

* **[!DNL Salesforce]Personalización de detalles de actividad**: capture más datos de tareas y actividades de ventas en [!DNL Salesforce] personalizando qué información se agrega al campo de asunto de tarea [!DNL Salesforce] cuando se registra una actividad de ventas en [!DNL Salesforce] desde [!DNL Sales Connect]. [Haga clic aquí](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para obtener más información.

## Anuncios

* **Desaprobación de Marketo Sky**: En marzo, Marketo Sky dejará de estar disponible, ya que centramos nuestros recursos en ofrecer la experiencia de usuario de próxima generación. Con el fin de mantener el acceso a una funcionalidad exclusiva de Marketo Sky hoy en día, en marzo incluimos la caducidad de los recursos y la anulación de prioridad de las campañas inteligentes en la experiencia general. [Haga clic aquí](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para obtener más información.

* **Desaprobación de extremos de formularios**: Los formularios de Marketo Engage Forms rechazarán los POST de formulario programáticos no admitidos en el extremo leadCapture/save2. [Haga clic aquí](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para obtener más información.

* **Diálogo para iniciar sesión en el usuario de invitación**: en marzo, la función opcional existente &quot;Iniciar sesión en el cuadro de diálogo para invitar a usuarios&quot; quedará obsoleta. La funcionalidad &quot;[!UICONTROL Iniciar sesión en el cuadro de diálogo de usuario de invitación]&quot; se sobrescribe con la función de identificador universal, que es necesaria para la próxima integración del sistema de Adobe Identity Management y se habilitó en agosto de 2021 en todas las suscripciones. Como resultado de la desuso, Marketo Engage exige que solo se asocie un usuario por dirección de correo electrónico dentro de una suscripción.

**Dominios de Marketo Engage - [!DNL Sales Insight] Configuración**: Para los dominios de Marketo Engage que no tienen certificado SSL aprovisionado y https://, las llamadas fallarán con un error de protocolo de enlace SSL. Por lo tanto, estos dominios van a desaparecer. Como resultado, [!DNL Sales Insight] usuarios con una configuración anterior que señala a cualquiera de estos dominios podrían encontrarse con errores de llamadas del sistema en su página de Posible cliente, Contacto, Cuenta, Paneles de oportunidad o Marketo Global. Le recomendamos que actualice la [configuración de Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) en [!DNL Salesforce] si se encuentra con este error. Solo necesita actualizar las credenciales de Marketo Engage resaltadas en la sección &quot;[!DNL Marketo Sales Insight] Config&quot; del documento.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de enero de 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## Marzo de 2022 {#march}

Las siguientes funciones se incluyen en la versión de marzo de 2022. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **11 de marzo de 2022**, con un despliegue gradual de cada característica en las semanas siguientes (a menos que se especifique lo contrario).

## Orquestación entre canales

* **[!DNL Dynamic Chat]**: Maximice todas las oportunidades en su sitio web al segmentar tanto los posibles clientes como las cuentas con conversaciones proactivas, atractivas y personalizadas 1:1. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permite a los usuarios de Marketo Engage empezar a aprovechar el chat como parte clave de las experiencias integradas en canales múltiples para los casos prácticos de ventas y marketing B2B. Las funciones incluyen: la capacidad de reservar reuniones directamente dentro del chat, enrutamiento de posibles clientes, plantillas de inicio, creación de conversaciones de arrastrar y soltar y mucho más. Dynamic Chat está incluido en todos los paquetes de Marketo Engage y se implementará para todos los usuarios de Marketo Engage este año.

* **Mejora del filtrado de actividades de bots de correo electrónico**: como mejora de la característica [Filtrado de actividades de bots de correo electrónico](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} lanzada anteriormente, ahora puede optar por registrarse en las actividades identificadas como bots. A continuación, puede filtrar y almacenar en déclencheur las acciones basadas en actividades identificadas como realizadas por bots.

## Experiencia de próxima generación

* **Screens actualizado en la experiencia de próxima generación**: Estamos ofreciendo pantallas adicionales actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia:

  * Vista de lista de formularios en [!UICONTROL Design Studio] (incluidas las nuevas acciones masivas)

* **Actualización del flujo de trabajo del programa de importación**: El flujo de trabajo del programa de importación se está entregando en la experiencia de próxima generación con un diseño actualizado y mejoras de uso. Se trata de un cambio automático sin conmutador.

* **Control de administración para el conmutador de alternancia de experiencia de próxima generación**: administre el despliegue de la experiencia de próxima generación de una manera que funcione para los usuarios con la capacidad para que los administradores seleccionen qué tipos de usuarios pueden acceder al conmutador de alternancia.

## Automatización de experiencias

* **Pasos de flujo de autoservicio (Beta)**: expanda la conectividad entre Marketo Engage y el resto de su pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas por lotes y ejecutables, a diferencia de los webhooks, que solo se pueden utilizar en campañas de déclencheur.

* **Caducidad de recursos**: mantenga el control de sus campañas y recursos en los que el tiempo es un factor importante con la capacidad de programar su desactivación automática en una fecha y hora especificadas en la experiencia del usuario de Classic.

* **Anulación de prioridad de campaña inteligente**: Asegúrese de que las campañas inteligentes de déclencheur de alta prioridad se ejecuten lo antes posible con la capacidad de anular la clasificación de prioridad de campaña estándar. Las campañas inteligentes de déclencheur de menor prioridad también se pueden reducir en prioridad para liberar recursos de procesamiento para otras tareas de alta prioridad.

## Mejoras de API

* **Devolver Deshabilitar estado de seguimiento abierto de correos electrónicos**: permite leer el estado de seguimiento abierto de los correos electrónicos a través de la API
* **Recuperar líneas de asunto de contenido dinámico del correo electrónico**: permite a los especialistas en marketing realizar análisis de las líneas de asunto dinámicas en las herramientas de BI
* **Campos personalizados de miembros de programa CRUD**: permite a los especialistas en marketing crear mediante programación campos personalizados de miembros de programa
* **Exportación masiva de objetos personalizados actualizadaEn el filtro**: permite a los especialistas en marketing sincronizar objetos personalizados mediante programación
* **Exponer la configuración de Head Start para programas de correo electrónico**: permite a los especialistas en marketing configurar programas de correo electrónico con Head Start a través de API
* **Actualización selectiva de etiquetas de programa**: permite a los especialistas en marketing insertar actualizaciones selectivas de etiquetas sin insertar todas las etiquetas al mismo tiempo
* **Campo actionResult de extracción masiva de actividades**: permite a los especialistas en marketing identificar qué actividades se omitieron o fallaron

**_Lanzamiento durante todo el trimestre_**

Las siguientes funciones están en un ciclo no trimestral y se lanzarán durante los próximos meses.

## [!DNL Bizible] {#bizible}

![(estrella)](assets/yellow-star.png)

* **Plantillas de BI**: [!DNL Bizible] ahora proporcionará artefactos de informes básicos descargables e informes de muestra para Tableau y Power BI para permitir el desarrollo rápido de informes personalizados adaptados a sus necesidades comerciales específicas.

## [!DNL Sales Connect]

![(estrella)](assets/yellow-star.png)

* **Restricción de conexión de correo electrónico (GA)**: la restricción de conexión de correo electrónico permite a los administradores de [!DNL Sales Connect] configurar la tasa de envío de correos electrónicos al usar Gmail o [!DNL Exchange] como canal de envío, de modo que la tasa a la que se entregan los correos electrónicos al proveedor del canal de envío no supere los límites forzados.

## Anuncios

* **Desaprobación de Marketo Sky**: En marzo, Marketo Sky dejará de estar disponible, ya que centramos nuestros recursos en ofrecer la experiencia de usuario de próxima generación. Con el fin de mantener el acceso a una funcionalidad exclusiva de Marketo Sky hoy en día, hemos incorporado la caducidad de los recursos y la anulación de prioridad de las campañas inteligentes a la experiencia clásica. [Haga clic aquí](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para obtener más información.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de marzo y mayo de 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Mayo de 2022 {#may}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2022. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **6 de mayo de 2022**, con un despliegue gradual de las características restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Integración nativa de CRM {#native-crm-integration}

**[Integración nativa de Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilidad limitada)**: Mejore la participación con los profesionales sanitarios sincronizando la actividad entre Veeva CRM y Marketo Engage mediante la integración nativa. Esta integración permite a los especialistas en marketing crear experiencias multicanal más personalizadas y fluidas para los profesionales sanitarios. Póngase en contacto con el gestor de éxito de los clientes si está interesado en participar.

## Orquestación entre canales

**Eventos de bots de chat para[!DNL Dynamic Chat]**: aprovecha datos de comportamiento más detallados para los visitantes web, como el tiempo que pasan en la página, el tiempo que pasan en el sitio y el porcentaje de desplazamiento por la página para definir cuándo se debe mostrar un cuadro de diálogo de chat.

**Incrustar PDF para[!DNL Dynamic Chat]**: aumente la participación y comparta contenido significativo al incrustar archivos PDF en los cuadros de diálogo de chat y mida el rendimiento del contenido mediante el seguimiento de la actividad de participación.

**Compatibilidad de idioma ampliada para[!DNL Dynamic Chat]**: la interfaz de usuario de [!DNL Dynamic Chat] ahora también estará disponible en francés, alemán, japonés, portugués y español. Los cuadros de diálogo de chat también se pueden configurar en estos idiomas.

**Excluir direcciones URL de[!DNL Dynamic Chat]**: controla cuál de tus páginas web [!DNL Dynamic Chat] aparece en con la capacidad de excluir direcciones URL específicas de los criterios de segmentación.

**[Mejoras en el filtrado de actividad de bots de correo electrónico](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: siga protegiendo el estado de la base de datos con la capacidad de identificar el comportamiento de bots en función de los agentes de usuario o las direcciones IP de vínculo oculto y los patrones de proximidad, además de la identificación de coincidencia de lista IAB existente. Vea las estadísticas de actividad de bots que le permiten comprender la cantidad de actividades de bots identificadas para cada tipo.

**[Encabezado STS para vínculos de seguimiento de correo electrónico](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: cumpla las prácticas recomendadas de seguridad con la capacidad de aplicar encabezados de seguridad de transporte seguro para garantizar que el tráfico a los vínculos rastreados siempre sea seguro.

## Experiencia de próxima generación

**Cambio de alternancia predeterminado a la experiencia de próxima generación**: el interruptor de alternancia estará predeterminado a la nueva experiencia en todas las pantallas donde esté disponible, lo que facilita a los usuarios descubrir los diseños actualizados y las mejoras de uso.

**Pantalla actualizada en la experiencia de próxima generación**:

En [!UICONTROL Design Studio] proporcionaremos una vista de detalles de las plantillas de correo electrónico en la experiencia de próxima generación, con lo que ofreceremos un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia.

## Automatización de experiencias

**Pasos de flujo de autoservicio (versión beta continuada)**: expanda la conectividad entre Marketo Engage y el resto de su pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de déclencheur, por lotes y ejecutables (a diferencia de los webhooks que solo se pueden utilizar en campañas de déclencheur).

## Mejoras de API

* **Acceso ampliado a la API para suscripciones habilitadas para CRM**: Estamos ampliando el acceso a la API para suscripciones que tienen habilitada una sincronización de CRM para permitir que los usuarios recuperen Compañías, Oportunidades y Vendedores de Marketo Engage.
* **Compatibilidad con tipos de datos &quot;ocultos&quot; en Forms**: proporciona la capacidad de administrar campos de formulario ocultos mediante API.
* **Admitir valores de comparación múltiple para isNot Form mediante reglas**: administre la visibilidad de los campos de formulario en función de si el valor de otro campo no es uno de los valores de una lista determinada.
* **Permitir la configuración de valores para mostrar y enviados en listas seleccionadas por separado**: establezca el valor para mostrar y el valor enviado en un campo por separado. Por ejemplo, mostrar el nombre de un hotel, pero enviar un ID interno al servidor.
* **Permitir la configuración de Deshabilitar el seguimiento de aperturas al crear o actualizar correo electrónico**: cree un correo electrónico con el seguimiento de aperturas deshabilitado.

## Anuncios

**Verificación y unicidad de correo electrónico**: a partir de abril, comenzará el despliegue de la verificación por correo electrónico. En este punto, las direcciones de correo electrónico de los usuarios de Marketo Engage requerirán verificación y unicidad (esto no se aplica a los usuarios solo de API). Los usuarios autenticados del servicio de directorio verán automáticamente sus correos electrónicos verificados cuando su suscripción esté habilitada con la verificación por correo electrónico.

La verificación por correo electrónico de las suscripciones que usan la función &quot;[!UICONTROL Iniciar sesión en el cuadro de diálogo de usuario de invitación]&quot; o que tienen un solo correo electrónico asociado a varios usuarios coincidirá con la versión de mayo. Las suscripciones que tengan un solo correo electrónico asociado a varios usuarios se habilitarán con la verificación por correo electrónico y requerirán que dichos usuarios resuelvan el conflicto y utilicen un correo electrónico único por usuario. Cuando la función &quot;Iniciar sesión en el cuadro de diálogo de invitar al usuario&quot; está habilitada, los usuarios invitados a través de esta función deberán tener una dirección de correo electrónico única. Para usuarios solo de API invitados mediante esta función, no es necesario que la dirección de correo electrónico sea única.

**Cambio de comportamiento de carpeta de archivo**: con esta versión, la capacidad de crear nuevos recursos en carpetas de archivo ya no estará disponible en los menús contextuales de árbol. Las opciones de menú para crear nuevos recursos se ocultarán para todos los recursos. [Obtenga más información aquí](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de marzo y mayo de 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Junio de 2022 {#june}

A continuación encontrará todas las funciones incluidas en la versión de junio de 2022. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

Las siguientes características comenzarán a lanzarse el **24 de junio de 2022**, con un despliegue gradual de las características restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Entorno de datos de marketing

* **Exponer campos CreatedAt/UpdatedAt para objetos personalizados**: Permite inspeccionar estos campos en la pantalla Detalles de persona para obtener insight adicional.

## Orquestación entre canales

* **Uso mejorado de Stream Designer para[!DNL Dynamic Chat]**: agrega tarjetas directamente desde el lienzo de Stream Designer sin necesidad de arrastrarlas y soltarlas. La interfaz [!DNL Dynamic Chat] también se ha mejorado para ofrecer una mejor visibilidad del contenido en tarjetas individuales.

* **Reglas de enrutamiento de citas avanzadas para[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] ofrece más opciones para el enrutamiento de citas de destino. Especifique las citas de los agentes que deben enrutarse según los atributos de Marketo Engage, asegurándose de que los posibles clientes se dirijan a los agentes correspondientes.

* **Informes de diálogo avanzados para[!DNL Dynamic Chat]**: vea el rendimiento de sus campañas de [!DNL Dynamic Chat] con mayor detalle mediante las nuevas visualizaciones de datos para las métricas de participación y conversión.

* **Desincronizar atributos de Marketo Engage no utilizados para[!DNL Dynamic Chat]**: desincronice los atributos de Marketo Engage de su suscripción a [!DNL Dynamic Chat] que no se usen, lo que le ayudará a facilitar la limpieza de los datos y permitirá que se sincronicen atributos alternativos según sea necesario.

## Experiencia de última generación

**Nuevas vistas de conmutador de alternancia**: Las vistas siguientes ya están disponibles en la experiencia de próxima generación:

* [Vista de detalles del correo electrónico](https://experienceleague.adobe.com/es/docs/marketo/using/home){target="_blank"}
* [Vista de lista del correo electrónico](https://experienceleague.adobe.com/es/docs/marketo/using/home){target="_blank"}

## Automatización de experiencias

* **Exclusiones de reglas de validación de campos de formulario globales**: excluya formularios específicos de las reglas de validación de formularios globales para que los centros de suscripción y otros flujos de trabajo críticos para la empresa puedan aceptar todos los valores.

* **Pasos de flujo de autoservicio**: expanda la conectividad entre Marketo Engage y el resto de su pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de Déclencheur, por lotes y ejecutables, a diferencia de los webhooks, que solo se pueden utilizar en campañas de Déclencheur.

* **Seguimiento de vínculos no basados en protocolos Munchkin**: amplíe la compatibilidad con el seguimiento de vínculos `tel` y `mailto` con Munchkin para realizar el seguimiento de un conjunto ampliado de comportamientos web.

* **Métodos HTTP adicionales para los webhooks**: especifique PUT, PATCH y DELETE como tipos de solicitud para interactuar con los servicios web.

## [!DNL Sales Insight]

![(estrella)](assets/yellow-star.png)

* Conjunto de permisos de **[!DNL Sales Insight]en[!DNL Salesforce]**: los administradores pueden proporcionar acceso de [!DNL Sales Insight] a un conjunto limitado de personas a nivel de usuario en lugar de a nivel de perfil mediante el conjunto de permisos de la aplicación de Marketo, que forma parte del paquete de [!DNL Sales Insight] [!DNL Salesforce].

* **Actualización del mosaico de Mi Marketo - [!DNL Sales Insight] Acciones**: Los administradores de Marketo (y los usuarios que designen) ahora pueden navegar rápidamente a su instancia de Acciones [!DNL Sales Insight] a través de un nuevo mosaico de Acciones [!DNL Sales Insight] ubicado en la página Mi Marketo.

## [!DNL Sales Connect]

![(estrella)](assets/yellow-star.png)

* **[!DNL Salesforce]Actualización de API**: Con la versión del verano de 2022, las versiones heredadas de API 21 -30 ya no serán compatibles con [!DNL Salesforce]. [!DNL Salesforce]Con esta versión de Marketo Engage, todas las [!DNL Sales Connect] solicitudes que utilizan versiones de API heredadas se han actualizado para permanecer dentro de una versión admitida. Para obtener detalles completos sobre [!DNL Salesforce] planes de retiro de API, haga clic [aquí](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Mejoras de API

* **Nuevas capacidades de filtrado para la API de extracción masiva de miembros del programa**: filtre por estado de pertenencia al programa, actualización, cadencia o contenido agotado para restringir el conjunto de datos extraídos.

* **Mejora de la API de extracción de miembros de programas en lotes**: especifique hasta 10 programas durante la creación del trabajo para mejorar el rendimiento.

## Anuncios

* **Desaprobación de Forms: Forms 1.0, extremo de captura/guardado de posibles clientes y versiones sin script de formularios**: La compatibilidad con los recursos de Forms 1.0 se eliminará completamente de Marketo Engage en octubre de 2022. Todos los recursos existentes de Forms 1.0 dejarán de funcionar. Los formularios Marketo Engage requerirán que JavaScript se cargue en páginas de aterrizaje y sitios web.

**_Seminario web sobre la versión del producto_**

[Seminario web de junio y agosto de 2022 sobre la versión de Marketo Engage](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Agosto de 2022 {#august}

A continuación encontrará todas las funciones incluidas en la versión de agosto de 2022. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

Las siguientes características comenzaron un despliegue gradual el **26 de agosto de 2022**.

## Orquestación entre canales

* Habilitar/deshabilitar todos los cuadros de diálogo publicados a la vez para [!DNL Dynamic Chat]**: habilita/deshabilita globalmente todos los cuadros de diálogo publicados a la vez desde la página Configuración con solo presionar un botón.

* **Avatares personalizados para[!DNL Dynamic Chat]**: carga un avatar de bot de chat personalizado para que se pueda personalizar a tu marca.

* **Transcripciones de chat de[!DNL Dynamic Chat]**: vea las transcripciones de chat de cada conversación para obtener información más detallada en insight sobre lo que le interesa a cada visitante web.

## Experiencia de última generación

* **Marca Adobe**: aspecto actualizado para la página de detalles de editores y personas con la nueva marca Adobe Experience Cloud.

* **Mostrar la jerarquía de carpetas de la carpeta de destino en el cuadro de diálogo Mover**: al ver la jerarquía de carpetas de cada carpeta, es más fácil mover recursos y se reduce la probabilidad de ponerlos en la carpeta incorrecta.

* **[Actualización de Screens en la experiencia de próxima generación](https://experienceleague.adobe.com/es/docs/marketo/using/home){target="_blank"}**: Estamos ofreciendo pantallas adicionales actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia:

  * Detalles del fragmento
  * Detalles de &quot;Imágenes y archivos&quot;

>[!NOTE]
>
>La excepción consiste en mover un recurso a una carpeta dentro de un programa en Actividades de marketing. Esta acción de mover no mostrará la jerarquía de carpetas, ya que las carpetas de un programa no pueden tener nombres duplicados.

## Automatización de experiencias

* **[Pasos de flujo de autoservicio - Mejoras en la importación de programas](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**: compatibilidad mejorada para importar programas con pasos de flujo personalizados en los que ahora puede utilizar varias instancias del mismo proveedor de servicios e importar programas que tengan pasos de flujo compatibles con esos proveedores de servicios.

* **[!DNL Munchkin]- Seguimiento de vínculos expandido**: amplíe la compatibilidad con el seguimiento de vínculos `tel` y `mailto` con Munchkin para realizar el seguimiento de un conjunto ampliado de comportamientos web.

* **Visibilidad personalizada de encabezados de webhook**: los encabezados personalizados de webhook ahora se muestran en la pestaña [!UICONTROL Administración] > [!UICONTROL Webhooks] para obtener una mejor visibilidad.

* **CAPTCHA**: evalúe la validez de los envíos de formularios [usando reCAPTCHA v3](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} para puntuar el tráfico entrante de los formularios. Cree flujos de trabajo de marketing para excluir, poner en cuarentena o eliminar automáticamente el tráfico de bots sospechoso.

* **Permiso para aprobar el formulario**: nuevo permiso para controlar qué diseñadores pueden aprobar cambios en un formulario en línea con otros recursos de [!UICONTROL Design Studio]. Esto evita que otros diseñadores inserten cambios en los formularios sin que otra persona con permiso de aprobación lo revise.

* **Reproducir siempre la campaña después de una combinación anónima**: la combinación anónima de posibles clientes se produce antes de la reproducción de la campaña, por lo que los filtros de campo personalizados se comportan de forma fiable cuando se realiza una reproducción anónima de la campaña.

## Entorno de datos de marketing

* **Corregir el truncamiento de la interfaz de usuario de los campos de objeto personalizado &quot;[!UICONTROL Utilizado por]&quot;**: ahora es más fácil identificar los campos de objeto personalizados que están &quot;en uso&quot; para que pueda eliminar campos de un objeto personalizado cuando sea necesario.

## Mejoras de API

* **Nuevas capacidades de filtrado para la API de extracción masiva de miembros del programa**: filtre por estado de pertenencia a programa, updatedAt, cadencia o contenido agotado para restringir el conjunto de datos extraídos.

## [!DNL Sales Insight]

![(estrella)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Integración con [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**: vea las actividades de [!DNL Dynamic Chat] en el panel [!DNL Sales Insight] y aproveche este nuevo punto de datos en su esfuerzo de prospección.

## Anuncios

**_Seminario web sobre la versión del producto_**

[Seminario web de junio y agosto de 2022 sobre la versión de Marketo Engage](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Octubre de 2022 {#october}

A continuación encontrará todas las funciones incluidas en la versión de octubre de 2022. Compruebe la disponibilidad de las funciones en su edición de Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Las funciones indicadas con una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

## Funciones del ciclo de lanzamiento estándar {#standard-release-cycle-features}

Las siguientes características están dentro del ciclo de lanzamiento estándar y comenzaron a lanzarse el **sábado, 14 de octubre de 2022**, con un despliegue gradual de las características restantes en las semanas siguientes. Las funciones y fechas del lanzamiento están sujetas a cambios. Compruebe el estado de cada una de las funciones.

### Entorno de datos de marketing

</br>

* **Sincronización de campos personalizados de miembros del programa**: capacidad de sincronizar bidireccionalmente los campos ampliables capturados para un miembro del programa (por ejemplo, las preferencias de los asistentes durante el registro del evento, como comida, sesiones, pistas, etc.) con campos de miembros de Campaign en Salesforce.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Sincronización de campo personalizado para miembros del programa</a></td>
  </tr>
  </tbody>
</table>

* **Integración de Adobe Privacy Service**: Armonícese con Privacy Service para automatizar el cumplimiento de las regulaciones de privacidad de datos en los productos de Experience Cloud. Actualmente, este servicio solo está disponible para los clientes de Marketo Engage que han incorporado el sistema Identity Management de Adobe.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Experiencia de última generación

</br>

* **Screens actualizado en la experiencia de próxima generación**: Estamos ofreciendo pantallas adicionales actualizadas en la experiencia de próxima generación que ofrecen un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia:

  * Detalles de plantilla de la página de destino
  * Lista de plantilla del correo electrónico

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="https://experienceleague.adobe.com/es/docs/marketo/using/home">Conmutador de alternancia</a></td>
  </tr>
  </tbody>
</table>

* **Mejorado usado por la pestaña en Detalles de plantilla de correo electrónico**: en la nueva experiencia, verá información adicional relacionada con los recursos que usan la plantilla de correo electrónico, incluidos el estado del recurso, la última modificación y la última modificación de. También puede buscar, ordenar y filtrar la lista de recursos utilizados por los recursos.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

* **Modelos de filtro de recursos de informe**: nuevo diseño para los modelos de configuración de informe que muestran un nuevo árbol de recursos en el menú de configuración y un filtro para Fecha de creación y modificación.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

### Mejoras de API

</br>

* **Importación masiva de posibles clientes: asociación de vendedores**: paridad con la API de REST de posibles clientes para poder asociar posibles clientes con vendedores durante el proceso de importación masiva de posibles clientes, lo que reduce la complejidad y el número de llamadas de API necesarias.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importación masiva de posibles clientes</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight

</br>

![(estrella)](assets/yellow-star.png)

* **Integración de Sales Insight con Dynamic Chat**: el panel de información ahora incluye actividades de Dynamic Chat en la cuadrícula inteligente junto con un resumen semanal y tarjetas de detalles.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integración de Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Funciones de versión de Agile

Las siguientes funciones siguen un formato Agile y se lanzan en varias fechas antes o después de la fecha de lanzamiento estándar. Compruebe el estado de cada una de las funciones.

* **Organizar automáticamente los flujos de diálogo para Dynamic Chat**: mejora tu lienzo de diálogo lleno organizando todo en el lienzo en un formato limpio y fácil de leer con solo pulsar un botón a través de Organizar automáticamente.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Iconos de Stream Designer</a></td>
  </tr>
  </tbody>
</table>

* **Vínculos de reunión para Dynamic Chat**: Opción para incluir automáticamente un vínculo de equipos o de reunión para Google y Outlook en cada invitación de calendario enviada a los visitantes.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendario</a></td>
  </tr>
  </tbody>
</table>

* **Admitir tipos de datos adicionales para Dynamic Chat**: Los tres nuevos tipos de datos (booleano, entero, flotante) le permiten aprovechar más campos de Marketo Engage existentes en Dynamic Chat para tareas como segmentar según puntuaciones o hacer preguntas de sí/no a los visitantes.

<table>
  <tr>
   <td><b>Estado</b></td>
   <td><b>Actualizaciones de la documentación</b></td>
  </tr>
  <tr>
   <td>Publicado</td>
   <td>n/a</td>
  </tr>
  </tbody>
</table>

## Anuncios

* **Forms 1.0**: la versión de Forms 1.0 quedará obsoleta y se completará con la versión de octubre. Los recursos de Forms 1.0 ya no podrán enviar datos a Marketo Engage y devolverán los errores si se intenta hacerlo.

* **Forms sin script**: Forms dejará de funcionar cuando Javascript esté deshabilitado en el explorador. El envío de formularios requerirá que esté habilitado Javascript.
