---
unique-page-id: 10096681
description: Explicación de los estados de programas de seminarios web - Documentos de Marketo - Documentación del producto
title: Explicación de los estados del programa seminario web
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Explicación de los estados del programa seminario web {#understanding-webinar-program-statuses}

Los estados de programa representan los diferentes estados de evento por los que progresa una persona como miembro del evento. Están asociados a un tipo de canal. Marketo tiene un tipo de canal integrado llamado **Seminario web**. Los estados se pueden utilizar en campañas por lotes y de déclencheur.

Las personas se desplazan por los estados de los programas de forma lineal y no regresan a su estado anterior. Por ejemplo, una persona con un estado de **Asistió** no se puede volver a mover a **Registrados**.

A continuación se muestra una breve descripción de los estados de programa asociados al canal del seminario web.

>[!TIP]
>
>Para actualizar los estados manualmente, haga clic en  **Actualizar del proveedor de seminarios web** en el **Acciones de evento** menú desplegable.

![](assets/image2015-12-17-13-3a52-3a39.png)

**No está en el programa** : utilice este estado para eliminar personas del evento.

**Invitado** : utilice este estado para añadir personas al evento.

**Pendiente de aprobación** : utilice este estado para mantener desactivado el envío de su gente un correo electrónico de confirmación. Consulte &quot;Aprobación manual de solicitantes&quot; en [Actualizaciones de registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} para obtener más información.

**Lista de espera** : utilice este estado para mantener a algunas personas esperando hasta que haya puestos adicionales disponibles.

**Rechazado** - Utilice este estado para rechazar el registro de una persona en su Evento.

**Registrados** : Este estado lleva a las personas a ON24 cuando se utiliza la integración ON24. El estado de la persona se actualiza cuando ON24 responde que se registró correctamente.

**Error de registro** : Este estado refleja un error del usuario al intentar registrarse en el evento.

>[!NOTE]
>
>Si se produce un error de registro, puede obtener información adicional para esa persona mirando la columna Motivo del estado en la pestaña Miembros del programa. Una vez corregido el error, puede cambiar manualmente el estado del programa del usuario a Registrado en Marketo.

**Asistió** - Al final del seminario web, ON24 devuelve una lista de personas que asistieron. Este estado se incorpora automáticamente a Marketo.

**Asistencia a petición** - Las personas que asistieron a la versión archivada del seminario web reciben este estado.

**No mostrar** - Al final del seminario web y después de que se recuperen los datos de asistencia de ON24, el estado de las personas que se registraron pero no asistieron se actualiza a No Show. ON24 puede tardar entre 30 minutos y 3 horas en preparar la información final de asistencia y ponerla a disposición en Marketo.

>[!NOTE]
>
>Para que Marketo extraiga el estado No mostrar, las personas deben estar registradas *en Marketo*. No podemos capturar Ningún programa que provenga de la fuente de datos On24.

>[!MORELIKETHIS]
>
>[Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
