---
description: ¿Por qué no se sincronizan mis campos de actividades y actividades de ventas con Salesforce? - Documentos de Marketo - Documentación del producto
title: ¿Por qué no se sincronizan mis campos de actividades y actividades de ventas con Salesforce?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# ¿Por qué no se sincronizan mis campos de actividades y actividades de ventas con Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**No veo las actividades de correo electrónico o llamada sincronizadas con Salesforce.**

* Asegúrese de que está conectado a Salesforce. Cada usuario deberá tener una conexión para registrar su correo electrónico y las llamadas a Salesforce.
* Asegúrese de haber configurado [Configuración de sincronización de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Los correos electrónicos registrarán la búsqueda en función del ID de Salesforce como búsqueda principal y la dirección de correo electrónico como secundaria. Puede confirmar que un registro de persona tiene un ID de Salesforce y una dirección de correo electrónico vinculados a ellos en la [aplicación web de acciones](https://toutapp.com/next#command_center){target="_blank"}.
* Las llamadas realizarán una búsqueda de registros basada únicamente en el ID de Salesforce. Si no existe ningún ID de Salesforce en el registro de persona en Actions, la llamada no se registrará. Puede confirmar que un registro de persona tiene un ID de Salesforce vinculado a él en la [aplicación web de acciones](https://toutapp.com/next#command_center){target="_blank"}.

**No veo campos de actividad en la actualización de Salesforce.**

Si no ve el correo electrónico [campos de atributos de actividad](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} actualizar en Salesforce, podría deberse a restricciones en la accesibilidad de los campos de su equipo. La seguridad de nivel de campo de Salesforce permite a los administradores de Salesforce establecer restricciones sobre la información que pueden ver y editar los usuarios. Si los usuarios de Acciones no tienen acceso para ver y editar estos campos, la sincronización de actividades de Acciones no podrá actualizar estos campos.

* Póngase en contacto con el administrador de Salesforce para asegurarse de que esta configuración de seguridad no interfiera con [los campos de actividad de Salesforce de acciones](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Si es administrador de Salesforce, puede ver la accesibilidad del campo en la pestaña Controles de seguridad. Los objetos principales con los que interactuarán las acciones son: posibles clientes, contactos, cuentas, oportunidades y tareas/actividades.

>[!NOTE]
>
>Los campos asociados con los objetos Posible cliente, Contacto, Cuenta y Oportunidad se instalarán con el paquete de Sales Insight Salesforce. Un administrador de Salesforce deberá crear los campos asociados con el tipo de registro [Tarea/Actividad](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
