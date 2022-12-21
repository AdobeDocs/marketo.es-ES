---
unique-page-id: 14352541
description: 'Sincronización de tareas de conexión de ventas con Salesforce por primera vez: Marketo Docs: documentación del producto'
title: Sincronización de tareas de conexión de ventas con Salesforce por primera vez
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sincronización de tareas de conexión de ventas con Salesforce por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Cuando activa por primera vez la sincronización entre las tareas de Conexión de ventas y Salesforce, importamos sus tareas de Salesforce. Nosotros **not** traspase cualquier tarea actual que tenga en Conexión de ventas a Salesforce. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan desde Conexión de ventas a Salesforce son las tareas creadas *after* sincroniza Sales Connect con SFDC.

Esto es lo que sucede cuando sincroniza las tareas de Conexión de ventas y SFDC:

- Tan pronto como haga clic en guardar en la sincronización de tareas, empezarán a sincronizarse. Inicialmente, esto llevará algún tiempo.

- Todos los recordatorios que se hayan actualizado o creado en las últimas 24 horas se extraerán de SFDC a Sales Connect. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el centro de comandos solo verá las tareas que vencen hoy y mañana.

- Si la sincronización se ha activado anteriormente y elimina cualquier tarea en SFDC, todo lo que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

- Sincronizaremos tareas constantemente entre Sales Connect y SFDC siempre que la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en Sales Connect se sincronizará con la lista de tareas de Salesforce. Y todo lo creado, editado, completado o eliminado en Salesforce actualizará su lista de tareas en Conexión de ventas.

Para activar esta sincronización, marque la casilla de sincronización en su [Página Configuración](https://toutapp.com/login) en la aplicación web.
