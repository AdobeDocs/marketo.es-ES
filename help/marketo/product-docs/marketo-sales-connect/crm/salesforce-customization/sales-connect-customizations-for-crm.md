---
unique-page-id: 14745793
description: Personalizaciones de Sales Connect para CRM - Documentos de marketing - Documentación del producto
title: Personalizaciones de Sales Connect para CRM
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---


# Personalizaciones de Sales Connect para CRM {#sales-connect-customizations-for-crm}

Los campos y botones siguientes son creados por la API de metadatos en Salesforce CRM. Una vez creados los campos, los administradores deben configurar los diseños de página en su CRM para exponerlos. Las instrucciones se pueden encontrar [aquí](https://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Esto afecta tanto a los clientes de ToutApp como a los de Sales Connect.

## Cómo instalar personalizaciones en Salesforce {#how-to-install-customizations-in-salesforce}

1. En Sales Connect, haga clic en el icono de engranaje y seleccione **Configuración**.

   ![](assets/one.png)

1. En Configuración de administración, seleccione **Salesforce**.

   ![](assets/two.png)

1. Haga clic en **Personalizaciones de Connect de Marketing para ventas**.

   ![](assets/three.png)

1. Haga clic en **Conectar a Salesforce**.

   ![](assets/four.png)

1. Inicie sesión en Salesforce.

   ![](assets/five.png)

## Campos de Actividad personalizados {#custom-activity-fields}

Marketo detectará la creación de los nuevos campos y, a continuación, realizará un relleno único de datos, una reasignación y una sincronización continua de valores únicamente en los campos **new**. Los campos antiguos no se actualizarán.

| **Nombre del campo** | **Descripción** |
|---|---|
| ID de presencia local de llamada MSE | Como usuario, puede elegir Presencia local como opción cuando realiza llamadas desde el teléfono MSE. Las llamadas entrantes mostrarán un número local para el receptor. |
| URL de registro de llamadas MSE | Las llamadas se pueden grabar y se registrará un vínculo para la grabación aquí. |
| Campaña MSE | Registra el nombre de la campaña MSE de la que es miembro el contacto/posible cliente. |
| URL de Campaña de MSE | Registra la dirección URL de la campaña creada en MSE. Al hacer clic en esto, se abrirá la campaña en la aplicación web MSE. |
| Etapa actual de Campaña de MSE | Si un contacto/posible cliente forma parte de una campaña, este campo registrará el nombre del paso en el que se encuentra el contacto/posible cliente. |
| Datos adjuntos de correo electrónico de MSE vistos | Registra los datos cuando se envía un correo electrónico con un archivo adjunto y el destinatario lo ve. |
| Se hizo clic en el mensaje de correo electrónico de MSE | Registra una marca de verificación cuando el destinatario hace clic en un vínculo de un correo electrónico. |
| Mensaje de correo electrónico MSE respondido | Registra una marca de verificación cuando el destinatario responde a un mensaje de correo electrónico. |
| Estado de correo electrónico de MSE | Muestra si se envía/está en curso/se devuelve un mensaje de correo electrónico (el seguimiento de los mensajes devueltos depende del canal de envío utilizado). |
| Plantilla de correo electrónico de MSE | Registra el nombre de la plantilla MSE que se utilizó en el correo electrónico enviado al posible cliente o contacto. |
| URL de plantilla de correo electrónico de MSE | Registra la dirección URL de la plantilla que se creó en MSE. Al hacer clic en esto, se abrirá la plantilla en la aplicación web de MSE. |
| URL de correo electrónico de MSE | Al hacer clic en esta URL se abrirá el Centro de comandos en MSE y se abrirá la ficha Historial de Vistas de detalles de personas, donde podrá ver el correo electrónico enviado. |
| Correo electrónico de MSE visualizado | Registra una marca de verificación cuando el destinatario vista un correo electrónico. |

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
   <td>MSE - Última participación de mercadotecnia</td> 
   <td>Última participación entrante de Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Última fecha de compromiso de mercadotecnia</td> 
   <td>Marca de hora de participación de Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Último desfase de compromiso de mercadotecnia</td> 
   <td>Descripción del compromiso.</td> 
  </tr> 
  <tr> 
   <td>MSE - Última fuente de compromiso de mercadotecnia</td> 
   <td>Fuente de participación de Marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último tipo de compromiso de mercadotecnia</td> 
   <td colspan="1">Tipo de compromiso.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última Actividad por ventas<br></td> 
   <td colspan="1">Última actividad saliente realizada por el equipo de ventas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última respuesta</td> 
   <td colspan="1">Última respuesta de correo electrónico al correo electrónico de ventas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campaña de ventas actual</td> 
   <td colspan="1">Registra el nombre de la campaña de MSE de la que es miembro el cliente/contacto.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última participación de ventas</td> 
   <td colspan="1">Última participación entrante de Ventas. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Exclusión</td> 
   <td colspan="1">Campo de exclusión.</td> 
  </tr> 
 </tbody> 
</table>

## Botones {#buttons}

| **Nombre del botón** | **Descripción** |
|---|---|
| Enviar correo electrónico MSE | Enviar correos electrónicos de ventas desde Salesforce. |
| Añadir a la Campaña de MSE | Añada a campañas MSE de Salesforce. |
| Insertar en MSE | Insertar contacto de Salesforce en MSE. |
| Llamar a MSE | Realizar llamadas de ventas desde Salesforce. |

## Botones de acción masiva {#bulk-action-buttons}

| **Nombre del botón** | **Descripción** |
|---|---|
| Añadir a la Campaña de MSE | Añada a campañas MSE de Salesforce. |
| Insertar en MSE | Insertar contacto de Salesforce en MSE. |

## Guías del usuario {#user-guides}

[Informes personalizados de MSE en Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE para Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE para Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
