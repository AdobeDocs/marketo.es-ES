---
unique-page-id: 4719304
description: Comprenda qué pasos del flujo de Salesforce déclencheur la sincronización automática de la persona con SFDC u otras acciones. Conozca las reglas para Agregar a Campaign, Cambiar propietario, Crear tarea y Convertir persona.
title: Acciones de Salesforce implícitas
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/lI3sRqk1if-UZ7DARSrGXXM485ZjZnlqDGb4si2wvi0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 163
ht-degree: 22%

---

# Acciones de Salesforce implícitas {#implied-salesforce-actions}

Cuando se ejecuta un paso de flujo específico de [!DNL Salesforce], a veces se realizan automáticamente pasos adicionales. Estas son las reglas, para que lo sepa:

Estas reglas se aplicarán cuando la persona no esté actualmente en [Salesforce.com](https://Salesforce.com){target="_blank"} como contacto o posible cliente.

<table>
 <thead>
  <tr>
   <th>Paso de flujo de Marketo</th>
   <th>Acción automática</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Agregar a campaña de SFDC</td>
   <td>Sincronizar persona con SFDC</td>
  </tr>
  <tr>
   <td>Cambiar estado de la campaña SFDC</td>
   <td>Sincronizar persona con SFDC<br>Agregar a SFDC Campaign</td>
  </tr>
  <tr>
   <td>Cambiar propietario</td>
   <td><p>Sincronizar persona con SFDC</p></td>
  </tr>
  <tr>
   <td>Convertir persona</td>
   <td><p>Sincronizar persona con SFDC</p></td>
  </tr>
  <tr>
   <td>Crear tarea</td>
   <td>Sincronizar persona con SFDC</td>
  </tr>
 </tbody>
</table>

Puede filtrar los registros de SFDC en una lista inteligente usando el filtro **[!UICONTROL SFDC Type]** con el operador establecido en &quot;[!UICONTROL no está vacío]&quot;. Todos los registros de SFDC tienen un valor en este campo.

Recuerde, estas acciones automáticas solo ocurren si el posible cliente no se encuentra actualmente en [Salesforce.com](https://salesforce.com){target="_blank"}
