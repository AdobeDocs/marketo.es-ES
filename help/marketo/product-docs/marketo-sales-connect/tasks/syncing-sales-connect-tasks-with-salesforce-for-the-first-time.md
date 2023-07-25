---
unique-page-id: 14352541
description: 'Sincronización de tareas de conexión de ventas con Salesforce por primera vez: documentos de Marketo, documentación del producto'
title: Sincronización de tareas de conexión de ventas con Salesforce por primera vez
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sincronización de tareas de conexión de ventas con Salesforce por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Cuando active por primera vez la sincronización entre las tareas de Sales Connect y Salesforce, importaremos sus tareas de Salesforce. Lo haremos **no** Pase cualquier tarea actual que tenga en Sales Connect a Salesforce. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan con Sales Connect son las creadas *después* se sincroniza Sales Connect con SFDC.

Esto es lo que sucede cuando sincroniza las tareas de Sales Connect y SFDC:

- Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

- Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se recuperará de SFDC a Sales Connect. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

- Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

- Siempre que la sincronización esté habilitada, sincronizaremos constantemente las tareas entre Sales Connect y SFDC.

Tras la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en Sales Connect se sincronizará con la lista de tareas de Salesforce. Y todo lo que se cree, edite, complete o elimine en Salesforce actualizará su lista de tareas en Sales Connect.

Para activar esta sincronización, simplemente marque la casilla de sincronización en su [Página Configuración](https://toutapp.com/login) en la aplicación web.
