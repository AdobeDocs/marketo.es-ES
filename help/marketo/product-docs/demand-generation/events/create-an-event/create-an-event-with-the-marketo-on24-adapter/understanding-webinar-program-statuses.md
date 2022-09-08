---
unique-page-id: 10096681
description: 'Explicación de los estados del programa de los seminarios web: Documentos de Marketo: Documentación del producto'
title: Explicación de los estados del programa de los seminarios web
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Explicación de los estados del programa de los seminarios web {#understanding-webinar-program-statuses}

>[!IMPORTANT]
>
>A partir de agosto de 2022, ON24 ya no es compatible con las nuevas integraciones de Marketo. La información de este artículo solo se aplica a los usuarios existentes.

Los estados de programa representan los diferentes estados de evento por los que una persona avanza como miembro del evento. Están asociados a un tipo de canal. Marketo tiene un tipo de canal integrado denominado **Seminario web**. Los estados se pueden utilizar en campañas por lotes y de déclencheur.

Las personas pasan por los estados del programa de forma lineal y no vuelven al estado. Por ejemplo, una persona con un estado de **Asistida** no se puede volver a **Registrados**.

A continuación se muestra una breve descripción de los estados de programa asociados al canal de seminario web.

>[!TIP]
>
>Para actualizar manualmente los estados, haga clic en  **Actualizar desde el proveedor de seminarios web** en el **Acciones de evento** lista desplegable.

![](assets/image2015-12-17-13-3a52-3a39.png)

**No está en el programa** - Utilice este estado para eliminar personas del evento.

**Invitado** - Utilice este estado para añadir personas al evento.

**Pendiente de aprobación** - Utilice este estado para permanecer desactivada al enviar a su gente un correo electrónico de confirmación. Consulte &quot;Aprobación manual de registros&quot; en [Actualizaciones de registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md) para obtener más información.

**Espera enumerada** - Utilice este estado para mantener a algunas personas esperando hasta que haya asientos adicionales disponibles.

**Rechazado** - Utilice este estado para rechazar el registro de una persona en su Evento.

**Registrados** - Este estado lleva a las personas a ON24 cuando está utilizando la integración ON24. El estado de la persona se actualiza cuando ON24 responde que la persona se registró correctamente.

**Error de registro** : este estado refleja que el usuario ha encontrado un error al intentar registrarse en el evento.

>[!NOTE]
>
>Si se produce un error de registro, puede obtener información adicional para esa persona consultando la columna Razón de estado en la pestaña Miembros de su programa. Una vez corregido el error, puede cambiar manualmente el estado del programa del usuario a Registrado en Marketo.

**Asistida** - Al final del seminario web, ON24 devuelve una lista de personas que asistieron. Este estado se incorpora automáticamente a Marketo.

**Asistencia bajo demanda** - Las personas que asistieron a la versión archivada del seminario web reciben este estado.

**No mostrar** - Al final del seminario web y después de extraer los datos de asistencia de ON24, el estado de las personas que se registraron pero no asistieron se actualiza a No Show. Puede tardar entre 30 minutos y 3 horas en que ON24 prepare la información de asistencia final y la ponga a disposición en Marketo.

>[!NOTE]
>
>Para que Marketo pueda extraer el estado No mostrar , las personas deben estar registradas *en Marketo*. No se pueden capturar los &quot;No shows&quot; que provienen de la fuente de datos On24.

>[!MORELIKETHIS]
>
>[Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
