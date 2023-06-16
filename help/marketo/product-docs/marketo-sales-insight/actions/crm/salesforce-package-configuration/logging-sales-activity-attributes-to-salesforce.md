---
description: Registro de atributos de actividad de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Registro de atributos de actividad de ventas en Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 6%

---

# Registro de atributos de actividad de ventas en Salesforce {#logging-sales-activity-attributes-to-salesforce}

El administrador de Salesforce puede agregar manualmente campos de actividad personalizados a Salesforce.

1. En su cuenta de Salesforce, haga clic en **Configurar**.

1. Busque &quot;Campos personalizados de actividad&quot; en el campo de búsqueda rápida y haga clic en él.

1. Clic **Nuevo**.

1. Seleccione el Tipo de datos correspondiente al campo que desee añadir en función de la tabla siguiente y haga clic en **Siguiente**.

1. Introduzca el Nombre de campo y la etiqueta correspondientes al campo que desea añadir.

Descripción de cada columna de la siguiente tabla:

* **Etiqueta de campo**: Nombre de campo que se muestra en la interfaz de usuario (este nombre se puede personalizar para mejorar la legibilidad por parte de su equipo)
* **Nombre de campo**: Nombre técnico del campo (asegúrese de que el Nombre de campo introducido coincida con el Nombre de campo de la tabla siguiente)
* **Nombre de API**: Nombre técnico del campo para API (asegúrese de que el nombre de API que introduzca coincida con el nombre de API de la tabla siguiente)
* **Tipo de datos**: Tipo de campo
* **Tamaño**: tamaño del campo de texto

<table>
 <tr>
  <th>Etiqueta de campo</th>
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
  <td>ID de presencia local de llamada de ventas de Marketo</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de grabación de llamada de ventas de Marketo</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campaña de ventas de Marketo</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Etapa actual de Marketo Sales Campaign</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de campaña de ventas de Marketo</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo Sales Email Attachment Visto</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Casilla</td>
  <td></td>
 </tr>
 <tr>
  <td>Correo electrónico de ventas de Marketo pulsado</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Casilla</td>
  <td></td>
 </tr>
 <tr>
  <td>Correo electrónico de ventas de Marketo respondido</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Casilla</td>
  <td></td>
 </tr>
 <tr>
  <td>Estado de correo electrónico de ventas de Marketo</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texto</td>
  <td></td>
 </tr>
 <tr>
  <td>Plantilla de correo electrónico de ventas de Marketo</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de plantilla de correo electrónico de ventas de Marketo</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL de correo electrónico de ventas de Marketo</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Correo electrónico de ventas de Marketo visto</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Casilla</td>
  <td></td>
 </tr>
</table>
