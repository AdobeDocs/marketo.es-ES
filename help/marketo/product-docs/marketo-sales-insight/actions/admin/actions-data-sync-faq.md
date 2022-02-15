---
description: Preguntas frecuentes sobre la sincronización de datos de acciones - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre la sincronización de datos de acciones
hide: true
hidefromtoc: true
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 8ded6cac96f17c81a8d37cbe51c39ad565ac828e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Preguntas frecuentes sobre la sincronización de datos de acciones {#actions-data-sync-faq}

La sincronización de campos de unificación de datos para acciones de perspectiva de ventas permite al sistema extraer información de las personas de la base de datos de Marketo Engage a la base de datos de acciones de perspectiva de ventas.

Esto proporciona datos de personas actualizados en la aplicación web Acciones de perspectiva de ventas y permite que el sistema recopile ID únicos para los registros de personas correspondientes en Marketo y registros de posible cliente/contacto/cuenta/oportunidad en Salesforce, de modo que se pueda hacer referencia a los registros correctamente para registrar datos.

Esta sincronización se puede habilitar desde la pestaña Configuración de acciones de perspectiva de ventas en la sección Administración del Marketo Engage. Para obtener más información, consulte [Iniciar sincronización de datos](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/msi-actions-admin-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

El diagrama anterior muestra cómo se pueden sincronizar los datos de actividades y tareas de las personas entre sistemas. Algunas cosas a tener en cuenta:

* Los registros de personas se sincronizan con las acciones de perspectiva de ventas del Marketo Engage, lo que convierte al Marketo Engage en la fuente de datos de personas de las acciones de perspectiva de ventas
* Acciones de perspectivas de Marketo Engage y ventas [tener un mecanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) para recopilar y sincronizar el estado de cancelación de suscripción a Salesforce
* El estado de cancelación de suscripción no se sincroniza de las acciones de ventas con el Marketo Engage, pero las acciones de perspectiva de ventas se pueden configurar para comprobar el estado de cancelación de suscripción de Marketo de las personas antes de permitir que los vendedores envíen un correo electrónico con [Comprobación de cancelación de suscripción de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

A continuación se presentan algunas preguntas frecuentes relacionadas con el funcionamiento de la sincronización de datos.

## ¿Qué posibles clientes/contactos se sincronizan con las acciones de perspectivas de ventas? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Los posibles clientes y contactos que tengan un propietario de ventas asignado se sincronizarán en Acciones de ventas.

Puede ver si un posible cliente o contacto tiene un propietario de ventas en Salesforce consultando el campo propietario estándar que existe.

El propietario de ventas no tiene que ser el usuario de sincronización de Marketo ni ningún usuario de ventas o Salesforce específico. Todo lo que necesitamos es que haya un usuario listado en el campo propietario del posible cliente y propietario del contacto que aparece en Salesforce, para que podamos identificarlo como posible cliente de ventas y sincronizarlo con las acciones de perspectiva de ventas. Las actualizaciones de los campos con los que sincronizamos también se detectarán y actualizarán en las acciones de perspectiva de ventas.

## ¿De dónde provienen los datos de actividad mostrados en la cuadrícula inteligente de perspectivas de ventas? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Los datos de la actividad, como el correo electrónico, la llamada, el momento interesante y la web, se obtienen de la base de datos del Marketo Engage. La cuadrícula inteligente de perspectiva de ventas realiza una solicitud a la instancia de Marketo Engage para recuperarla cada vez que un usuario de ventas carga el panel Perspectiva de ventas .

![](assets/actions-data-sync-faq-4.png)

Para garantizar que todos los datos de actividad se puedan obtener de un Marketo Engage, las acciones de perspectiva de ventas sincronizan todos los datos de actividad con un Marketo Engage.

## ¿Qué campos relacionados con los registros de personas se sincronizan de Marketo Engage a acciones de perspectiva de ventas? {#what-fields-sync}

Hay 11 campos que se sincronizan desde Marketo Engage a acciones de perspectiva de ventas:

* Nombre
* Apellido
* ID de contacto de Salesforce
* ID de posible cliente de Salesforce
* Marketo ID
* Compañía
* Título
* Email
* Número de teléfono
* URL de Linkedin
* Origen

## ¿Los campos que se sincronizan entre Marketo Engage y Acciones de perspectiva de ventas son configurables? {#are-the-fields-that-sync-configurable}

La configuración de la sincronización de campos de Marketo Engage con las acciones de perspectiva de ventas no está disponible, al igual que la capacidad de asignar campos. La sincronización de Marketo asigna automáticamente los campos estándar de Marketo a los campos estándar de la instancia de acción de ventas.

## ¿Por qué Sales Insight Actions tiene su propia base de datos? {#why-does-actions-have-its-own-database}

Sales Insight Actions tiene su propia aplicación web con una base de datos de persona y actividad dedicada para proporcionar un espacio de trabajo optimizado creado y diseñado para los equipos de ventas. Esto permite que los responsables de ventas y los vendedores tengan un espacio para desarrollar y administrar su estrategia de participación sin conceder acceso o privilegios al espacio de trabajo del Marketo Engage principal, que está optimizado para los especialistas en operaciones de marketing.

## ¿Cómo se gestionan los duplicados? {#how-are-duplicates-handled}

La base de datos de acciones de ventas será una copia de las personas cualificadas (posibles clientes/contactos con un propietario de ventas) que existan en la base de datos de Marketo Engage. Esto significa que si hay dos registros con la misma dirección de correo electrónico creada en Marketo, habrá un registro duplicado creado en Acciones de ventas.

## ¿Cuánto tiempo se tarda en completar la sincronización inicial? {#how-long-initial-sync}

El proceso inicial para sincronizar todos los datos de posibles clientes de ventas en una nueva instancia de acciones de perspectiva de ventas normalmente procesará a las personas en aproximadamente 1000 cada 1-2 minutos. Esto es solo una estimación y puede variar.

Una vez que se realice la sincronización inicial y que todos los posibles clientes de ventas se hayan rellenado en la instancia de la aplicación web Acciones de perspectiva de ventas, habrá una sincronización incremental que se ejecutará cada vez que se actualice uno de los campos admitidos que se hayan sincronizado.

## ¿Pueden los usuarios de Acciones de perspectiva de ventas editar los datos de personas desde la aplicación web Acciones? {#can-actions-users-edit-people-data}

No, la capacidad de crear y editar registros de personas en Acciones no está disponible para los usuarios ni para los administradores de la aplicación web de Acciones. La creación y edición de personas debe realizarse en Salesforce o en el Marketo Engage. Las acciones de perspectiva de ventas utilizan Marketo como su fuente de verdad para los datos de personas mediante la sincronización continua de nuevos datos, por lo que si una persona se actualiza o crea en Marketo desde un flujo de trabajo en Marketo o se sincroniza desde Salesforce, esas actualizaciones se pasarán a la base de datos de la aplicación web Acciones de perspectiva de ventas .

## ¿Las actividades de ventas se registran en Marketo? {#do-sales-activities-log-to-marketo}

Sí, las actividades de participación de ventas registrarán en Marketo como actividades nativas. Estas actividades también incluyen filtros nativos que se pueden usar con restricciones para segmentar posibles clientes en función de los atributos de actividad de ventas.

![](assets/actions-data-sync-faq-5.png)

A continuación se muestra una lista de las actividades que inician sesión en Marketo:

* Enviar email de ventas
* Abrir email de ventas
* Hacer clic en el email de ventas
* Respondido a correo electrónico de ventas
* Se rechazó el email de ventas
* Llamada de ventas recibida
* Agregar a la campaña de ventas
* Eliminado de la campaña de ventas

## ¿Las actividades de ventas se registran en Salesforce? {#do-sales-activities-log-to-salesforce}

Sí, las actividades de participación de ventas registrarán en Salesforce como tareas nativas. Estas tareas se pueden utilizar en los informes de Salesforce para impulsar los paneles de equipo que rastrean las actividades de ventas.

Las acciones de perspectiva de ventas permiten a los administradores configurar qué actividades de ventas se registran en Salesforce. Estas actividades incluyen correos electrónicos, llamadas y tareas de recordatorio abiertas.

![](assets/actions-data-sync-faq-6.png)

El diagrama anterior muestra qué información se registra en Salesforce. Actividades como correos electrónicos y llamadas se registran en Salesforce en un [sincronización unidireccional](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Cancelación de suscripción](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) y [Tareas de recordatorio](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) se mantienen actualizados con una sincronización bidireccional. Cada una de estas sincronizaciones de datos se puede configurar desde la interfaz de la aplicación web Acciones de perspectiva de ventas .

>[!MORELIKETHIS]
>
>* [Sincronización de la cancelación de suscripciones con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Comprobación de cancelación de suscripción de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Configuración de sincronización de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronización de tareas de recordatorio con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Iniciar sincronización de datos](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/msi-actions-admin-guide.md#initiate-data-sync)

