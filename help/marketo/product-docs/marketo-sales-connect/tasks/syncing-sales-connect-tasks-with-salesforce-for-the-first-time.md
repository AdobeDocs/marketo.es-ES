---
unique-page-id: 14352541
description: Aprenda a sincronizar las tareas de Sales Connect con Salesforce por primera vez. Configure la sincronización de tareas para que las tareas aparezcan en Salesforce.
title: Sincronización de las tareas de Sales Connect con Salesforce por primera vez
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/5anDeeHVD0mkZLIac5rTb4vW7iiiOBHDBgQKUf5lv4Y
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 3%

---

# Sincronizando [!DNL Sales Connect] tareas con [!DNL Salesforce] por primera vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

La primera vez que active la sincronización entre [!DNL Sales Connect] y [!DNL Salesforce] tareas, importaremos sus [!DNL Salesforce] tareas. **no** insertaremos ninguna tarea actual que tenga en [!DNL Sales Connect] a [!DNL Salesforce]. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan de [!DNL Sales Connect] a [!DNL Salesforce] son las tareas creadas *después de* que sincronice [!DNL Sales Connect] con SFDC.

Esto es lo que sucede cuando sincroniza [!DNL Sales Connect] y tareas de SFDC:

- Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

- Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se recuperará de SFDC a [!DNL Sales Connect]. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

- Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

- Sincronizaremos constantemente las tareas entre [!DNL Sales Connect] y SFDC siempre y cuando la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en [!DNL Sales Connect] se sincronizará con su lista de tareas en [!DNL Salesforce]. Y todo lo que se cree, edite, complete o elimine en [!DNL Salesforce] actualizará su lista de tareas en [!DNL Sales Connect].

Para activar esta sincronización, simplemente marca la casilla de sincronización en tu [página de configuración](https://toutapp.com/login) en la aplicación web.
