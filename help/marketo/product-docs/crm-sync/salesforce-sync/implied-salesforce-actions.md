---
unique-page-id: 4719304
description: 'Acciones De Salesforce Implícitas: Documentos De Marketo: Documentación Del Producto'
title: Acciones de Salesforce implícitas
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# Acciones de Salesforce implícitas {#implied-salesforce-actions}

Cuando se ejecuta un paso de flujo específico de Salesforce, a veces se realizan pasos adicionales automáticamente. Estas son las reglas, para que lo sepa:

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
   <td>Sincronizar persona con SFDC<br>Añadir a la campaña de SFDC</td> 
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

Puede filtrar los registros SFDC en una lista inteligente utilizando la variable **[!UICONTROL Tipo de SFDC]** Filtre con el operador establecido en no está vacío. Todos los registros SFDC tienen un valor en este campo.

Recuerde, estas acciones automáticas solo se producen si el posible cliente no está actualmente en [Salesforce.com](https://salesforce.com){target="_blank"}
