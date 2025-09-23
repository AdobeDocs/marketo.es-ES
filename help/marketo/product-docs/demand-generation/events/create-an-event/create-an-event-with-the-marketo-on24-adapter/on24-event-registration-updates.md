---
unique-page-id: 10096683
description: Actualizaciones de registro de eventos ON24 - Documentos de Marketo - Documentación del producto
title: Actualizaciones de registro de eventos ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 2%

---

# Actualizaciones de registro de eventos ON24 {#on-event-registration-updates}

## Aprobación Manual De Registrantes {#manually-approving-registrants}

Puede aprobar manualmente a los registrantes antes de enviarles un correo electrónico de confirmación. Para ello, deberá configurar sus campañas para que gestionen este paso adicional:

1. Para la campaña de Déclencheur de registro:

   * En la [!UICONTROL lista inteligente], establezca el déclencheur en **[!UICONTROL Rellena el formulario]**.
   * En el flujo, establezca el [!UICONTROL estado en progresión] en **[!UICONTROL Aprobación pendiente]**.

1. Vaya al evento y haga clic en la ficha **[!UICONTROL Miembros]**. Esta pestaña muestra todas las personas que han rellenado el formulario. Su estado debe establecerse en **[!UICONTROL Aprobación pendiente]**.
1. Utilice el filtro de la parte superior de la cuadrícula para ver solamente las personas con un estado de **[!UICONTROL Aprobación pendiente]**.
1. Seleccione las personas que desea registrar (Mayús + clic, Control + clic o Seleccionar todo).
1. En el menú, haga clic en **[!UICONTROL Cambiar estado]**. Seleccione **[!UICONTROL Registrado]**, **[!UICONTROL Rechazado]** o cualquier otro estado aplicable.

## Gestión de personas con un error de registro {#handling-people-with-a-registration-error}

Si una persona termina sin estar registrada, pero se establece en el estado [!UICONTROL Error de registro], no es demasiado tarde para recuperarse.

1. En la ficha [!UICONTROL Miembros], filtre la lista de personas con el estado **[!UICONTROL Error de registro]**.
1. Antes de continuar, asegúrese de haber determinado y corregido el problema de integración (compruebe que no haya errores en **[!UICONTROL Socios de eventos]** en el administrador).
1. Una vez resuelto el problema, seleccione todas las personas con el estado [!UICONTROL Error de registro] y cambie su estado a **[!UICONTROL Registradas]**. Esto intentará registrarlos de nuevo con ON24.

## Actualizando estado de miembro de ON24 {#updating-member-status-from-on}

Marketo obtiene automáticamente la información de asistencia aproximadamente a las 23:00 (hora del Pacífico) cada noche. Para actualizar manualmente la información de asistencia, haga clic en **[!UICONTROL Actualizar del proveedor de seminarios web]** en **[!UICONTROL Acciones de eventos]**.

>[!MORELIKETHIS]
>
>[Explicación de los eventos del adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
