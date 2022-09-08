---
unique-page-id: 10096683
description: Actualizaciones en el registro de eventos ON24 - Documentos de Marketo - Documentación del producto
title: Actualizaciones de registro de eventos ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Actualizaciones de registro de eventos ON24 {#on-event-registration-updates}

>[!IMPORTANT]
>
>A partir de agosto de 2022, ON24 ya no es compatible con las nuevas integraciones de Marketo. La información de este artículo solo se aplica a los usuarios existentes.

## Aprobación manual de los registros {#manually-approving-registrants}

Puede aprobar manualmente los usuarios registrados antes de enviarles un correo electrónico de confirmación. Para ello, deberá configurar las campañas para que se ocupen de este paso adicional:

1. Para la campaña Déclencheur de registro:

   * En la lista inteligente, establezca el déclencheur en **Rellena el formulario**.
   * En Flujo, establezca el estado en Progreso en **Pendiente de aprobación**.

1. Vaya al evento y haga clic en el botón **Miembros** pestaña . Esta ficha muestra todas las personas que han rellenado el formulario. Su estado debe establecerse en **Pendiente de aprobación**.
1. Utilice el filtro de la parte superior de la cuadrícula para ver solo las personas con un estado de **Pendiente de aprobación**.
1. Seleccione las personas que desea registrar (Mayús-clic, Control-clic o Seleccionar todo).
1. En el menú , haga clic en **Cambiar estado**. Select **Registrados**, **Rechazado**, o cualquier otro estado aplicable.

## Gestión de personas con un error de registro {#handling-people-with-a-registration-error}

Si una persona termina no siendo registrada, sino que se establece en el estado Error de registro, no es demasiado tarde para recuperarse.

1. En la pestaña Miembros , filtre la lista de personas con el estado **Error de registro**.
1. Antes de continuar, asegúrese de haber determinado y corregido el problema con la integración (compruebe que no hay errores en **Socios de eventos** en Administración).
1. Una vez resuelto el problema, seleccione todas las personas con el estado de error de registro y cambie su estado a **Registrados**. Esto intentará registrarlos de nuevo con ON24.

## Actualización del estado del miembro desde ON24 {#updating-member-status-from-on}

Marketo extrae automáticamente la información de asistencia aproximadamente a las 23:00 de la noche en el Pacífico. Para actualizar manualmente la información de asistencia, haga clic en **Actualizar desde el proveedor de seminarios web** under **Acciones de evento**.

>[!MORELIKETHIS]
>
>[Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
