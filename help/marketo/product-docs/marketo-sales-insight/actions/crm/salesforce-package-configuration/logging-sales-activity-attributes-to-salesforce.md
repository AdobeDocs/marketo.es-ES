---
description: Registro de atributos de actividad de ventas en Salesforce - Documentos de Marketo - Documentación del producto
title: Registro de atributos de actividad de ventas en Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 10%

---

# Registrando atributos de actividad de ventas en [!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

El administrador de Salesforce puede agregar manualmente campos de actividad personalizados a [!DNL Salesforce].

1. En su cuenta de [!DNL Salesforce], haga clic en **[!UICONTROL Configurar]**.

1. Busque &quot;Campos personalizados de actividad&quot; en el campo de búsqueda rápida y haga clic en él.

1. Haga clic en **[!UICONTROL Nuevo]**.

1. Seleccione el tipo de datos correspondiente al campo que desee agregar según la tabla siguiente y haga clic en **[!UICONTROL Siguiente]**.

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
  <td>[!UICONTROL Call Outcomes]</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Razones de llamada]</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Local Presence ID]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL de grabación de llamada de ventas de Marketo]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign Current Step]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL de campaña de ventas de Marketo]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Attachment Visto]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Clicked]</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Correo electrónico de ventas de Marketo respondido]</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Estado de correo electrónico de ventas Marketo]</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texto</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Plantilla de correo electrónico de ventas de Marketo]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL de plantilla de correo electrónico de ventas de Marketo]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email URL]</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Visto]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Casilla de verificación</td>
  <td></td>
 </tr>
</table>
