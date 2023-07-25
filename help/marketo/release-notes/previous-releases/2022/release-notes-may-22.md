---
description: 'Notas de la versión, mayo de 2022: Documentos de Marketo: documentación del producto'
title: Notas de la versión, mayo de 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Notas de la versión: mayo de 2022 {#release-notes-may-22}

A continuación encontrará todas las funciones incluidas en la versión de mayo de 2022. Compruebe la disponibilidad de las funciones en Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Características indicadas por una estrella (![estrella](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones comenzarán a lanzarse el **6 de mayo de 2022**, con un despliegue gradual de las funciones restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Integración nativa de CRM {#native-crm-integration}

**[Integración nativa de Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilidad limitada)**: Mejore la participación con los profesionales sanitarios sincronizando la actividad entre Veeva CRM y el Marketo Engage a través de la integración nativa. Esta integración permite a los especialistas en marketing crear experiencias multicanal más personalizadas y fluidas para los profesionales sanitarios. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) si está interesado en participar.

## Orquestación entre canales {#cross-channel-orchestration}

**Eventos de bots de chat para Dynamic Chat**: Aproveche datos de comportamiento más detallados para los visitantes web, como el tiempo en la página, el tiempo en el sitio y el porcentaje de desplazamiento de la página para definir cuándo se debe mostrar un cuadro de diálogo de chat.

**Incrustar PDF para Dynamic Chat**: aumente la participación y comparta contenido significativo incrustando PDF en los cuadros de diálogo de chat y mida el rendimiento del contenido mediante el seguimiento de la actividad de participación.

**Compatibilidad de idioma extendida para Dynamic Chat**: la interfaz de usuario de Dynamic Chat ahora también está disponible en francés, alemán, japonés, portugués y español. Los cuadros de diálogo de chat también se pueden configurar en estos idiomas.

**Excluir direcciones URL del Dynamic Chat**: controle cuál de los Dynamic Chat de las páginas web aparece en con la capacidad de excluir direcciones URL específicas de los criterios de segmentación.

**[Mejoras en el filtrado de actividades de bots de correo electrónico](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: siga protegiendo el estado de la base de datos con la capacidad de identificar el comportamiento de bots en función de agentes de usuario o direcciones IP de vínculo oculto y patrones de proximidad, además de la identificación de coincidencias de lista IAB existente. Vea las estadísticas de actividad de bots que le permiten comprender la cantidad de actividades de bots identificadas para cada tipo.

**[Encabezado STS para vínculos de seguimiento de correo electrónico](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: cumpla las prácticas recomendadas de seguridad con la capacidad de aplicar encabezados de seguridad de transporte seguro para garantizar que el tráfico a los vínculos rastreados siempre sea seguro.

## Experiencia de próxima generación {#modern-ux}

**Cambiar de forma predeterminada a la experiencia de próxima generación**: el conmutador estará predeterminado en la nueva experiencia en todas las pantallas donde esté disponible, lo que facilita a los usuarios descubrir los diseños actualizados y las mejoras de uso.

**Pantalla actualizada en la experiencia de próxima generación**:

En Design Studio proporcionamos una vista de detalles de plantillas de correo electrónico en la experiencia de próxima generación, con mejoras actualizadas de diseño y facilidad de uso accesibles mediante el conmutador de alternancia.

## Automatización de experiencias {#experience-automation}

**Pasos del flujo de autoservicio (versión beta continuada)**: Amplíe la conectividad entre Marketo Engage y el resto de la pila con la capacidad de crear pasos de flujo personalizados para utilizarlos en campañas inteligentes. Tanto los usuarios como los socios de Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de déclencheur, por lotes y ejecutables (a diferencia de los webhooks que solo se pueden utilizar en campañas de déclencheur).

## Mejoras de API {#api-enhancements}

* **Acceso a API ampliado para suscripciones habilitadas para CRM**: Estamos expandiendo el acceso a la API para suscripciones que tienen una sincronización CRM habilitada para permitir que los usuarios recuperen Compañías, Oportunidades y Personas de ventas de Marketo Engage.
* **Compatibilidad con tipos de datos &quot;ocultos&quot; en Forms**: Proporciona la capacidad de administrar campos de formulario ocultos mediante API.
* **Compatibilidad con varios valores de comparación para isNot Form mediante reglas**: administre la visibilidad de los campos de formulario en función de si el valor de otro campo no es uno de los valores de una lista determinada.
* **Permitir la configuración de Mostrar y Enviar valores en Seleccionar listas por separado**: establezca por separado el valor de visualización y el valor enviado en un campo. Por ejemplo, mostrar el nombre de un hotel, pero enviar un ID interno al servidor.
* **Permitir la configuración de Deshabilitar el seguimiento de aperturas al crear o actualizar correo electrónico**: cree un correo electrónico con el seguimiento de aperturas deshabilitado.

## Anuncios {#announcements}

**Verificación y unicidad del correo electrónico**: A partir de abril, comenzará el despliegue de la verificación por correo electrónico. En este punto, las direcciones de correo electrónico de los usuarios Marketo Engage requerirán verificación y unicidad (esto no se aplica a los usuarios solo de API). Los usuarios autenticados del servicio de directorio verán automáticamente sus correos electrónicos verificados cuando su suscripción esté habilitada con la verificación por correo electrónico.

La verificación por correo electrónico de las suscripciones que utilizan la función &quot;Iniciar sesión en el cuadro de diálogo de usuario de invitación&quot; o que tienen un solo correo electrónico asociado a varios usuarios coincidirá con la versión de mayo. Las suscripciones que tengan un solo correo electrónico asociado a varios usuarios se habilitarán con la verificación por correo electrónico y requerirán que dichos usuarios resuelvan el conflicto y utilicen un correo electrónico único por usuario. Cuando la función &quot;Iniciar sesión en el cuadro de diálogo de invitar al usuario&quot; está habilitada, los usuarios invitados a través de esta función deberán tener una dirección de correo electrónico única. Para usuarios solo de API invitados mediante esta función, no es necesario que la dirección de correo electrónico sea única.

**Archivar cambio de comportamiento de carpeta**: Con esta versión, la capacidad de crear nuevos recursos en carpetas de archivo ya no estará disponible en los tres menús contextuales. Las opciones de menú para crear nuevos recursos se ocultarán para todos los recursos. [Obtenga más información aquí](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Seminario web sobre lanzamiento de productos_**

[Seminario web de marzo y mayo de 2022 sobre la versión para Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
