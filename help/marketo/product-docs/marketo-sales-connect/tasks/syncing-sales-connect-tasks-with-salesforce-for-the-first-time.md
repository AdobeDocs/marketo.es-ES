---
unique-page-id: 14352541
description: Sincronización de Tareas de Sales Connect con Salesforce por primera vez - Documentos de marketing - Documentación del producto
title: Sincronización de Tareas de Sales Connect con Salesforce por primera vez
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Sincronización de Tareas de Sales Connect con Salesforce por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Al activar por primera vez la sincronización entre las tareas de Sales Connect y Salesforce, importamos sus tareas de Salesforce. **no** impulsaremos cualquier tarea actual que tenga en Sales Connect a Salesforce. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan de Sales Connect a Salesforce son tareas creadas *después de* sincronizar Sales Connect con SFDC.

Esto es lo que sucede cuando sincroniza tareas de Sales Connect y SFDC:

- Tan pronto como haga clic en Guardar al sincronizar tareas, empezarán a sincronizarse. Inicialmente, esto llevará algún tiempo.

- Todos los recordatorios que se hayan actualizado o creado en las últimas 24 horas se extraerán de SFDC a Sales Connect. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el centro de comandos solo verá tareas que vencen hoy y mañana.

- Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, todo lo que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

- Sincronizaremos constantemente tareas entre Sales Connect y SFDC siempre que la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en Sales Connect se sincronizará con la lista de tareas de Salesforce. Y todo lo que se cree, edite, complete o elimine en Salesforce actualizará la lista de tareas en Sales Connect.

Para activar esta sincronización, marque la casilla de sincronización en la [página Configuración](https://toutapp.com/login) de la aplicación Web.
