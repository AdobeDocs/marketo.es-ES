---
unique-page-id: 4719304
description: Acciones implícitas de Salesforce - Documentos de marketing - Documentación del producto
title: Acciones de Salesforce implícitas
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Acciones de Salesforce implícitas {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Cuando se ejecuta un paso de flujo específico de Salesforce, a veces se realizan pasos adicionales automáticamente. Estas son las reglas, así que ya saben:

Estas reglas se aplicarán *cuando la persona no se encuentre actualmente en [Salesforce.com](http://Salesforce.com)* como contacto o posible cliente.

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
   <td>Sincronizar persona con Campaña<br>SFDCAd a SFDC</td> 
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

Puede filtrar los registros SFDC en una Lista inteligente mediante el filtro de tipo **** SFDC con el operador definido como &quot;no está vacío&quot;. Todos los registros SFDC tienen un valor en este campo.

Recuerde que estas acciones automáticas solo se producen si el posible cliente no está actualmente en [Salesforce.com](http://Salesforce.com)

La sincronización de Salesforce es genial, ¿verdad?
