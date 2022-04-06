---
description: Notas de la versión actuales - Documentos de Marketo - Documentación del producto
title: Notas de la versión actual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Notas de la versión: Mayo de 2022 {#release-notes-may-22}

A continuación encontrará todas las funciones incluidas en la versión del 22 de mayo. Consulte la edición para Marketo Engage de Adobe si hay disponibilidad de funcionalidades.

>[!AVAILABILITY]
>
>Funciones denotadas por una estrella (![star](assets/yellow-star.png)) son complementos de pago. Póngase en contacto con el representante del Marketo Engage para obtener más información.

**_Versiones trimestrales_**

Las siguientes funciones empezarán a lanzarse en **6 de mayo de 2022**, con un despliegue gradual de las funciones restantes en las semanas siguientes (a menos que se especifique lo contrario).

## Integración nativa de CRM {#native-crm-integration}

**Integración nativa de Veva CRM (disponibilidad limitada)**: Mejore la participación con los profesionales sanitarios mediante la sincronización de la actividad entre el VRM de Veva y el Marketo Engage a través de la integración nativa. Esta integración permite a los especialistas en marketing crear experiencias más personalizadas y fluidas entre canales para los profesionales sanitarios. Póngase en contacto con el gestor de éxito de los clientes si está interesado en participar.

## Organización en canales múltiples {#cross-channel-orchestration}

**Eventos de bots para la conversación dinámica**: Aproveche los datos de comportamiento más detallados para los visitantes web, como el tiempo en la página, el tiempo en el sitio y el porcentaje de desplazamiento de la página, para definir cuándo se debe mostrar un cuadro de diálogo de chat.

**PDF incrustado en Dynamic Chat**: Aumente la participación y comparta contenido significativo integrando PDF en los diálogos de chat y midiendo el rendimiento del contenido mediante el seguimiento de la actividad de participación.

**Compatibilidad ampliada de idiomas para Dynamic Chat**: La interfaz de usuario de Dynamic Chat ahora también estará disponible en francés, alemán, japonés, portugués y español. Los diálogos de chat también se pueden configurar en estos idiomas.

**Excluir direcciones URL para la conversación dinámica**: Controle cuál de sus páginas web aparece en Dynamic Chat con la capacidad de excluir direcciones URL específicas de los criterios de objetivo.

**Mejoras en el filtrado de actividades de bots de correo electrónico**: Continúe protegiendo el estado de la base de datos con la capacidad de identificar el comportamiento de los bots en función del vínculo oculto Agentes de usuario o IP y los patrones de proximidad, además de la identificación de coincidencias de la lista IAB existente. Vea las estadísticas de actividad de bots que le permiten comprender el número de actividades de bots identificadas para cada tipo.

**Encabezado STS para vínculos de seguimiento de correo electrónico**: Satisfaga las prácticas recomendadas de seguridad con la capacidad de aplicar encabezados de seguridad de transporte seguro para garantizar que el tráfico a los vínculos rastreados siempre sea seguro.

## Experiencia de próxima generación {#next-generation-experience}

**Alternar conmutador predeterminado a la experiencia de próxima generación**: el conmutador será el predeterminado para la nueva experiencia en todas las pantallas en las que esté disponible, lo que facilitará a los usuarios la detección de diseños actualizados y mejoras de uso.

**Pantalla actualizada en la experiencia de próxima generación**:

Estamos entregando la Vista de detalles de las plantillas de correo electrónico en Design Studio en la experiencia de próxima generación, lo que ofrece mejoras actualizadas de diseño y facilidad de uso a las que se puede acceder mediante el conmutador.

## Automatización de la experiencia {#experience-automation}

**Pasos de flujo de autoservicio (continuación beta)**: Amplíe la conectividad entre el Marketo Engage y el resto de la pila con la capacidad de crear pasos de flujo personalizados para utilizarlos en campañas inteligentes. Tanto los usuarios como los socios Marketo Engage pueden aprovechar esta funcionalidad para permitir el uso de servicios web externos en campañas de déclencheur, por lotes y ejecutables (a diferencia de los enlaces web que solo se pueden usar en campañas de déclencheur).

## Mejoras de API {#api-enhancements}

* **Acceso a la API ampliado para suscripciones con CRM habilitado**: Estamos ampliando el acceso a la API para suscripciones que tengan una sincronización de CRM habilitada para permitir a los usuarios recuperar Compañías, Oportunidades y Vendedores de parte del Marketo Engage.
* **Compatibilidad con tipos de datos &quot;ocultos&quot; en Forms**: Proporciona la capacidad de administrar campos de formulario ocultos mediante API.
* **Compatibilidad con varios valores de comparación para isNotForm mediante reglas**: Administre la visibilidad de los campos de formulario en función de si el valor de otro campo no es uno de los valores de una lista determinada.
* **Permitir la configuración de Mostrar y Enviar valores en Seleccionar listas por separado**: Defina el valor de visualización y el valor enviado en un campo por separado. Por ejemplo, mostrar el nombre de un hotel, pero enviar un ID interno al servidor.
* **Permitir la configuración de Deshabilitar el seguimiento abierto al crear o actualizar correo electrónico**: Cree un correo electrónico con el seguimiento de aperturas desactivado.

## Anuncios {#announcements}

**Verificación y unicidad del correo electrónico**: A partir de abril, comenzará la implementación de la verificación por correo electrónico. En este punto, las direcciones de correo electrónico de los usuarios Marketo Engage requerirán verificación y exclusividad (esto no se aplica a los usuarios solo de API). Los usuarios autenticados del servicio de directorio tendrán automáticamente sus correos electrónicos verificados cuando su suscripción esté habilitada con Verificación de correo electrónico.

La verificación de correo electrónico para suscripciones que utilizan la función &quot;Iniciar sesión en el cuadro de diálogo de invitación de usuario&quot; o que tienen un solo correo electrónico asociado con varios usuarios coincidirá con la versión de mayo. Las suscripciones que tengan un solo correo electrónico asociado con varios usuarios se habilitarán con la verificación de correo electrónico y requerirán que esos usuarios resuelvan el conflicto y utilicen un correo electrónico único por usuario. Cuando la función &quot;Iniciar sesión en el cuadro de diálogo de invitación de usuario&quot; está activada, los usuarios invitados mediante esta función deberán tener una dirección de correo electrónico única. Para los usuarios solo de API invitados mediante esta función, la dirección de correo electrónico no tiene que ser única.

**_Seminario web sobre la versión del producto_**

Únase a nosotros el 11 de mayo de 2022, a las 9:00 AM PT / 12:00 PM ET para un [seminario web en directo](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} alojado por nuestro equipo de productos, donde puede aprender a utilizar las últimas innovaciones de productos.
