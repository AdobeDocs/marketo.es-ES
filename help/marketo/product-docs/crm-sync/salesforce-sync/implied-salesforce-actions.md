---
unique-page-id: 4719304
description: Acciones implícitas de Salesforce - Documentos de marketing - Documentación del producto
title: Acciones de Salesforce implícitas
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---


# Acciones de Salesforce implícitas {#implied-salesforce-actions}

Cuando se ejecuta un paso de flujo específico de Salesforce, a veces se realizan pasos adicionales automáticamente. Estas son las reglas, así que ya saben:

Estas reglas se aplicarán _cuando la persona no se encuentre actualmente en [Salesforce.com](https://Salesforce.com)_ como contacto o posible cliente.

<table> 
 <thead> 
  <tr> 
   <th>Paso de flujo de marketing</th> 
   <th>Acción automática</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Añadir a la Campaña de SFDC</td> 
   <td>Sincronizar persona con SFDC</td> 
  </tr> 
  <tr> 
   <td>Cambiar estado en la Campaña SFDC</td> 
   <td>Sincronizar persona con SFDC<br>Añadir a la Campaña de SFDC</td> 
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
   <td>Crear Tarea</td> 
   <td>Sincronizar persona con SFDC</td> 
  </tr> 
 </tbody> 
</table>

Puede filtrar los registros SFDC en una Lista inteligente mediante el filtro **Tipo SFDC** con el operador establecido en &quot;no está vacío&quot;. Todos los registros SFDC tienen un valor en este campo.

Recuerde que estas acciones automáticas solo se producen si el posible cliente no está actualmente en [Salesforce.com](https://salesforce.com)
