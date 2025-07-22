---
unique-page-id: 18317669
description: Configuración de sincronización de Salesforce - Documentos de Marketo - Documentación del producto
title: Configuraciones de sincronización de Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 2%

---

# Configuraciones de sincronización de Salesforce {#salesforce-sync-settings}

## Registro de actividades de correo electrónico en Salesforce mediante API {#logging-email-activity-to-salesforce-via-api}

Esta funcionalidad requiere que esté en la edición Enterprise/Unlimited de Salesforce o en la edición Professional si ha adquirido Integration mediante la API de servicios web.

>[!PREREQUISITES]
>
>Salesforce y Sales Connect deben estar conectados.

1. En [!DNL Sales Connect], haga clic en el icono de engranaje en la esquina superior derecha y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one-2.png)

1. En [!UICONTROL Mi cuenta] ([!UICONTROL Configuración de administración] si eres administrador), haz clic en **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de sincronización]**.

   ![](assets/three-1.png)

1. Haga clic en la flecha situada junto a Registrar actividad de correo electrónico en [!DNL Salesforce].

   ![](assets/four-1.png)

1. Haga clic en la ficha **[!UICONTROL API de Salesforce]**. En esta tarjeta puede configurar su preferencia para registrar información en [!DNL Salesforce]. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/five.png)

## Registro de actividades de correo electrónico en Salesforce mediante correo electrónico a Salesforce (CCO) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Una vez que active &quot;Email to Salesforce (BCC)&quot;, recibirá un CCO de sus correos electrónicos de ventas y sus correos electrónicos se registrarán como actividades en oportunidades, posibles clientes y contactos.

>[!PREREQUISITES]
>
>[!DNL Salesforce] y [!DNL Sales Connect] deben estar conectados.

**Para registrar sus correos electrónicos en Salesforce por correo electrónico (CCO)**

1. En [!UICONTROL Conexión de ventas], haga clic en el icono de engranaje en la esquina superior derecha y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one-3.png)

1. En [!UICONTROL Mi cuenta] ([!UICONTROL Configuración de administración] si eres administrador), haz clic en **[!UICONTROL Salesforce]**.

   ![](assets/two-3.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de sincronización]**.

   ![](assets/three-1.png)

1. Haga clic en la ficha **[!UICONTROL Correo electrónico a Salesforce (CCO)]** y luego en **[!UICONTROL Activar]**.

   ![](assets/six-2.png)

Si, por alguna razón, el correo electrónico a la dirección [!DNL Salesforce] no se extrae, siga estos pasos para activar la función CCO en su cuenta de [!DNL Salesforce]:

1. Inicie sesión en su instancia de [!DNL Salesforce].
1. Busque su nombre de usuario en la esquina superior derecha y seleccione la barra desplegable.
1. Seleccione **[!UICONTROL Mi configuración]**.
1. Seleccione **[!UICONTROL Correo electrónico]**.
1. Seleccione **[!UICONTROL Mi correo electrónico a Salesforce]**.
1. En esta página, verá un campo etiquetado como &quot;Correo electrónico a dirección de Salesforce&quot;. Si no hay nada rellenado junto a él, desplácese hacia abajo hasta &quot;Mis direcciones de correo electrónico aceptables&quot;.
1. Introduzca las direcciones de correo electrónico que desea incluir en la lista de destinatarios copiados ocultos (CCO).
1. Haga clic en **[!UICONTROL Guardar cambios]**.

**No puedo encontrar mi correo electrónico a [!DNL Salesforce] en Mi configuración**

Si no ve Mi correo electrónico a Salesforce en su configuración, es posible que el administrador no lo haya habilitado. Esto puede suceder si su equipo es nuevo en [!DNL Salesforce] o si su equipo nunca ha usado la dirección de CCO que [!DNL Salesforce] proporciona.

>[!NOTE]
>
>Necesitará privilegios de administrador para configurar esto.

1. Haga clic en **[!UICONTROL Configuración]**.
1. Haga clic en **[!UICONTROL Administración de correo electrónico]**.
1. Haga clic en **[!UICONTROL Correo electrónico a Salesforce]**.
1. Haga clic en **[!UICONTROL Editar]**.
1. Marque la casilla junto a &quot;[!UICONTROL Activo]&quot;.
1. Haga clic en **[!UICONTROL Guardar]**.

## Sincronizar tareas/recordatorios de conexión de ventas con [!DNL Salesforce] tareas {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Haga clic en el icono de engranaje en la esquina superior derecha y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one-3.png)

1. En [!UICONTROL Mi cuenta] ([!UICONTROL Configuración de administración] si eres administrador), haz clic en **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de sincronización]**.

   ![](assets/three-1.png)

1. Haga clic en la flecha situada junto a [!UICONTROL Sincronizar tareas/recordatorios de participación de ventas con tareas de Salesforce].

   ![](assets/seven-2.png)

1. Elija la opción que desee (&quot;[!UICONTROL No sincronizar con tareas de Salesforce]&quot; está seleccionada de forma predeterminada).

   ![](assets/eight.png)
