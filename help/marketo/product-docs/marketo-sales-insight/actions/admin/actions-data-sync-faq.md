---
description: 'Preguntas frecuentes sobre la sincronización de datos de acciones: documentos de Marketo, documentación del producto'
title: Preguntas frecuentes sobre sincronización de datos de acciones
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%

---

# Preguntas frecuentes sobre sincronización de datos de acciones {#actions-data-sync-faq}

La sincronización de campos de unificación de datos para [!DNL Sales Insight Actions] permite que el sistema extraiga información personal de la base de datos de Marketo Engage en la base de datos de [!DNL Sales Insight Actions].

Esto proporciona datos de personas actualizados en la aplicación web [!DNL Sales Insight Actions] y permite al sistema recopilar identificadores únicos para los registros de persona correspondientes en Marketo y los registros de posible cliente/contacto/cuenta/oportunidad en [!DNL Salesforce], de modo que se pueda hacer referencia correctamente a los registros para registrar los datos.

Esta sincronización se puede habilitar desde la pestaña [!DNL Sales Insight Actions] Config en la sección Admin de Marketo Engage. Para obtener más información, consulta [Iniciar sincronización de datos](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

El diagrama anterior muestra cómo se pueden sincronizar los datos de actividad y de tarea de las personas entre sistemas. Algunas cosas que hay que tener en cuenta:

* Los registros de personas se sincronizan con [!DNL Sales Insight Actions] desde Marketo Engage, lo que convierte a Marketo Engage en la fuente fiable para los datos de [!DNL Sales Insight Actions] personas
* Tanto Marketo Engage como [!DNL Sales Insight Actions] [tienen un mecanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) para recopilar y sincronizar el estado de cancelación de suscripción a [!DNL Salesforce]
* El estado de cancelación de suscripción no se sincroniza de las acciones de ventas a Marketo Engage, pero [!DNL Sales Insight Actions] se puede configurar para comprobar el estado de cancelación de suscripción de Marketo de las personas antes de permitir que los vendedores envíen un correo electrónico con [Verificación de cancelación de suscripción de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

A continuación, se muestran algunas de las preguntas más frecuentes relacionadas con el funcionamiento de la sincronización de unificación de datos.

## ¿Qué posibles clientes/contactos se sincronizan con [!DNL Sales Insight Actions]? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Los posibles clientes y contactos que tengan un propietario de ventas asignado se sincronizan con las acciones de ventas.

Puede ver si un posible cliente/contacto tiene un propietario de ventas en [!DNL Salesforce] mirando el campo de propietario estándar que existe.

El propietario de ventas no tiene que ser el usuario de sincronización de Marketo ni ningún [!DNL Salesforce] o usuario de ventas específico. Todo lo que necesitamos es que haya un usuario en el campo Propietario del posible cliente y Propietario del contacto en [!DNL Salesforce], para que podamos identificarlo como posible cliente de ventas y sincronizarlo con [!DNL Sales Insight Actions]. Cualquier actualización de los campos con los que sincronizamos también se detectará y actualizará en [!DNL Sales Insight Actions].

## ¿De dónde proceden los datos de actividad que se muestran en la cuadrícula inteligente de Insight de ventas? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Los datos de la actividad, como el correo electrónico, la llamada, el momento interesante y la web, proceden todos de la base de datos de Marketo Engage. Sales Insight Smart Grid realiza una solicitud a la instancia de Marketo Engage para recuperarla cada vez que un usuario de ventas carga el panel Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Para asegurarse de que todos los datos de la actividad procedan de Marketo Engage, [!DNL Sales Insight Actions] sincroniza todos los datos de la actividad con Marketo Engage.

## ¿Qué campos están relacionados con la sincronización de registros de personas de Marketo Engage a [!DNL Sales Insight Actions]? {#what-fields-sync}

Hay 11 campos que se sincronizan de Marketo Engage a [!DNL Sales Insight Actions]:

* Nombre
* Apellido
* [!DNL Salesforce] ID de contacto
* [!DNL Salesforce] ID de posible cliente
* ID de cuenta [!DNL Salesforce]
* [!DNL Salesforce] ID de oportunidad
* Identificación de Marketo
* Compañía
* Título
* Correo electrónico
* Número de teléfono
* URL [!DNL Linkedin]
* Origen

## ¿Se pueden configurar los campos que se sincronizan entre Marketo Engage y [!DNL Sales Insight Actions]? {#are-the-fields-that-sync-configurable}

No está disponible la configuración de la sincronización de los campos de Marketo Engage con [!DNL Sales Insight Actions], ni tampoco la capacidad de asignar campos. La sincronización de Marketo asigna automáticamente campos estándar de Marketo a campos estándar de la instancia de acción de ventas.

## ¿Por qué [!DNL Sales Insight Actions] tiene su propia base de datos? {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions] tiene su propia aplicación web con una base de datos de personas y actividades dedicada para proporcionar un espacio de trabajo optimizado que se ha creado y diseñado para los equipos de ventas. Esto permite a los gestores de ventas y a los vendedores disponer de un espacio para desarrollar y gestionar su estrategia de participación   sin conceder acceso ni privilegios al espacio de trabajo principal de Marketo Engage, que está optimizado para especialistas en operaciones de marketing.

## ¿Cómo se gestionan los duplicados? {#how-are-duplicates-handled}

Su base de datos de acciones de ventas será una copia de las personas cualificadas (posibles clientes o contactos con un propietario de ventas) que existan en su base de datos de Marketo Engage. Esto significa que si hay dos registros con la misma dirección de correo electrónico creada en Marketo, se crea un registro duplicado en Acciones de ventas.

## ¿Cuánto tiempo tarda en completarse la sincronización inicial? {#how-long-initial-sync}

El proceso inicial para sincronizar todos los datos de posibles clientes en una nueva instancia de [!DNL Sales Insight Actions] procesará a las personas aproximadamente a las 1000 cada 1-2 minutos. Esto es solo una estimación y puede variar.

Una vez que se realice la sincronización inicial y se hayan rellenado todos los posibles clientes en la instancia de la aplicación web [!DNL Sales Insight Actions], se producirá una sincronización incremental que se ejecutará cada vez que haya una actualización en uno de los campos admitidos que se sincronicen.

## ¿Pueden los usuarios de [!DNL Sales Insight Actions] editar los datos de personas desde la aplicación web Acciones? {#can-actions-users-edit-people-data}

No, la capacidad de crear y editar registros de personas en Acciones no está disponible para los usuarios y administradores de la aplicación web Acciones. La creación y edición de personas debe realizarse en [!DNL Salesforce] o Marketo Engage. [!DNL Sales Insight Actions] usa Marketo como fuente fiable para los datos de personas mediante la sincronización continua de nuevos datos, de modo que si una persona se actualiza o se crea en Marketo desde un flujo de trabajo en Marketo o se sincroniza desde [!DNL Salesforce], esas actualizaciones se pasarán a la base de datos de la aplicación web [!DNL Sales Insight Actions].

## ¿Registran las actividades de ventas en Marketo? {#do-sales-activities-log-to-marketo}

Sí, las actividades de participación en ventas se registrarán en Marketo como actividades nativas. Estas actividades también incluyen filtros nativos que se pueden utilizar con restricciones para dirigirse a posibles clientes en función de los atributos de la actividad de ventas.

![](assets/actions-data-sync-faq-5.png)

A continuación se muestra una lista de las actividades que inician sesión en Marketo:

* Enviar correo electrónico de ventas
* Abrir correo electrónico de ventas
* Hacer clic en el correo electrónico de ventas
* Respondió al email de ventas
* Se rechazó el email de ventas
* Llamada de ventas recibida
* Agregar a la campaña de ventas
* Se quitó de Campaña de ventas

## ¿Las actividades de ventas registran en [!DNL Salesforce]? {#do-sales-activities-log-to-salesforce}

Sí, las actividades de participación en ventas registrarán [!DNL Salesforce] como tareas nativas. Estas tareas se pueden usar en [!DNL Salesforce] informes para impulsar los paneles de los equipos que hacen un seguimiento de las actividades de ventas.

[!DNL Sales Insight Actions] permite a los administradores configurar qué actividades de ventas se han registrado en [!DNL Salesforce]. Estas actividades incluyen correos electrónicos, llamadas y tareas de recordatorio de apertura.

![](assets/actions-data-sync-faq-6.png)

El diagrama anterior muestra qué información se ha registrado en [!DNL Salesforce]. Las actividades como correos electrónicos y llamadas se han registrado en [!DNL Salesforce] en una [sincronización unidireccional](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). Las [cancelaciones de suscripciones](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) y las [tareas de recordatorio](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) se mantienen actualizadas con una sincronización bidireccional. Cada una de estas sincronizaciones de datos se puede configurar desde la interfaz de la aplicación web [!DNL Sales Insight Actions].

>[!MORELIKETHIS]
>
>* [Sincronizando cancelaciones de suscripción con [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Comprobación de cancelación de suscripción de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] Configuración de sincronización](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronización de tarea de recordatorio con [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Iniciar sincronización de datos](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
