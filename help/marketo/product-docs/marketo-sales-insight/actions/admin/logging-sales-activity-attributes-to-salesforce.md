---
description: Registro de atributos de actividad de ventas en Salesforce - Marketo Docs - Documentación del producto
title: Registro de atributos de actividad de ventas en Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 3%

---

# Registro de atributos de actividad de ventas en Salesforce {#logging-sales-activity-attributes-to-salesforce}

El administrador de Salesforce puede agregar manualmente campos de actividad personalizados a Salesforce.

1. En la cuenta de Salesforce, haga clic en **Configuración**.

1. Busque &quot;Campos personalizados de actividad&quot; en el campo de búsqueda rápida y haga clic en él.

1. Haga clic en **Nuevo**.

1. Seleccione Tipo de datos correspondiente al campo que desea añadir en función de la siguiente tabla y haga clic en **Siguiente**.

1. Introduzca el Nombre de campo y la etiqueta correspondientes al campo que desea añadir.

Descripción de cada columna de la tabla siguiente:

* **Etiqueta de campo**: Nombre de campo que se muestra en la interfaz de usuario (este nombre se puede personalizar para mejorar la legibilidad de su equipo)
* **Nombre del campo**: Nombre técnico del campo (asegúrese de que el Nombre de campo que ha introducido coincide con el Nombre de campo de la tabla siguiente)
* **Nombre de API**: Nombre técnico del campo para API (asegúrese de que el nombre de API que ha introducido coincide con el nombre de la API que aparece en la siguiente tabla)
* **Tipo de datos**: Tipo de campo
* **Tamaño**: Tamaño del campo de texto

<table>
 <tr>
  <th>Etiqueta de campo</th>
  <th>Nombre del campo</th>
  <th>Nombre de API</th>
  <th>Tipo de datos</th>
  <th>Tamaño</th>
 </tr>
 <tr>
  <td>ID de presencia local de llamada de venta de Marketo</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de registro de llamada de venta de Marketo</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campaña de ventas de Marketo</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Paso actual de la campaña de ventas de Marketo</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de campaña de ventas de Marketo</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Archivo adjunto de correo electrónico de ventas de Marketo visto</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed_c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>Correo electrónico de ventas de Marketo en el que se hizo clic</td>
  <td>MSE_Clicks</td>
  <td>MSE_Clicked_c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>Correo electrónico de ventas de Marketo respondido</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>Estado del correo electrónico de ventas de Marketo</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texto</td>
  <td></td>
 </tr>
 <tr>
  <td>Plantilla de correo electrónico de ventas de Marketo</td>
  <td>MSE_Template</td>
  <td>MSE_Template_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de la plantilla de correo electrónico de ventas de Marketo</td>
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
  <td>MSE_Viewed_c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
</table>
