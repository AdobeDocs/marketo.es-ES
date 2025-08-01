---
description: 'Notas de la versión, mayo de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, mayo de 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Notas de la versión: mayo de 2022 {#release-notes-may-22}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Las funciones indicadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con su representante de Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes características comenzarán a lanzarse el **6 de mayo de 2022**, con un despliegue gradual de las características restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Integración nativa de CRM {#native-crm-integration}

**[Integración nativa de Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilidad limitada)**: Mejore la participación con los profesionales sanitarios sincronizando la actividad entre Veeva CRM y Marketo Engage mediante la integración nativa. Esta integración permite a los especialistas en marketing crear experiencias multicanal más personalizadas y fluidas para los profesionales sanitarios. Póngase en contacto con el administrador de satisfacción del cliente si está interesado en participar.

## Orquestación entre canales {#cross-channel-orchestration}

**Eventos de bots de chat para[!DNL Dynamic Chat]**: aprovecha datos de comportamiento más detallados para los visitantes web, como el tiempo que pasan en la página, el tiempo que pasan en el sitio y el porcentaje de desplazamiento por la página para definir cuándo se debe mostrar un cuadro de diálogo de chat.

**Incrustar PDF para[!DNL Dynamic Chat]**: aumente la participación y comparta contenido significativo al incrustar archivos PDF en los cuadros de diálogo de chat y mida el rendimiento del contenido mediante el seguimiento de la actividad de participación.

**Compatibilidad de idioma ampliada para[!DNL Dynamic Chat]**: la interfaz de usuario de [!DNL Dynamic Chat] ahora también estará disponible en francés, alemán, japonés, portugués y español. Los cuadros de diálogo de chat también se pueden configurar en estos idiomas.

**Excluir direcciones URL de[!DNL Dynamic Chat]**: controla cuál de tus páginas web [!DNL Dynamic Chat] aparece en con la capacidad de excluir direcciones URL específicas de los criterios de segmentación.

**[Mejoras en el filtrado de actividad de bots de correo electrónico](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: siga protegiendo el estado de la base de datos con la capacidad de identificar el comportamiento de bots en función de los agentes de usuario o las direcciones IP de vínculo oculto y los patrones de proximidad, además de la identificación de coincidencia de lista IAB existente. Vea las estadísticas de actividad de bots que le permiten comprender la cantidad de actividades de bots identificadas para cada tipo.

**[Encabezado STS para vínculos de seguimiento de correo electrónico](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: cumpla las prácticas recomendadas de seguridad con la capacidad de aplicar encabezados de seguridad de transporte seguro para garantizar que el tráfico a los vínculos rastreados siempre sea seguro.

## Experiencia de próxima generación {#modern-ux}

**Cambio de alternancia predeterminado a la experiencia de próxima generación**: el interruptor de alternancia estará predeterminado a la nueva experiencia en todas las pantallas donde esté disponible, lo que facilita a los usuarios descubrir los diseños actualizados y las mejoras de uso.

**Pantalla actualizada en la experiencia de próxima generación**:

En [!UICONTROL Design Studio], la experiencia de próxima generación, ofreceremos una vista de detalles de las plantillas de correo electrónico con un diseño actualizado y mejoras de uso accesibles mediante el conmutador de alternancia.

## Automatización de experiencias {#experience-automation}

**Pasos de flujo de autoservicio (versión beta continuada)**: expanda la conectividad entre Marketo Engage y el resto de su pila con la capacidad de crear pasos de flujo personalizados para usarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de déclencheur, por lotes y ejecutables (a diferencia de los webhooks que solo se pueden utilizar en campañas de déclencheur).

## Mejoras de API {#api-enhancements}

* **Acceso ampliado a la API para suscripciones habilitadas para CRM**: Estamos ampliando el acceso a la API para suscripciones que tienen habilitada una sincronización de CRM para permitir que los usuarios recuperen Compañías, Oportunidades y Vendedores de Marketo Engage.
* **Compatibilidad con tipos de datos &quot;ocultos&quot; en Forms**: proporciona la capacidad de administrar campos de formulario ocultos mediante API.
* **Admitir valores de comparación múltiple para isNot Form mediante reglas**: administre la visibilidad de los campos de formulario en función de si el valor de otro campo no es uno de los valores de una lista determinada.
* **Permitir la configuración de valores para mostrar y enviados en listas seleccionadas por separado**: establezca el valor para mostrar y el valor enviado en un campo por separado. Por ejemplo, mostrar el nombre de un hotel, pero enviar un ID interno al servidor.
* **Permitir la configuración de Deshabilitar el seguimiento de aperturas al crear o actualizar correo electrónico**: cree un correo electrónico con el seguimiento de aperturas deshabilitado.

## Anuncios {#announcements}

**Verificación y unicidad de correo electrónico**: a partir de abril, comenzará el despliegue de la verificación por correo electrónico. En este punto, las direcciones de correo electrónico de los usuarios de Marketo Engage requerirán verificación y unicidad (esto no se aplica a los usuarios solo de API). Los usuarios autenticados del servicio de directorio verán automáticamente sus correos electrónicos verificados cuando su suscripción esté habilitada con la verificación por correo electrónico.

La verificación por correo electrónico de las suscripciones que usan la función &quot;[!UICONTROL Iniciar sesión en el cuadro de diálogo de usuario de invitación]&quot; o que tienen un solo correo electrónico asociado a varios usuarios coincidirá con la versión de mayo. Las suscripciones que tengan un solo correo electrónico asociado a varios usuarios se habilitarán con la verificación por correo electrónico y requerirán que dichos usuarios resuelvan el conflicto y utilicen un correo electrónico único por usuario. Cuando la función &quot;Iniciar sesión en el cuadro de diálogo de invitar al usuario&quot; está activada, los usuarios invitados a través de esta función deberán tener una dirección de correo electrónico única. Para usuarios solo de API invitados mediante esta función, no es necesario que la dirección de correo electrónico sea única.

**Cambio de comportamiento de carpeta de archivo**: con esta versión, la capacidad de crear nuevos recursos en carpetas de archivo ya no estará disponible en los menús contextuales de árbol. Las opciones de menú para crear nuevos recursos se ocultarán para todos los recursos. [Obtenga más información aquí](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Seminario web sobre la versión del producto_**

[Seminario web sobre la versión de Marketo Engage de marzo y mayo de 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
