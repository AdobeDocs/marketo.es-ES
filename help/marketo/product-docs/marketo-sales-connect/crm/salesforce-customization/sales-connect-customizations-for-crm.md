---
unique-page-id: 14745793
description: Personalizaciones de Sales Connect para CRM - Documentos de Marketo - Documentación del producto
title: Personalizaciones de Sales Connect para CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 1%

---

# Personalizaciones de Sales Connect para CRM {#sales-connect-customizations-for-crm}

La API de metadatos crea los campos y los botones siguientes en Salesforce CRM. Una vez creados los campos, los administradores deben configurar los diseños de página en su CRM para exponerlos. Se pueden encontrar las instrucciones [aquí](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Esto afecta tanto a los clientes de ToutApp como de Sales Connect.

## Cómo instalar personalizaciones en Salesforce {#how-to-install-customizations-in-salesforce}

1. En Sales Connect, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one.png)

1. En Configuración de administración, seleccione **Salesforce**.

   ![](assets/two.png)

1. Clic **Personalizaciones de Marketo Sales Connect**.

   ![](assets/three.png)

1. Clic **Conectar con Salesforce**.

   ![](assets/four.png)

1. Inicie sesión en Salesforce.

   ![](assets/five.png)

## Actualizar personalización de Salesforce {#update-salesforce-customization}

Las actualizaciones del paquete Personalización de Salesforce incluirán mejoras y correcciones de errores. Para comprobar si hay actualizaciones disponibles o realizar una actualización, siga los pasos a continuación.

>[!NOTE]
>
>**Permisos de administración necesarios.**

1. En el [aplicación web](https://www.toutapp.com), haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. En Configuración de administración, haga clic en **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. La tarjeta de personalización de Sales Connect le mostrará si hay actualizaciones disponibles. Clic **Actualizar personalizaciones**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Clic **Actualizar**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Espere a que se instalen las actualizaciones. Dependiendo de cuántos números de versión necesite, el tiempo de instalación variará.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Una vez completada, en la tarjeta se mostrará &quot;Las personalizaciones de Sales Connect están actualizadas&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campos de actividad personalizada {#custom-activity-fields}

Marketo detectará la creación de los nuevos campos y, a continuación, rellenará una vez los datos, volverá a asignar y realizará una sincronización continua de valores con **nuevo** solo campos de. Los campos antiguos no se actualizarán.

| **Nombre del campo** | **Descripción** |
|---|---|
| ID de presencia local de llamada MSE | Como usuario, puede elegir la presencia local como opción cuando realice llamadas desde el teléfono MSE. Las llamadas entrantes mostrarán un número local para el receptor. |
| URL de grabación de llamadas MSE | Las llamadas se pueden grabar y aquí se registrará un vínculo para la grabación. |
| Campaña MSE | Registra el nombre de la campaña de MSE a la que pertenece el contacto/posible cliente. |
| URL de campaña de MSE | Registra la URL de la campaña creada en MSE. Al hacer clic en esta opción, se abre la campaña en la aplicación web de MSE. |
| Etapa actual de la campaña de MSE | Si un contacto/posible cliente forma parte de una campaña, este campo registrará el nombre de la etapa en la que se encuentra actualmente el contacto/posible cliente. |
| Archivos adjuntos de correo electrónico MSE vistos | Registra datos cuando se envía un correo electrónico con un archivo adjunto y este lo ve el destinatario. |
| Correo electrónico MSE pulsado | Registra una marca de verificación cuando el destinatario hace clic en un vínculo de un correo electrónico. |
| Correo electrónico de MSE respondido | Registra una marca de verificación cuando el destinatario responde a un correo electrónico. |
| Estado de correo electrónico MSE | Muestra si un correo electrónico se envía/está en curso/se rechaza (el seguimiento de los correos electrónicos rechazados depende del canal de envío utilizado). |
| Plantilla de correo electrónico de MSE | Registra el nombre de la plantilla MSE que se utilizó en el correo electrónico enviado al posible cliente/contacto. |
| URL de plantilla de correo electrónico MSE | Registra la dirección URL de la plantilla creada en MSE. Al hacer clic en esta opción, se abrirá la plantilla en la aplicación web de MSE. |
| URL de correo electrónico MSE | Al hacer clic en esta URL, se abrirá el Centro de comandos en MSE y se abrirá la pestaña Historial de vista de detalles de personas, donde podrá ver el correo electrónico enviado. |
| Correo electrónico de MSE visto | Registra una marca de verificación cuando el destinatario ve un correo electrónico. |

## Campos de registro resumidos {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Nombre del campo</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>MSE: Última participación de marketing</td> 
   <td>Última participación entrante de Marketing. </td> 
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
   <td>MSE: último origen de participación de marketing</td> 
   <td>Origen de la participación de marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE: último tipo de participación de marketing</td> 
   <td colspan="1">Tipo de participación.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última actividad por ventas<br></td> 
   <td colspan="1">Última actividad saliente realizada por el equipo de ventas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última respuesta</td> 
   <td colspan="1">Última respuesta de correo electrónico al correo electrónico de ventas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campaña de ventas actual</td> 
   <td colspan="1">Registra el nombre de la campaña de MSE a la que pertenece el posible cliente/contacto.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE: Último acuerdo de ventas</td> 
   <td colspan="1">Último compromiso entrante de Ventas. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE: exclusión</td> 
   <td colspan="1">Campo de exclusión.</td> 
  </tr> 
 </tbody> 
</table>

## Botones {#buttons}

| **Nombre del botón** | **Descripción** |
|---|---|
| Enviar correo electrónico MSE | Envíe correos electrónicos de ventas desde Salesforce. |
| Añadir a campaña de MSE | Agregar a campañas MSE desde Salesforce. |
| Insertar en MSE | Contacto push de Salesforce a MSE. |
| Llamada con MSE | Realice llamadas de ventas desde Salesforce. |

## Botones de acción masiva {#bulk-action-buttons}

| **Nombre del botón** | **Descripción** |
|---|---|
| Añadir a campaña de MSE | Agregar a campañas MSE desde Salesforce. |
| Insertar en MSE | Contacto push de Salesforce a MSE. |

## Guías del usuario {#user-guides}

[Informes personalizados de MSE en Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE para Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE para Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
