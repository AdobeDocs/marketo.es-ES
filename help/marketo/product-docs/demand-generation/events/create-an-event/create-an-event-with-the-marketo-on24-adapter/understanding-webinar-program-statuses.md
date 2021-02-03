---
unique-page-id: 10096681
description: 'Explicación de los estados de Programa de seminario web: documentos de marketing: documentación del producto'
title: Explicación de los estados de Programa de seminario web
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Explicación de los estados de Programa de seminario web {#understanding-webinar-program-statuses}

Los estados de programa representan los distintos estados de evento que una persona avanza como miembro del evento. Están asociados a un tipo de canal. Marketo tiene un tipo de canal integrado llamado **Seminario web**. Los estados se pueden utilizar en campañas por lotes y déclencheur.

Las personas se mueven a través de los estados de programa de forma lineal y no regresan al estado. Por ejemplo, una persona con el estado **Asistencia** no puede volver a **Registrada**.

Esta es una breve descripción de los estados de programa asociados al canal de seminario web.

>[!TIP]
>
>Para actualizar manualmente los estados, haga clic en **Actualizar desde el proveedor de seminario web** en la lista desplegable **Acciones de Evento**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**No está en Programa** : utilice este estado para eliminar personas del evento.

**Invitado** : utilice este estado para agregar personas al evento.

**Pendiente de aprobación** : utilice este estado para retener el envío de un correo electrónico de confirmación a sus usuarios. Consulte &quot;Aprobación manual de registros&quot; en [Actualizaciones de registro de Evento en ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md) para obtener más información.

**Lista**  de espera: use este estado para mantener a algunas personas esperando hasta que haya más asientos disponibles.

**Rechazado** : Utilice este estado para rechazar el registro de una persona en su Evento.

**Registrado** : Este estado lleva a las personas a ON24 cuando se utiliza la integración de ON24. El estado de la persona se actualiza cuando ON24 responde que la persona se registró correctamente.

**Error**  de registro: este estado refleja que el usuario encontró un error al intentar registrarse en el Evento.

>[!NOTE]
>
>Si se produce un error de registro, puede obtener información adicional para esa persona consultando la columna Motivo de estado en la ficha Miembros de su programa. Una vez solucionado el error, puede cambiar manualmente el estado de programa del usuario a Registrado en el marketing.

**Asistida** - Al finalizar el seminario, ON24 devuelve una lista de personas que asistieron. Este estado se extrae automáticamente en Marketing.

**Asistencia bajo demanda** : las personas que asistieron a la versión archivada del seminario web reciben este estado.

**No Mostrar** : Al final del seminario web y después de extraer los datos de asistencia de ON24, el estado de las personas que se registraron pero no asistieron se actualiza a No Mostrar. El ON24 puede tardar entre 30 minutos y 3 horas en preparar la información de asistencia final y ponerla a disposición en Marketing.

>[!NOTE]
>
>Para que Marketing pueda extraer el estado No mostrar, las personas deben haberse registrado *en Marketing*. No podemos capturar No se muestran los datos procedentes de la fuente de datos On24.

>[!MORELIKETHIS]
>
>[Explicación de los Eventos del adaptador de Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
