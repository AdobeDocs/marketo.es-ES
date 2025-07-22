---
unique-page-id: 4719304
description: 'Acciones de Salesforce implícitas: documentos de Marketo, documentación del producto'
title: Acciones de Salesforce implícitas
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 21%

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
   <td>Agregar a Campaña de SFDC</td> 
   <td>Sincronizar persona con SFDC</td> 
  </tr> 
  <tr> 
   <td>Cambiar estado en campaña SFDC</td> 
   <td>Sincronizar persona con SFDC<br>Agregar a SFDC Campaign</td> 
  </tr> 
  <tr> 
   <td>Cambiar propietario</td> 
   <td><p>Sincronizar persona con SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Convertir Persona</td> 
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
