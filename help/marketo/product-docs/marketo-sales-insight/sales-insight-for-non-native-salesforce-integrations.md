---
unique-page-id: 45417125
description: Perspectiva de ventas para integraciones de Salesforce no nativas - Documentos de Marketo - Documentación del producto
title: Perspectiva de ventas para integraciones de Salesforce no nativas
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Perspectiva de ventas para integraciones de Salesforce no nativas {#sales-insight-for-non-native-salesforce-integrations}

Si su cuenta de Adobe Marketo Engage está conectada a Salesforce a través de una integración personalizada o no nativa, utilice este artículo para configurar Sales Insight.

>[!PREREQUISITES]
>
>* La función &quot;MSI no nativo&quot; habilitada para su instancia de Marketo antes de comenzar a configurar MSI. Si no es así y ya ha adquirido la función, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si todavía no ha adquirido esta función, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas).
>* Una cuenta de Salesforce con [Configuración del paquete MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* API DE REST DE MARKETO [configurado correctamente](https://developers.marketo.com/rest-api/){target="_blank"}. Las API de CRUD expuestas constituirán la base para realizar la sincronización no nativa.
>* Leer [esta publicación de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para comprender el objeto y las relaciones.
>* Configure los objetos de Salesforce para que muestren el identificador único global que distingue entre mayúsculas y minúsculas de 18 caracteres, en lugar del identificador único global que distingue entre mayúsculas y minúsculas de 15 caracteres.

>[!NOTE]
>
>La configuración de la API de REST en el panel de administración de MSI de Marketo no se puede usar para la sincronización no nativa.

## La sincronización no nativa correcta para MSI requiere lo siguiente {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronice el usuario de ventas de Salesforce con Marketo.

   El usuario de ventas de Salesforce es un usuario externo propietario de los posibles clientes/contactos de Salesforce. Se debe actualizar un vendedor de Marketo para el usuario de ventas de Salesforce. El *externalSalesPersonId* Este campo es obligatorio para el mantenimiento del vendedor.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de vendedor de Marketo</strong></td> 
      <td><strong>Campo de usuario de ventas de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador único global que distingue entre mayúsculas y minúsculas en las ventas de Salesforce</td> 
      <td><p>Identifica el registro de vendedor de Marketo en un objeto de usuario de ventas de Salesforce externo.</p><p>Se exige que el vendedor se sincronice primero antes de sincronizar los otros objetos, de modo que se creen las relaciones adecuadas.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para el vendedor: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * Documentación de la API para sincronizar el vendedor: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronice las cuentas de Salesforce con Marketo.

   Será necesario actualizar una compañía de Marketo para la cuenta de Salesforce. El _externalCompanyId_ y _externalSalesPersonId_ Estos campos son obligatorios para el mantenimiento de la Compañía.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de compañía de Marketo</strong></td> 
      <td><strong>Campo de cuenta de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global de cuenta de Salesforce que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica un registro de compañía de Marketo en un objeto de cuenta de Salesforce externo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador único global que distingue entre mayúsculas y minúsculas en las ventas de Salesforce</td> 
      <td>Identifica un registro de compañía de Marketo en un objeto de usuario de ventas de Salesforce externo que es el propietario de la cuenta.<br><br>También se utiliza en Marketo para asociar la compañía al vendedor que posee el registro de compañía. Es obligatorio sincronizar primero el vendedor antes de establecer este campo.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para empresas: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * Documentación de API para sincronizar compañías: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. Sincronice los contactos o posibles clientes de Salesforce con Marketo.

   Deberá actualizar un posible cliente de Marketo para el posible cliente/contacto de Salesforce. El _externalPersonId_, _externalSalesPersonId_, y _externalCompanyId_ Los campos de son obligatorios para el mantenimiento del posible cliente.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de posible cliente de Marketo</strong></td> 
      <td><strong>Campo de contacto/posible cliente de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identificador único global que no distingue entre mayúsculas y minúsculas y posible cliente de Salesforce</td> 
      <td>Identifica el registro de posible cliente de Marketo en un objeto de contacto o posible cliente de Salesforce externo.<br><br>Este es un nuevo campo que se introduce para MSI no nativo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador único global que distingue entre mayúsculas y minúsculas en las ventas de Salesforce</td> 
      <td>Identifica el objeto de usuario de ventas de Salesforce externo que posee este cliente potencial/contacto.<br><br>También relaciona el posible cliente con el vendedor en Marketo. Se requiere que el Vendedor se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global de cuenta de Salesforce que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece el cliente potencial/contacto.<br><br>También relaciona el registro de posibles clientes con una compañía en Marketo. Se requiere que la cuenta de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para posibles clientes: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * Documentación de la API para sincronizar posibles clientes: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronizar las oportunidades de Salesforce con Marketo.

   Deberá actualizar una oportunidad de Marketo para la oportunidad de Salesforce. El _externalOpportunityId_, _externalCompanyId_, y _externalSalesPersonId_ Los campos de son obligatorios para el mantenimiento de la oportunidad.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de objeto de oportunidad de Marketo</strong></td> 
      <td><strong>Campo de objeto de oportunidad de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificador único global que no distingue entre mayúsculas y minúsculas y posible cliente de Salesforce</td> 
      <td>Identifica el registro de oportunidad de Marketo en un objeto de oportunidad de Salesforce externo.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global de cuenta de Salesforce que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece esta oportunidad. <br><br>Se requiere que la cuenta de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador único global que distingue entre mayúsculas y minúsculas en las ventas de Salesforce</td> 
      <td>Identifica el objeto de usuario de ventas externo de Salesforce propietario de esta oportunidad. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de la API para Oportunidad: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * Documentación de la API para sincronizar oportunidades: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/syncOpportunityUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/syncOpportunityUsingPOST){target="_blank"}

1. Sincronizar las funciones de contacto de Salesforce con Marketo.

   Las funciones de contacto de Salesforce para una oportunidad de Salesforce se pueden sincronizar a través de la función de oportunidad de Marketo. El registro de función de oportunidad exige que _externalOpportunityId_, _función_, y _leadId_ campos.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de rol de oportunidad de Marketo</strong></td> 
      <td><strong>Campo de rol de contacto de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificador único global que distingue entre mayúsculas y minúsculas en las oportunidades de Salesforce</td> 
      <td>Identifica la función de oportunidad de Marketo en un objeto de oportunidad de Salesforce externo.<br><br>Es obligatorio que la oportunidad de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, sería un ID de posible cliente de Marketo</td> 
      <td>Este sería el ID de posible cliente de Marketo del contacto de Salesforce sincronizado.<br><br>Una vez que el contacto se sincroniza en Marketo, puede utilizar el identificador único global que distingue entre mayúsculas y minúsculas de Contacto de Salesforce como externalPersonId y consultar al posible cliente de Marketo mediante la API de REST de Marketo.</td> 
     </tr> 
     <tr> 
      <td>función</td> 
      <td>El campo Función para el contacto de Salesforce</td> 
      <td>Describe la función del contacto en esta oportunidad.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de la API para Oportunidad: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * Documentación de la API para sincronizar oportunidades: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/syncOpportunityUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/syncOpportunityUsingPOST){target="_blank"}

1. Sincronizar los campos de puntuación de último momento interesante/MSI con SFDC.

   Una vez que los objetos de Salesforce estén correctamente sincronizados con Marketo, puede aprovechar las funciones de MSI. Los campos Último momento interesante/Puntuación de MSI se expondrán en la API de REST para posibles clientes. Estos campos se calculan mediante MSI y son de solo lectura.

   Los campos Último momento interesante/Puntuación de un posible cliente de Marketo deberán sincronizarse regularmente con Salesforce mediante el punto final del posible cliente de la API de REST. Consulte este extremo para un posible cliente de Marketo mediante la variable _externalPersonId_ como filterType y pasando el GUID de posible cliente de Salesforce como filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   A continuación, puede utilizar los valores de estos campos para sincronizarlos con el objeto de posible cliente/contacto de Salesforce.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de posible cliente de Marketo</strong></td> 
      <td><strong>Campo de contacto/posible cliente de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Etiqueta: Tipo de último momento interesante<br>Nombre: Last_Interesting_Moment_Type__c</td> 
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
      <td><p>Etiqueta: Último momento interesante Fuente</p><p>Nombre: Last_Interesting_Moment_Source__c</p></td> 
      <td>Origen del último momento interesante para el posible cliente</td> 
     </tr> 
     <tr> 
      <td>prioridad</td> 
      <td><p>Etiqueta: Participación</p><p>Nombre: Priority__c</p></td> 
      <td>Prioridad del posible cliente</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Etiqueta: Valor de urgencia relativa</p><p>Nombre: Urgency_Value__c</p></td> 
      <td>Relativa urgencia del posible cliente</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Etiqueta: Valor de puntuación relativo</p><p>Nombre: Relative_Score_Value__c</p></td> 
      <td>Puntuación relativa del posible cliente</td> 
     </tr> 
    </tbody> 
   </table>

   Documentación de la API de REST de posible cliente: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   El uso adecuado de los campos externos es clave para que la sincronización no nativa se realice correctamente. Si no ve los datos en algunas vistas, es probable que un campo determinado no se haya sincronizado correctamente. Por ejemplo, si las actividades y los momentos interesantes de un posible cliente no aparecen al buscar en el widget MSI debajo de su cuenta, es probable que la compañía o la cuenta del posible cliente no se hayan sincronizado correctamente. Realizar una solicitud de GET para este posible cliente al especificar los campos externos le ayudará a comprobar si el posible cliente se sincronizó correctamente. Además, el correo electrónico del vendedor externo de Marketo debe coincidir con el del usuario de Salesforce en cuestión. Es posible que los datos no se muestren en la pestaña Marketo de Salesforce si los correos electrónicos no coinciden.
