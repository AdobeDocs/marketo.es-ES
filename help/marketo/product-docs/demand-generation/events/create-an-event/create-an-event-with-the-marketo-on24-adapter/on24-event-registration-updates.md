---
unique-page-id: 10096683
description: Actualizaciones del registro de Evento ON24 - Documentos de marketing - Documentación del producto
title: Actualizaciones de registro en Evento ON24
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---


# Actualizaciones de registro en Evento ON24 {#on-event-registration-updates}

## Aprobación manual de los registros {#manually-approving-registrants}

Puede aprobar manualmente los usuarios registrados antes de enviarles un mensaje de correo electrónico de confirmación. Para ello, deberá configurar sus campañas para gestionar este paso adicional:

1. Para la Campaña Activador de registro:

   * En la Lista inteligente, establezca el activador en **Rellenar formulario**.
   * En Flujo, establezca el estado en progresión en **Pendiente de aprobación**.

1. Vaya al Evento y haga clic en la ficha **Miembros** . Esta ficha muestra todas las personas que han rellenado el formulario. Su estado debe establecerse en **Pendiente de aprobación**.
1. Utilice el filtro situado en la parte superior de la cuadrícula para vista solo a las personas con un estado de **Pendiente de aprobación**.
1. Seleccione las personas que desee registrar (Mayús-clic, Control-clic o Seleccionar todo).
1. En el menú, haga clic en **Cambiar estado**. Seleccione **Registrado**, **Rechazado** o cualquier otro estado aplicable.

## Gestión de personas con un error de registro {#handling-people-with-a-registration-error}

Si una persona termina sin estar registrada, sino más bien configurada en el error de registro de estado, no es demasiado tarde para recuperarse.

1. En la ficha Miembros, filtre la lista de personas con el estado Error **de** registro.
1. Antes de continuar, asegúrese de haber determinado y corregido el problema con la integración (compruebe que no hay errores en Socios **de** Evento en Administración).
1. Una vez resuelto el problema, seleccione todas las personas con el estado Error de registro y cambie su estado a **Registrado**. Esto intentará registrarlos nuevamente con ON24.

## Actualización del estado del miembro desde ON24 {#updating-member-status-from-on}

Marketo extrae automáticamente la información de asistencia a las 11pm aproximadamente Pacific cada noche. Para actualizar manualmente la información de asistencia, haga clic en **Actualizar desde el proveedor** de seminario web en Acciones **de** Evento.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Explicación de los Eventos del adaptador de Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



