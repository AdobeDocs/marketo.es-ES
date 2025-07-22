---
description: Configuración de sincronización de Salesforce - Documentos de Marketo - Documentación del producto
title: Configuraciones de sincronización de Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 1%

---

# Configuración de sincronización de [!DNL Salesforce] {#salesforce-sync-settings}

## Registrando actividad de correo electrónico en [!DNL Salesforce] mediante API {#logging-email-activity-to-salesforce-via-api}

Esta funcionalidad requiere que esté en la edición Enterprise/Unlimited de [!DNL Salesforce] o en la edición Professional si ha adquirido Integration a través de la API de Web Services.

>[!PREREQUISITES]
>
>[!DNL Salesforce] y [!DNL Sales Insight Actions] deben estar conectados.

1. En [!DNL Sales Insight Actions], haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/salesforce-sync-settings-1.png)

1. En [!UICONTROL Configuración de administración] (o &quot;[!UICONTROL Mi cuenta]&quot; si no eres administrador), haz clic en **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-2.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de sincronización]**.

   ![](assets/salesforce-sync-settings-3.png)

1. Haga clic en la flecha junto a [!UICONTROL Registrar actividad de correo electrónico] en [!DNL Salesforce].

   ![](assets/salesforce-sync-settings-4.png)

1. Haga clic en la ficha **[!UICONTROL API de Salesforce]**. En esta tarjeta puede configurar su preferencia para registrar información en [!DNL Salesforce]. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/salesforce-sync-settings-5.png)

## Registrando actividad de correo electrónico en [!DNL Salesforce] por correo electrónico en [!DNL Salesforce] (CCO) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Una vez que active &quot;[!UICONTROL Correo electrónico a Salesforce (CCO)]&quot;, recibirá un CCO de sus correos electrónicos de ventas y sus correos electrónicos se registrarán como actividades en oportunidades, posibles clientes y contactos.

>[!PREREQUISITES]
>
>[!DNL Salesforce] y [!DNL Sales Insight Actions] deben estar conectados.

**Para registrar sus correos electrónicos en [!DNL Salesforce] por correo electrónico (CCO)**

1. En Marketo Sales, haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/salesforce-sync-settings-6.png)

1. En [!UICONTROL Configuración de administración] (o &quot;[!UICONTROL Mi cuenta]&quot; si no eres administrador), haz clic en **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-7.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de sincronización]**.

   ![](assets/salesforce-sync-settings-8.png)

1. Haga clic en la ficha **[!UICONTROL Correo electrónico a Salesforce (CCO)]** y luego en **[!UICONTROL Activar]**.

   ![](assets/salesforce-sync-settings-9.png)

Si, por alguna razón, el correo electrónico a la dirección [!DNL Salesforce] no se extrae, siga estos pasos para activar la función CCO en su cuenta de [!DNL Salesforce]:

1. Inicie sesión en su instancia de [!DNL Salesforce].
1. Busque su nombre de usuario en la esquina superior derecha y seleccione la barra desplegable.
1. Seleccione **[!UICONTROL Mi configuración]**.
1. Seleccione **[!UICONTROL Correo electrónico]**.
1. Seleccione **[!UICONTROL Mi correo electrónico a Salesforce]**.
1. En esta página, verá un campo denominado &quot;[!UICONTROL Correo electrónico a la dirección de Salesforce]&quot;. Si no hay nada completado junto a él, desplácese hacia abajo hasta &quot;[!UICONTROL Mis direcciones de correo electrónico aceptables]&quot;.
1. Introduzca las direcciones de correo electrónico que desea incluir en la lista de destinatarios copiados ocultos (CCO).
1. Haga clic en **[!UICONTROL Guardar cambios]**.

**No puedo encontrar mi correo electrónico a [!DNL Salesforce] en Mi configuración**

Si no ve Mi correo electrónico a [!DNL Salesforce] en su configuración, es posible que el administrador no lo haya habilitado. Esto puede suceder si su equipo es nuevo en [!DNL Salesforce] o si su equipo nunca ha usado la dirección de CCO que [!DNL Salesforce] proporciona.

>[!NOTE]
>
>Necesitará privilegios de administrador para configurar esto.

1. Haga clic en **[!UICONTROL Configuración]**.
1. Haga clic en **[!UICONTROL Administración de correo electrónico]**.
1. Haga clic en **[!UICONTROL Correo electrónico a Salesforce]**.
1. Haga clic en **[!UICONTROL Editar]**.
1. Marque la casilla junto a &quot;Activo&quot;.
1. Haga clic en **[!UICONTROL Guardar]**.

## Sincronizar [!DNL Sales Insight Actions] tareas/recordatorios con [!DNL Salesforce] tareas {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. En [!DNL Sales Insight Actions], haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/salesforce-sync-settings-10.png)

1. En [!UICONTROL Configuración de administración] (o &quot;[!UICONTROL Mi cuenta]&quot; si no eres administrador), haz clic en **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-11.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de sincronización]**.

   ![](assets/salesforce-sync-settings-12.png)

1. Haga clic en la flecha situada junto a Sincronizar tareas/recordatorios de ventas de Marketo con [!DNL Salesforce] tareas.

   ![](assets/salesforce-sync-settings-13.png)

1. Elija la opción que desee (&quot;No sincronizar con [!DNL Salesforce] tareas&quot; está seleccionada de forma predeterminada).

   ![](assets/salesforce-sync-settings-14.png)

## Sincronizando [!DNL Sales Insight Actions] tareas con [!DNL Salesforce] por primera vez {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

La primera vez que active la sincronización entre [!DNL Sales Insight Actions] y [!DNL Salesforce] tareas, importaremos sus [!DNL Salesforce] tareas. No insertaremos ninguna tarea actual que usted tenga en [!DNL Sales Insight Actions] en [!DNL Salesforce]. Para reducir el desorden y los duplicados, las únicas tareas que se sincronizan de [!DNL Sales Insight Actions] a [!DNL Salesforce] son las que se crearon después de sincronizar [!DNL Sales Insight Actions] con SFDC.

Esto es lo que sucede cuando sincroniza [!DNL Sales Insight Actions] y tareas de SFDC:

Tan pronto como haga clic en guardar en las tareas que se sincronizan, comienzan a sincronizarse. Inicialmente, esto llevará algún tiempo.

Cualquier recordatorio que se haya actualizado o creado en las últimas 24 horas se recuperará de SFDC a [!DNL Sales Insight Actions]. La sincronización se basa en la fecha de vencimiento y todas esas tareas se sincronizarán en el back-end, pero en el Centro de comandos, solo verá las tareas con vencimiento hoy y mañana.

Si la sincronización se ha activado anteriormente y elimina cualquier tarea de SFDC, cualquier elemento que se haya eliminado en los últimos 15 días se eliminará del Centro de comandos.

Sincronizaremos constantemente tareas entre [!DNL Sales Insight Actions] y SFDC siempre y cuando la sincronización esté habilitada.

Después de la sincronización inicial, cualquier tarea que cree, edite, complete o elimine en [!DNL Sales Insight Actions] se sincronizará con su lista de tareas en [!DNL Salesforce]. Y todo lo que se cree, edite, complete o elimine en [!DNL Salesforce] actualizará su lista de tareas en [!DNL Sales Insight Actions].

Para activar esta sincronización, simplemente marca la casilla de sincronización en tu página de [!UICONTROL Configuración] en la aplicación web.
