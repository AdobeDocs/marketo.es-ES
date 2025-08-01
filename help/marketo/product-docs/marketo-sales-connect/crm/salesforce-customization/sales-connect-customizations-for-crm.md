---
unique-page-id: 14745793
description: '[!DNL Sales Connect] personalizaciones para CRM - Documentos de Marketo - Documentación del producto'
title: '[!DNL Sales Connect] personalizaciones para CRM'
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 2%

---

# [!DNL Sales Connect] personalizaciones para CRM {#sales-connect-customizations-for-crm}

La API de metadatos crea los campos y los botones siguientes en Salesforce CRM. Una vez creados los campos, los administradores deben configurar los diseños de página en su CRM para exponerlos. Las instrucciones [se pueden encontrar aquí](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Cómo instalar personalizaciones en [!DNL Salesforce] {#how-to-install-customizations-in-salesforce}

1. En [!DNL Sales Connect], haga clic en el icono del engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/one.png)

1. En [!UICONTROL Configuración de administración], seleccione **[!UICONTROL Salesforce]**.

   ![](assets/two.png)

1. Haga clic en **[!UICONTROL Personalizaciones de Marketo Sales Engage]**.

   ![](assets/three.png)

1. Haga clic en **[!UICONTROL Conectarse a Salesforce]**.

   ![](assets/four.png)

1. Iniciar sesión en [!DNL Salesforce].

   ![](assets/five.png)

## Actualizar personalización de [!DNL Salesforce] {#update-salesforce-customization}

Las actualizaciones del paquete de personalización de [!DNL Salesforce] incluirán mejoras y correcciones de errores. Para comprobar si hay actualizaciones disponibles o realizar una actualización, siga los pasos a continuación.

>[!NOTE]
>
>Se requieren **permisos de administración.**

1. En la [aplicación web](https://www.toutapp.com), haga clic en el icono de engranaje y seleccione **[!UICONTROL Configuración]**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. En [!UICONTROL Configuración de administración], haga clic en **[!UICONTROL Salesforce]**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. La tarjeta de personalización [!DNL Sales Connect] mostrará si hay actualizaciones disponibles. Haga clic en **[!UICONTROL Actualizar personalizaciones]**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Haga clic en **[!UICONTROL Actualizar]**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Espere a que se instalen las actualizaciones. Dependiendo de cuántos números de versión necesite, el tiempo de instalación variará.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Una vez completada, en la tarjeta se mostrará &quot;Las personalizaciones de Sales Connect están actualizadas&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campos de actividad personalizada {#custom-activity-fields}

Marketo detectará la creación de los nuevos campos y realizará un relleno único de datos, una reasignación y una sincronización continua de valores solo en los **nuevos** campos. Los campos antiguos no se actualizarán.

<table><thead>
  <tr>
    <th>Nombre del campo</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ID de presencia local de llamada MSE</td>
    <td>Como usuario, puede elegir la presencia local como opción cuando realice llamadas desde el teléfono MSE. Las llamadas entrantes mostrarán un número local para el receptor.</td>
  </tr>
  <tr>
    <td>URL de grabación de llamadas MSE</td>
    <td>Las llamadas se pueden grabar y aquí se registrará un vínculo para la grabación.</td>
  </tr>
  <tr>
    <td>Campaña MSE</td>
    <td>Registra el nombre de la campaña de MSE a la que pertenece el contacto/posible cliente.</td>
  </tr>
  <tr>
    <td>URL de campaña de MSE</td>
    <td>Registra la URL de la campaña creada en MSE. Al hacer clic en esta opción, se abre la campaña en la aplicación web de MSE.</td>
  </tr>
  <tr>
    <td>Etapa actual de la campaña de MSE</td>
    <td>Si un contacto/posible cliente forma parte de una campaña, este campo registrará el nombre de la etapa en la que se encuentra actualmente el contacto/posible cliente.</td>
  </tr>
  <tr>
    <td>Archivos adjuntos de correo electrónico MSE vistos</td>
    <td>Registra datos cuando se envía un correo electrónico con un archivo adjunto y este lo ve el destinatario.</td>
  </tr>
  <tr>
    <td>Correo electrónico MSE pulsado</td>
    <td>Registra una marca de verificación cuando el destinatario hace clic en un vínculo de un correo electrónico.</td>
  </tr>
  <tr>
    <td>Correo electrónico de MSE respondido</td>
    <td>Registra una marca de verificación cuando el destinatario responde a un correo electrónico.</td>
  </tr>
  <tr>
    <td>Estado de correo electrónico MSE</td>
    <td>Muestra si un correo electrónico se envía/está en curso/se rechaza (el seguimiento de los correos electrónicos rechazados depende del canal de envío utilizado).</td>
  </tr>
  <tr>
    <td>Plantilla de correo electrónico de MSE</td>
    <td>Registra el nombre de la plantilla MSE que se utilizó en el correo electrónico enviado al posible cliente/contacto.</td>
  </tr>
  <tr>
    <td>URL de plantilla de correo electrónico MSE</td>
    <td>Registra la dirección URL de la plantilla creada en MSE. Al hacer clic en esta opción, se abrirá la plantilla en la aplicación web de MSE.</td>
  </tr>
  <tr>
    <td>URL de correo electrónico MSE</td>
    <td>Al hacer clic en esta URL, se abrirá el Centro de comandos en MSE y se abrirá la pestaña Historial de vista de detalles de personas, donde podrá ver el correo electrónico enviado.</td>
  </tr>
  <tr>
    <td>Correo electrónico de MSE visto</td>
    <td>Registra una marca de verificación cuando el destinatario ve un correo electrónico.</td>
  </tr>
</tbody></table>

## Campos de registro resumidos {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Nombre del campo</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE: Última participación de marketing</td>
    <td>Última participación entrante de Marketing.</td>
  </tr>
  <tr>
    <td>MSE - Fecha de la última participación en marketing</td>
    <td>Marca de tiempo de la participación del departamento de marketing.</td>
  </tr>
  <tr>
    <td>MSE: Última descripción de la participación de marketing</td>
    <td>Descripción de la participación.</td>
  </tr>
  <tr>
    <td>MSE: Último Source de participación de marketing</td>
    <td>Participación de Source of Marketing.</td>
  </tr>
  <tr>
    <td>MSE: último tipo de participación de marketing</td>
    <td>Tipo de participación.</td>
  </tr>
  <tr>
    <td>MSE - Última actividad por ventas</td>
    <td>Última actividad saliente realizada por el equipo de ventas.</td>
  </tr>
  <tr>
    <td>MSE - Última respuesta</td>
    <td>Última respuesta de correo electrónico al correo electrónico de ventas.</td>
  </tr>
  <tr>
    <td>MSE - Campaña de ventas actual</td>
    <td>Registra el nombre de la campaña de MSE a la que pertenece el posible cliente/contacto.</td>
  </tr>
  <tr>
    <td>MSE: Último acuerdo de ventas</td>
    <td>Último compromiso entrante de Ventas.</td>
  </tr>
  <tr>
    <td>MSE: exclusión</td>
    <td>Campo de exclusión.</td>
  </tr>
</tbody></table>

## Botones {#buttons}

<table><thead>
  <tr>
    <th>Nombre del botón</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Enviar correo electrónico MSE</td>
    <td>Envíe correos electrónicos de ventas desde Salesforce.</td>
  </tr>
  <tr>
    <td>Añadir a campaña de MSE</td>
    <td>Agregar a campañas MSE desde Salesforce.</td>
  </tr>
  <tr>
    <td>Insertar en MSE</td>
    <td>Contacto push de Salesforce a MSE.</td>
  </tr>
  <tr>
    <td>Llamada con MSE</td>
    <td>Realice llamadas de ventas desde Salesforce.</td>
  </tr>
</tbody>
</table>

## Botones de acción masiva {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Nombre del botón</th>
    <th>Descripción</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Añadir a campaña de MSE</td>
    <td>Agregar a campañas MSE desde Salesforce.</td>
  </tr>
  <tr>
    <td>Insertar en MSE</td>
    <td>Contacto push de Salesforce a MSE.</td>
  </tr>
</tbody>
</table>

## Guías del usuario {#user-guides}

[Informes personalizados de MSE en Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE para Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE para Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
