---
unique-page-id: 18317669
description: Configuración de sincronización de Salesforce - Documentos de Marketo - Documentación del producto
title: Configuraciones de sincronización de Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 1%

---

# Configuraciones de sincronización de Salesforce {#salesforce-sync-settings}

## Registro de actividades de correo electrónico en Salesforce mediante API {#logging-email-activity-to-salesforce-via-api}

Esta funcionalidad requiere que esté en la edición Enterprise/Unlimited de Salesforce o en la edición Professional si ha adquirido Integration a través de la API de servicios web.

>[!PREREQUISITES]
>
>Salesforce y Sales Connect deben estar conectados.

1. En Sales Connect, haga clic en el icono del engranaje situado en la esquina superior derecha y seleccione **Configuración**.

   ![](assets/one-2.png)

1. En Mi cuenta (Configuración de administración si es administrador), haga clic en **Salesforce**.

   ![](assets/two-2.png)

1. Haga clic en **Configuración de sincronización** pestaña.

   ![](assets/three-1.png)

1. Haga clic en la flecha situada junto a Registrar actividad de correo electrónico en Salesforce.

   ![](assets/four-1.png)

1. Haga clic en **API de Salesforce** pestaña. En esta tarjeta puede configurar sus preferencias para registrar información en Salesforce. Clic **Guardar** cuando termine.

   ![](assets/five.png)

## Registro de actividades de correo electrónico en Salesforce por correo electrónico a Salesforce (CCO) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Una vez que active &quot;Email to Salesforce (BCC)&quot;, recibirá un CCO de sus correos electrónicos de ventas y sus correos electrónicos se registrarán como actividades en oportunidades, posibles clientes y contactos.

>[!PREREQUISITES]
>
>Salesforce y Sales Connect deben estar conectados.

**Para registrar los correos electrónicos en Salesforce por correo electrónico (CCO)**

1. En Sales Connect, haga clic en el icono del engranaje situado en la esquina superior derecha y seleccione **Configuración**.

   ![](assets/one-3.png)

1. En Mi cuenta (Configuración de administración si es administrador), haga clic en **Salesforce**.

   ![](assets/two-3.png)

1. Haga clic en **Configuración de sincronización** pestaña.

   ![](assets/three-1.png)

1. Haga clic en **Correo electrónico a Salesforce (CCO)** y haga clic en **Activar**.

   ![](assets/six-2.png)

Si, por alguna razón, su dirección de correo electrónico a Salesforce no se incorpora, siga estos pasos para activar la función CCO en su cuenta de Salesforce:

1. Inicie sesión en la instancia de Salesforce.
1. Busque su nombre de usuario en la esquina superior derecha y seleccione la barra desplegable.
1. Seleccionar **Mis configuraciones**.
1. Seleccionar **Correo electrónico**.
1. Seleccionar **Mi correo electrónico a Salesforce**.
1. En esta página, verá un campo denominado &quot;Enviar correo electrónico a la dirección de Salesforce&quot;. Si no hay nada rellenado junto a él, desplácese hacia abajo hasta &quot;Mis direcciones de correo electrónico aceptables&quot;.
1. Introduzca las direcciones de correo electrónico que desea incluir en la lista de destinatarios copiados ocultos (CCO).
1. Clic **Guardar cambios**.

**No se puede encontrar mi correo electrónico a Salesforce en Mi configuración**

Si no ve Mi correo electrónico a Salesforce en su Configuración, es posible que el administrador no lo haya habilitado. Esto puede suceder si su equipo es nuevo en Salesforce o si su equipo nunca ha utilizado la dirección de CCO que Salesforce proporciona.

>[!NOTE]
>
>Necesitará privilegios de administrador para configurar esto.

1. Clic **Configurar**.
1. Clic **Administración de correo electrónico**.
1. Clic **Correo electrónico a Salesforce**.
1. Clic **Editar**.
1. Marque la casilla junto a &quot;Activo&quot;.
1. Clic **Guardar**.

## Sincronizar tareas/recordatorios de Sales Connect con tareas de Salesforce {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Haga clic en el icono de engranaje en la esquina superior derecha y seleccione **Configuración**.

   ![](assets/one-3.png)

1. En Mi cuenta (Configuración de administración si es administrador), haga clic en **Salesforce**.

   ![](assets/two-2.png)

1. Haga clic en **Configuración de sincronización** pestaña.

   ![](assets/three-1.png)

1. Haga clic en la flecha situada junto a Sincronizar tareas/recordatorios de Sales Connect con tareas de Salesforce.

   ![](assets/seven-2.png)

1. Elija la opción que desee (&quot;No sincronizar con tareas de Salesforce&quot; está seleccionada de forma predeterminada).

   ![](assets/eight.png)
