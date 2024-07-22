---
description: Registro de atributos de actividad de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Registro de atributos de actividad de ventas en Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 29%

---

# Registro de atributos de actividad de ventas en Salesforce {#logging-sales-activity-attributes-to-salesforce}

El administrador de Salesforce puede agregar manualmente campos de actividad personalizados a Salesforce.

1. En su cuenta de Salesforce, haga clic en **Configurar**.

1. Busque &quot;Campos personalizados de actividad&quot; en el campo de búsqueda rápida y haga clic en él.

1. Haga clic en **Nuevo**.

1. Seleccione el tipo de datos correspondiente al campo que desee agregar según la tabla siguiente y haga clic en **Siguiente**.

1. Introduzca el Nombre de campo y la etiqueta correspondientes al campo que desea añadir.

Descripción de cada columna de la siguiente tabla:

* **Etiqueta de campo**: nombre de campo mostrado en la interfaz de usuario (este nombre se puede personalizar para mejorar la legibilidad por su equipo)
* **Nombre de campo**: Nombre técnico del campo (asegúrese de que el Nombre de campo que escriba coincida con el Nombre de campo de la tabla siguiente)
* **Nombre de API**: Nombre técnico del campo de API (asegúrese de que el nombre de API que escriba coincida con el nombre de API de la tabla siguiente)
* **Tipo de datos**: Tipo de campo
* **Tamaño**: tamaño del campo de texto

<table>
 <tr>
  <th>Etiqueta del campo</th>
  <th>Nombre del campo</th>
  <th>Nombre de API</th>
  <th>Tipo de datos</th>
  <th>Tamaño</th>
 </tr>
  <tr>
  <td>Resultados de llamadas</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Razones de llamada</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Identificación de presencia local de la llamada de Marketo Sales</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de la grabación de la llamada de Marketo Sales</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campaña de Marketo Sales</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Paso actual de la campaña de Marketo Sales</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de la campaña de Marketo Sales</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Archivo adjunto visto del email de Marketo Sales</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>Email de Marketo Sales en el que se hizo clic</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>Email de Marketo Sales respondido</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>Estado del email de Marketo Sales</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texto</td>
  <td></td>
 </tr>
 <tr>
  <td>Plantilla de email de Marketo Sales</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de la plantilla de email de Marketo Sales</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL del email de Marketo Sales</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Email de Marketo Sales visto</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
</table>
