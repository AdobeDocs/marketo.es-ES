---
description: 'Sincronización de datos de acción de ventas con Marketo y Salesforce: Documentos de Marketo: documentación del producto'
title: Sincronización de datos de acción de ventas con Marketo y Salesforce
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Sincronización de datos de acción de ventas con Marketo y Salesforce {#sync-sales-action-data-with-marketo-and-salesforce}

La sincronización de campos de unificación de datos para las acciones de perspectiva de ventas permite al sistema extraer información de la persona de la base de datos de Marketo Engage a la base de datos de acciones de perspectiva de ventas.

Esto proporciona datos de personas actualizados en la aplicación web Sales Insight Actions y permite al sistema recopilar ID únicos para los registros de personas correspondientes en Marketo y los registros de posible cliente/contacto/cuenta/oportunidad en Salesforce, de modo que se pueda hacer referencia correctamente a los registros para registrar datos.

Esta sincronización se puede activar desde la pestaña Sales Insight Actions Config de la sección Admin de Marketo Engage. Para obtener más información, consulte [Iniciar sincronización de datos](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

El diagrama anterior muestra cómo se pueden sincronizar los datos de actividad y de tarea de las personas entre sistemas. Algunas cosas que hay que tener en cuenta:

* Los registros de personas se sincronizan con las acciones de perspectiva de ventas de Marketo Engage, lo que convierte a Marketo Engage en la fuente fiable para los datos de personas de acciones de perspectiva de ventas
* Acciones de perspectiva de Marketo Engage y ventas [tener un mecanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) para recopilar y sincronizar el estado de cancelación de suscripción con Salesforce
* El estado de cancelación de suscripción no se sincroniza de las acciones de ventas a Marketo Engage, pero las acciones de información de ventas se pueden configurar para comprobar el estado de cancelación de suscripción de personas de Marketo antes de permitir que los vendedores envíen un correo electrónico con [Comprobación de cancelación de suscripción de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

A continuación, se muestran algunas de las preguntas más frecuentes relacionadas con el funcionamiento de la sincronización de unificación de datos.

## ¿Qué posibles clientes/contactos se sincronizan con las acciones de información de ventas? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Los posibles clientes y contactos que tengan un propietario de ventas asignado se sincronizan con las acciones de ventas.

Puede ver si un posible cliente/contacto tiene un propietario de ventas en Salesforce si consulta el campo de propietario estándar que existe.

El propietario de ventas no tiene que ser el usuario de sincronización de Marketo ni ningún usuario de ventas o fuerza de ventas específico. Todo lo que necesitamos es que haya un usuario enumerado en el campo Propietario del posible cliente y Propietario del contacto enumerado en Salesforce, de modo que podamos identificarlo como un posible cliente de ventas y sincronizarlo con las acciones de perspectiva de ventas. Cualquier actualización de los campos con los que sincronizamos también se detectará y actualizará en Acciones de perspectiva de ventas.

## ¿De dónde proceden los datos de actividad que se muestran en la cuadrícula inteligente de Sales Insight? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Los datos de la actividad, como el correo electrónico, la llamada, el momento interesante y la web, proceden todos de la base de datos de Marketo Engage. Sales Insight Smart Grid realiza una solicitud a la instancia de Marketo Engage para recuperarla cada vez que un usuario de ventas carga el panel Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Para garantizar que todos los datos de la actividad procedan del Marketo Engage, Acciones de perspectiva de ventas sincroniza todos los datos de la actividad con el Marketo Engage.

## ¿Qué campos relacionados con los registros de personas se sincronizan entre las acciones de Marketo Engage e Información de ventas? {#what-fields-sync}

Hay 11 campos que se sincronizan con las acciones de perspectiva de ventas de Marketo Engage:

* Nombre
* Apellido
* ID de contacto de Salesforce
* ID de posible cliente de Salesforce
* ID de cuenta de Salesforce
* ID de oportunidad de Salesforce
* ID de Marketo
* Compañía
* Título
* Correo electrónico
* Número de teléfono
* URL de Linkedin
* Origen

## ¿Se pueden configurar los campos que sincronizan las acciones de perspectiva de Marketo Engage y ventas? {#are-the-fields-that-sync-configurable}

No está disponible la configuración de qué campos de Marketo Engage se sincronizan con las acciones de información de ventas, ni tampoco la capacidad de asignar campos. La sincronización de Marketo asigna automáticamente campos estándar de Marketo a campos estándar de la instancia de acción de ventas.

## ¿Por qué las acciones de perspectiva de ventas tienen su propia base de datos? {#why-does-actions-have-its-own-database}

Sales Insight Actions tiene su propia aplicación web con una base de datos de personas y actividades dedicada para proporcionar un espacio de trabajo optimizado creado y diseñado para los equipos de ventas. Esto permite a los gestores de ventas y a los vendedores disponer de un espacio para desarrollar y gestionar su estrategia de participación sin conceder acceso ni privilegios al espacio de trabajo del Marketo Engage principal, que está optimizado para los especialistas en operaciones de marketing.

## ¿Cómo se gestionan los duplicados? {#how-are-duplicates-handled}

Su base de datos de acciones de ventas será una copia de las personas cualificadas (posibles clientes o contactos con un propietario de ventas) que existan en su base de datos de Marketo Engage. Esto significa que si hay dos registros con la misma dirección de correo electrónico creada en Marketo, se crea un registro duplicado en Acciones de ventas.

## ¿Cuánto tiempo tarda en completarse la sincronización inicial? {#how-long-initial-sync}

El proceso inicial para sincronizar todos los datos de posibles clientes en una nueva instancia de acciones de información de ventas procesará a las personas aproximadamente a 1000 cada 1-2 minutos. Esto es solo una estimación y puede variar.

Una vez que se realiza la sincronización inicial y todos los posibles clientes se han rellenado en la instancia de la aplicación web Acciones de información de ventas, se producirá una sincronización incremental que se ejecutará cada vez que haya una actualización en uno de los campos admitidos que se sincronicen.

## ¿Pueden los usuarios de Acciones de perspectiva de ventas editar los datos de personas desde la aplicación web Acciones? {#can-actions-users-edit-people-data}

No, la capacidad de crear y editar registros de personas en Acciones no está disponible para los usuarios y administradores de la aplicación web Acciones. La creación y edición de personas debe realizarse en Salesforce o en Marketo Engage. Las acciones de perspectiva de ventas utilizan Marketo como fuente fiable para los datos de personas mediante la sincronización continua de nuevos datos, de modo que si una persona se actualiza o crea en Marketo desde un flujo de trabajo en Marketo o se sincroniza desde Salesforce, dichas actualizaciones se pasarán a la base de datos de la aplicación web acciones de perspectiva de ventas.

## ¿Registran las actividades de ventas en Marketo? {#do-sales-activities-log-to-marketo}

Sí, las actividades de participación en ventas se registrarán en Marketo como actividades nativas. Estas actividades también incluyen filtros nativos que se pueden utilizar con restricciones para dirigirse a posibles clientes en función de los atributos de la actividad de ventas.

![](assets/actions-data-sync-faq-5.png)

A continuación se muestra una lista de las actividades que inician sesión en Marketo:

* Enviar email de ventas
* Abrir email de ventas
* Hacer clic en el email de ventas
* Correo electrónico de respuesta a ventas
* Se rechazó el email de ventas
* Llamada de ventas recibida
* Añadir a la campaña de ventas
* Se quitó de Campaña de ventas

## ¿Registran las actividades de ventas en Salesforce? {#do-sales-activities-log-to-salesforce}

Sí, las actividades de participación en ventas se registrarán en Salesforce como tareas nativas. Estas tareas se pueden usar en los informes de Salesforce para impulsar paneles de equipos que hagan un seguimiento de las actividades de ventas.

Las acciones de información de ventas permiten a los administradores configurar qué actividades de ventas se registran en Salesforce. Estas actividades incluyen correos electrónicos, llamadas y tareas de recordatorio de apertura.

![](assets/actions-data-sync-faq-6.png)

El diagrama anterior muestra qué información se registra en Salesforce. Las actividades como correos electrónicos y llamadas de se registran en Salesforce como [sincronización unidireccional](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md). [Cancela la suscripción](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) y [Tareas de recordatorio](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) se mantienen actualizados con una sincronización bidireccional. Cada una de estas sincronizaciones de datos se puede configurar desde la interfaz de la aplicación web Sales Insight Actions.

>[!MORELIKETHIS]
>
>* [Sincronización de cancelaciones de suscripción con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Comprobación de cancelación de suscripción de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Sincronizar actividades de ventas con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Sincronización de tareas de recordatorio con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Iniciar sincronización de datos](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
