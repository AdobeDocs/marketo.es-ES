---
description: Solucionar problemas cuando las actividades y los campos de ventas no se sincronizan con Salesforce. Compruebe el registro de API, los campos personalizados y los permisos.
title: ¿Por qué mis actividades de ventas y los campos de actividad no se sincronizan con Salesforce?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
TQID: https://experienceleague.adobe.com/ATXA1f3wZqC0z-QFjrK2ax0w8-wmf5cjKn4jdZJLtt0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 339
ht-degree: 6%

---

# ¿Por qué mis actividades de ventas y los campos de actividad no se sincronizan con Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**No veo actividades de correo electrónico o llamada sincronizadas con Salesforce.**

* Asegúrese de que está conectado a Salesforce. Cada usuario deberá tener una conexión para registrar su correo electrónico y las llamadas a Salesforce.
* Asegúrese de haber configurado [Configuración de sincronización de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Los correos electrónicos realizan una búsqueda de registros basada en el Salesforce ID como búsqueda principal y la dirección de correo electrónico como secundaria. Puede confirmar que un registro de persona tiene un Salesforce ID y una dirección de correo electrónico vinculados a ellos en la [aplicación web de acciones](https://toutapp.com/next#command_center){target="_blank"}.
* Las llamadas realizarán una búsqueda de registros basada únicamente en el Salesforce ID. Si no existe ningún Salesforce ID en el registro de persona en Actions, la llamada no se registrará. Puede confirmar que un registro de persona tiene un Salesforce ID vinculado a él en la [aplicación web de acciones](https://toutapp.com/next#command_center){target="_blank"}.

**No veo campos de actividad en la actualización de Salesforce.**

Si no ve el correo electrónico [campos de atributos de actividad](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} actualizar en Salesforce, puede deberse a restricciones en la accesibilidad de los campos de su equipo. La seguridad de nivel de campo de Salesforce permite a los administradores de Salesforce establecer restricciones sobre qué información pueden ver y editar los usuarios. Si los usuarios de Acciones no tienen acceso para ver y editar estos campos, la sincronización de actividades de Acciones no podrá actualizar estos campos.

* Póngase en contacto con el administrador de Salesforce para asegurarse de que esta configuración de seguridad no interfiera con [Acciones en los campos de actividad de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Si es administrador de Salesforce, puede ver la Accesibilidad de los campos en la pestaña Controles de seguridad. Los objetos principales con los que interactuarán las acciones son: posibles clientes, contactos, cuentas, oportunidades y tareas/actividades.

>[!NOTE]
>
>Los campos asociados con los objetos de cliente potencial, contacto, cuenta y oportunidad se instalarán con el paquete de Salesforce de Insight de ventas. Un administrador de Salesforce tendrá que crear los campos asociados con el tipo de registro [Tarea/Actividad](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
