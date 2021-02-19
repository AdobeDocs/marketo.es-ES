---
unique-page-id: 45417125
description: Perspectiva de ventas para integraciones no nativas de Salesforce - Documentos de marketing - Documentación del producto
title: Perspectiva de ventas para integraciones no nativas de Salesforce
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# Perspectiva de ventas para integraciones no nativas de Salesforce {#sales-insight-for-non-native-salesforce-integrations}

Si su cuenta de Marketing está conectada a Salesforce a través de una integración personalizada o no nativa, utilice este documento para configurar Sales Insight.

>[!PREREQUISITES]
>
>* Póngase en contacto con el administrador de éxito del cliente para habilitar la función &quot;MSI no nativo&quot; para la instancia de Marketing.
>* Cuenta de Salesforce con la configuración del paquete MSI.
>* La API de REST de Marketing to [configuró correctamente](https://developers.marketo.com/rest-api/). Las API de CRUD expuestas serán la base para realizar la sincronización no nativa.
>* Lea [esta entrada de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) para comprender el objeto y las relaciones.
>* Configure los objetos de Salesforce para que muestren el identificador único global que distingue entre mayúsculas y minúsculas de 18 caracteres en lugar del identificador único global que distingue entre mayúsculas y minúsculas de 15 caracteres.


>[!NOTE]
>
>La configuración de la API de REST en el panel de administración de MSI de Marketing to no se puede usar para la sincronización no nativa.

## La sincronización no nativa correcta para MSI requiere lo siguiente: {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronice el usuario de ventas de Salesforce con el comerciante.

   El usuario de ventas de Salesforce es un usuario externo propietario de los posibles clientes/contactos en Salesforce. Es necesario actualizar a un vendedor de marketing para el usuario de ventas de Salesforce. El campo *externalSalesPersonId* tiene el mandato de mantener al Vendedor.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de persona de ventas de marketing</strong></td> 
   <td><strong>Campo de usuario de ventas de Salesforce</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales Identificación única global que no distingue entre mayúsculas y minúsculas del usuario</td> 
   <td><p>Identifica el registro de persona de ventas de marketing en un objeto de usuario de ventas de Salesforce externo.</p><p>Se requiere que el Vendedor se sincronice primero antes de sincronizar los otros objetos para que se creen las relaciones adecuadas.</p></td> 
  </tr> 
 </tbody> 
</table>

Documentación de API para el vendedor: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
Documentación de API para sincronizar al vendedor: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. Sincronice las cuentas de Salesforce con Marketing.

   Se deberá actualizar una Compañía de marketing para la cuenta de Salesforce. Los campos _externalCompanyId_ y _externalSalesPersonId_ tienen el mandato de mantener la Compañía.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de Compañía de marketing</strong></td> 
   <td><strong>Campo de cuenta de Salesforce</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificador único global que no distingue entre mayúsculas y minúsculas de la cuenta de Salesforce</td> 
   <td>Identifica un registro de Compañía de marketing en un objeto de cuenta de Salesforce externo.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales Identificación única global que no distingue entre mayúsculas y minúsculas del usuario</td> 
   <td>Identifica un registro de Compañía de marketing para un objeto de usuario de ventas de Salesforce externo que es el propietario de la cuenta.<br><br>También se utiliza en Marketing para asociar la Compañía con el Vendedor propietario del registro de Compañía. Es obligatorio que el Vendedor se sincronice primero antes de configurar este campo.</td> 
  </tr> 
 </tbody> 
</table>

Documentación de API para Compañías: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Sincronice los leads/Contactos de Salesforce con Marketing.

   Tendrá que mantener un posible cliente de marketing para el contacto/posible cliente de Salesforce. Los campos _externalPersonId_, _externalSalesPersonId_ y _externalCompanyId_ tienen el mandato de mantener el posible cliente.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de posible cliente de marketing</strong></td> 
   <td><strong>Campo de contacto/posible cliente de Salesforce</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Identificador único global que no distingue entre mayúsculas y minúsculas en los posibles clientes y contactos de Salesforce</td> 
   <td>Identifica el registro de posibles clientes de marketing en un objeto de contacto/posible cliente de Salesforce externo.<br><br>Se trata de un nuevo campo que se introduce para los MSI no nativos.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales Identificación única global que no distingue entre mayúsculas y minúsculas del usuario</td> 
   <td>Identifica el objeto de usuario de ventas externo de Salesforce que posee este posible cliente/contacto.<br><br>También relaciona el posible cliente con la persona de ventas de Marketing. Se le exige que primero sincronice correctamente al Vendedor.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificador único global que no distingue entre mayúsculas y minúsculas de la cuenta de Salesforce</td> 
   <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece el posible cliente o contacto.<br><br>También relaciona el registro de posibles clientes con una Compañía en Marketing. Se requiere que la cuenta de Salesforce se sincronice correctamente primero.</td> 
  </tr> 
 </tbody> 
</table>

Documentación de API para posibles clientes: [`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
Documentación de API para sincronizar leads:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronizar oportunidades de Salesforce con Marketing.

   Tendrá que mantener una oportunidad de marketing para la oportunidad de Salesforce. Los campos _externalOpportunityId_, _externalCompanyId_ y _externalSalesPersonId_ tienen el mandato de mantener la oportunidad.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de objeto de oportunidad de marketing</strong></td> 
   <td><strong>Campo de objeto de oportunidad de Salesforce</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificador único global que no distingue entre mayúsculas y minúsculas en los posibles clientes y contactos de Salesforce</td> 
   <td>Identifica el registro de oportunidad de marketing en un objeto de oportunidad de Salesforce externo.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificador único global que no distingue entre mayúsculas y minúsculas de la cuenta de Salesforce</td> 
   <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece esta oportunidad. <br><br>Se requiere que la cuenta de Salesforce se sincronice correctamente primero.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales Identificación única global que no distingue entre mayúsculas y minúsculas del usuario</td> 
   <td>Identifica el objeto de usuario de ventas externo de Salesforce que posee esta oportunidad. </td> 
  </tr> 
 </tbody> 
</table>

Documentación de API para oportunidad: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizar funciones de contacto de Salesforce con Marketing.

   Las funciones de contacto de Salesforce para una oportunidad de Salesforce se pueden sincronizar mediante la función de oportunidad de marketing. El registro de la función de oportunidad establece los campos _externalOpportunityId_, _role_ y _leadId_.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de función de oportunidad de marketing</strong></td> 
   <td><strong>Campo de función de contacto de Salesforce</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificador único global que no distingue entre mayúsculas y minúsculas de Salesforce Opportunity</td> 
   <td>Identifica la función de oportunidad de marketing en un objeto de oportunidad de Salesforce externo.<br><br>Es obligatorio que la oportunidad de Salesforce se sincronice correctamente primero.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>N/D, sería un ID de posible cliente de marketing</td> 
   <td>Sería el ID de posible cliente de marketing del contacto sincronizado de Salesforce.<br><br>Una vez sincronizado el contacto en Marketing, puede utilizar el identificador único global que diferencia mayúsculas y minúsculas en Salesforce Contact como externoPersonId y la consulta para el posible cliente de marketing mediante la API REST de Marketing to.</td> 
  </tr> 
  <tr> 
   <td>role</td> 
   <td>Campo Función del contacto de Salesforce</td> 
   <td>Describe la función del contacto para esta oportunidad.</td> 
  </tr> 
 </tbody> 
</table>

Documentación de API para oportunidad: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizar los campos Última puntuación de momento interesante/MSI con SFDC.

   Una vez que los objetos de Salesforce estén correctamente sincronizados con Marketing, podrá aprovechar las funciones MSI. Los campos Último momento interesante/Puntuación del MSI se exponen en la API de REST para posibles clientes. Los MSI calculan estos campos y son de solo lectura.

   Los campos Último momento interesante/Puntuación de un posible cliente de marketing deberán sincronizarse regularmente con Salesforce mediante el extremo de posible cliente de la API de REST. Consulta este extremo para un posible cliente de marketing usando el _externalPersonId_ como filterType y pasando el GUID de posible cliente de Salesforce como filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   A continuación, puede utilizar los valores de estos campos para sincronizarlos con el objeto Lead/Contact de Salesforce.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de posible cliente de marketing</strong></td> 
   <td><strong>Campo de contacto/posible cliente de Salesforce</strong></td> 
   <td><strong>Descripción</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentType</td> 
   <td>Etiqueta: Último tipo de momento interesante<br>Nombre: Last_Interesting_Moment_Type__c</td> 
   <td>Tipo del último momento interesante para el posible cliente</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDate</td> 
   <td><p>Etiqueta: Fecha del último momento interesante</p><p>Nombre: Last_Interesting_Moment_Date__c</p></td> 
   <td>Fecha del último momento interesante para el posible cliente</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDesc</td> 
   <td><p>Etiqueta: Descripción del último momento interesante</p><p>Nombre: Last_Interesting_Moment_Desc__c</p></td> 
   <td>Descripción del último momento interesante para el posible cliente</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentSource</td> 
   <td><p>Etiqueta: Última fuente de momento interesante</p><p>Nombre: Last_Interesting_Moment_Source__c</p></td> 
   <td>Fuente del último momento interesante para el líder</td> 
  </tr> 
  <tr> 
   <td>prioridad</td> 
   <td><p>Etiqueta: Participación</p><p>Nombre: Priority_c</p></td> 
   <td>Prioridad del posible cliente</td> 
  </tr> 
  <tr> 
   <td>relativeUrgency</td> 
   <td><p>Etiqueta: Valor de urgencia relativo</p><p>Nombre: Urgency_Value__c</p></td> 
   <td>Urgencia relativa del posible cliente</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>Etiqueta: Valor de puntuación relativo</p><p>Nombre: Relative_Score_Value__c</p></td> 
   <td>Puntuación relativa del posible cliente</td> 
  </tr> 
 </tbody> 
</table>

Documentación para la API de REST de posibles clientes: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

El uso correcto de los campos externos es clave para que la sincronización no nativa se realice correctamente. Si no ve los datos en algunas de las vistas, es probable que un campo determinado no se haya sincronizado correctamente. Por ejemplo, si las actividades de un posible cliente y los momentos interesantes no aparecen al buscar en el widget MSI debajo de su cuenta, es probable que la compañía del posible cliente o la cuenta no se hayan sincronizado correctamente. La realización de una solicitud de GET para este posible cliente al especificar los campos externos le ayudará a comprobar si el posible cliente se sincronizó correctamente. Además, el correo electrónico del vendedor externo en Marketing debe coincidir con el correo electrónico de ese usuario en Salesforce. Es posible que los datos no se muestren en la ficha Comercialización de Salesforce si los mensajes de correo electrónico no coinciden.
