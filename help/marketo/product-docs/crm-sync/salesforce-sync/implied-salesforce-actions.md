---
unique-page-id: 4719304
description: 'Acciones implícitas de Salesforce: Documentos de Marketo: Documentación del producto'
title: Acciones de Salesforce implícitas
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Acciones de Salesforce implícitas {#implied-salesforce-actions}

Cuando se ejecuta un paso de flujo específico de Salesforce, a veces se realizan automáticamente pasos adicionales. Estas son las reglas, por lo que sabe:

Estas reglas se aplicarán _cuando la persona no esté actualmente en [Salesforce.com](https://Salesforce.com)_ como contacto o posible cliente.

<table> 
 <thead> 
  <tr> 
   <th>Paso de flujo de Marketo</th> 
   <th>Acción automática</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Añadir a la campaña SFDC</td> 
   <td>Sincronizar persona con SFDC</td> 
  </tr> 
  <tr> 
   <td>Cambiar estado en una campaña SFDC</td> 
   <td>Sincronizar persona con SFDC<br>Agregar a campaña SFDC</td> 
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

Puede filtrar los registros SFDC en una lista inteligente mediante el filtro **Tipo SFDC** con el operador establecido en &quot;no está vacío&quot;. Todos los registros SFDC tienen un valor en este campo.

Recuerde que estas acciones automáticas solo se producen si el posible cliente no está actualmente en [Salesforce.com](https://salesforce.com)
