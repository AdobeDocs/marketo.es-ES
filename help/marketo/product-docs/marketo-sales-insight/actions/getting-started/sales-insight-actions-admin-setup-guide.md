---
description: Guía de configuración de administración de acciones de ventas de Insight - Documentos de Marketo - Documentación del producto
title: Guía de configuración de administración de acciones de Sales Insight
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 4%

---

# Guía de configuración de administración de acciones de Sales Insight {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions es una aplicación basada en la Web que se integra exclusivamente con Salesforce CRM mediante el [paquete Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. A veces se denomina &quot;Ventas Marketo&quot; o simplemente &quot;Acciones&quot;.

>[!PREREQUISITES]
>
>* Confirme con el equipo de cuenta de Adobe (su administrador de cuentas) que las acciones MSI se han habilitado para su cuenta de Marketo Engage (si no tiene un administrador de cuentas, póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
>* La sincronización de Marketo/Salesforce debe estar configurada.

<table>
 <tr>
  <th>Persona</th>
  <th>Paso</th>
 </tr>
 <tr>
  <td>Admin. de Marketo</td>
  <td>Configurar la cuenta de ventas de Marketo</td>
 </tr>
 <tr>
  <td>Administrador de Marketo o administrador de <br/>[!DNL Salesforce]</td>
  <td>Conectar la cuenta de ventas de Marketo a [!DNL Salesforce]</td>
 </tr>
 <tr>
  <td>Admin. de Marketo</td>
  <td>Conectar la cuenta de ventas de Marketo a Marketo</td>
 </tr>
 <tr>
  <td>Admin. de Marketo</td>
  <td>Iniciar sincronización de datos de Marketo a la cuenta de ventas de Marketo</td>
 </tr>
 <tr>
  <td>Admin. de Marketo</td>
  <td>Invitar a usuarios a MSI-Actions</td>
 </tr>
 <tr>
  <td>[!DNL Salesforce] Administrador</td>
  <td>Instalación/actualización del paquete MSI en [!DNL Salesforce]</td>
 </tr>
 <tr>
  <td>[!DNL Salesforce] Administrador</td>
  <td>Configurar acciones MSI en [!DNL Salesforce]</td>
 </tr>
</table>

## Configurar la cuenta de ventas de Marketo {#set-up-marketo-sales-account}

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Si no ve un ID de cliente y un Secreto de cliente en la tarjeta de información de integración, active la instancia de acciones invitando al primer usuario y verá aparecer el ID de cliente y el Secreto de cliente.

1. Haga clic en **Sales Insight** y luego en **Actions Config**. Seleccione de una lista de administradores de Marketo para invitar y haga clic en **Enviar invitación**.

   ![](assets/msi-actions-admin-guide-2.png)

El usuario recibirá un correo electrónico con los pasos para obtener acceso a la cuenta.

>[!NOTE]
>
>Los usuarios adicionales no se añadirán a través de Marketo y, en su lugar, se añadirán a través de la página de Administración de usuarios de la cuenta de ventas. [Haga clic aquí](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} para obtener más información sobre cómo agregar usuarios adicionales.

## Conectar la cuenta de ventas de Marketo a [!DNL Salesforce] {#connect-marketo-sales-account-to-salesforce}

1. En tu cuenta de ventas de Marketo, haz clic en el icono del engranaje y selecciona **[!UICONTROL Configuración]**.

   ![](assets/msi-actions-admin-guide-3.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL Salesforce]**.

   ![](assets/msi-actions-admin-guide-4.png)

1. En la ficha [!UICONTROL Conexiones y personalizaciones], haga clic en **[!UICONTROL Conectar]**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/msi-actions-admin-guide-6.png)

Si ya ha iniciado sesión en Salesforce, estará conectado. Si no lo está, se le pedirá que inicie sesión.

## Conectar Marketo a su cuenta de aplicaciones de ventas {#connect-marketo-to-your-sales-apps-account}

1. En tu cuenta de ventas de Marketo, haz clic en el icono del engranaje y selecciona **[!UICONTROL Configuración]**.

   ![](assets/msi-actions-admin-guide-7.png)

1. En [!UICONTROL Configuración de administración], haga clic en **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Haga clic en **[!UICONTROL conectar]**. La cuenta se conectará a continuación.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Si no se conecta, copie las credenciales de la pestaña &quot;Configuración de acciones&quot; de Marketo Sales Insight y péguelas en la pestaña Configuración.

## Iniciar sincronización de datos {#initiate-data-sync}

La sincronización de campos de unificación de datos para las acciones de Sales Insight permite al sistema extraer información sobre las personas de la base de datos de Marketo Engage en la base de datos de acciones de Sales Insight, mantener actualizados los datos de las personas y garantizar que las actividades se registren en los registros correctos en Marketo y [!DNL Salesforce].

>[!CAUTION]
>
>Una vez iniciada la sincronización de datos, debería **no** eliminar el usuario original de su instancia de Sales Insight Actions. Este es el usuario al que se envió la primera invitación.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Haga clic en **[!UICONTROL Insight de ventas]**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Haga clic en la ficha **[!UICONTROL Configuración de acciones]**. En la tarjeta Sincronizar campos de acción, haga clic en **[!UICONTROL Sincronizar]**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Verá una vista previa de los campos que se sincronizarán. Haga clic en **[!UICONTROL Iniciar sincronización]**.

   ![](assets/msi-actions-admin-guide-13.png)

Los registros de persona que existen en Marketo y [!DNL Salesforce] se sincronizarán con su cuenta de Marketo Sales Apps.

>[!NOTE]
>
>Para obtener más información sobre cómo los datos de personas y actividades se sincronizan entre las acciones de Sales Insight, Marketo y Salesforce, [haga clic aquí](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Invitar usuarios individuales a acciones de MSI {#invite-individual-users-to-msi-actions}

1. En tu cuenta de ventas de Marketo, haz clic en el icono del engranaje y selecciona **[!UICONTROL Configuración]**.

   ![](assets/msi-actions-admin-guide-14.png)

1. En [!UICONTROL Configuración de administración], seleccione **[!UICONTROL Administración de usuarios]**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Haga clic en **[!UICONTROL Acciones]** y seleccione **[!UICONTROL Invitar usuarios]**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Escriba las direcciones de correo electrónico y haga clic en **[!UICONTROL Invitar]**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>De forma predeterminada, todos los miembros nuevos se agregarán al equipo Todos.

Recibirá un mensaje de confirmación.

## Invitar a usuarios mediante CSV a acciones MSI {#invite-users-via-csv-to-msi-actions}

1. En tu cuenta de ventas de Marketo, haz clic en el icono del engranaje y selecciona **[!UICONTROL Configuración]**.

   ![](assets/msi-actions-admin-guide-18.png)

1. En [!UICONTROL Configuración de administración], seleccione **[!UICONTROL Administración de usuarios]**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Haga clic en **[!UICONTROL Acciones]** y seleccione **[!UICONTROL Invitar usuarios mediante CSV]**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Busque el archivo CSV en el equipo, selecciónelo y haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Confirme que los campos estén asignados correctamente y haga clic en **[!UICONTROL Invitar]**.

   ![](assets/msi-actions-admin-guide-22.png)

Recibirá un mensaje de confirmación una vez que se envíen las invitaciones.

>[!NOTE]
>
>Una vez hecho esto, puede actualizar su paquete MSI existente o instalar uno nuevo y pasar a [configurar acciones MSI en Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
