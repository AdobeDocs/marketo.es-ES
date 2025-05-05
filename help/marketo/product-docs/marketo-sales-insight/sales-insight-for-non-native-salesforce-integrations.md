---
unique-page-id: 45417125
description: Perspectiva de ventas para integraciones de Salesforce no nativas - Documentos de Marketo - Documentación del producto
title: Perspectiva de ventas para integraciones de Salesforce no nativas
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 0%

---

# Perspectiva de ventas para integraciones de Salesforce no nativas {#sales-insight-for-non-native-salesforce-integrations}

Si su cuenta de Adobe Marketo Engage está conectada a Salesforce a través de una integración personalizada o no nativa, utilice este artículo para configurar Sales Insight.

>[!PREREQUISITES]
>
>* La función &quot;MSI no nativo&quot; habilitada para su instancia de Marketo antes de comenzar a configurar MSI. Si no es así y ya compraste la función, comunícate con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si todavía no ha adquirido esta función, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas).
>* Cuenta de Salesforce con [paquete MSI configurado](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* La API de REST de Marketo [se configuró correctamente](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Las API de CRUD expuestas constituirán la base para realizar la sincronización no nativa.
>* Lea [esta publicación de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para comprender el objeto y las relaciones.
>* Configure los objetos de Salesforce para que muestren el identificador único global que distingue entre mayúsculas y minúsculas de 18 caracteres, en lugar del identificador único global que distingue entre mayúsculas y minúsculas de 15 caracteres.

>[!NOTE]
>
>La configuración de la API de REST en el panel de administración de MSI de Marketo no se puede usar para la sincronización no nativa.

## La sincronización no nativa correcta para MSI requiere lo siguiente {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronice el usuario de ventas de Salesforce con Marketo.

   El usuario de ventas de Salesforce es un usuario externo propietario de los posibles clientes o contactos de Salesforce. Se debe actualizar un vendedor de Marketo para el usuario de ventas de Salesforce. El campo *externalSalesPersonId* se exige para el mantenimiento del vendedor.

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

   * Documentación de API para el vendedor: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentación de API para sincronizar el vendedor: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronice las cuentas de Salesforce con Marketo.

   Será necesario actualizar una compañía de Marketo para la cuenta de Salesforce. Los campos _externalCompanyId_ y _externalSalesPersonId_ son obligatorios para la actualización de la compañía.

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
      <td>Identifica un registro de compañía de Marketo en un objeto de usuario de ventas de Salesforce externo que es el propietario de la cuenta.<br><br>También se usa en Marketo para asociar la compañía al vendedor que posee el registro de compañía. Es obligatorio sincronizar primero el vendedor antes de establecer este campo.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para compañías: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentación de API para sincronizar compañías: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Sincronice los contactos o posibles clientes de Salesforce con Marketo.

   Deberá actualizar un posible cliente de Marketo para el posible cliente/contacto de Salesforce. Los campos _externalPersonId_, _externalSalesPersonId_ y _externalCompanyId_ son obligatorios para la actualización del posible cliente.

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
      <td>Identifica el objeto de usuario de ventas de Salesforce externo que posee este cliente potencial/contacto.<br><br>También relaciona al posible cliente con el vendedor en Marketo. Se requiere que el Vendedor se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global de cuenta de Salesforce que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece el cliente potencial/contacto.<br><br>También relaciona el registro de posibles clientes con una compañía en Marketo. Se requiere que la cuenta de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para posibles clientes: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentación de API para sincronizar posibles clientes: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Sincronizar las oportunidades de Salesforce con Marketo.

   Deberá actualizar una oportunidad de Marketo para la oportunidad de Salesforce. Los campos _externalOpportunityId_, _externalCompanyId_ y _externalSalesPersonId_ son obligatorios para la actualización de la oportunidad.

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
      <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece esta oportunidad. <br><br>Es obligatorio que la cuenta de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador único global que distingue entre mayúsculas y minúsculas en las ventas de Salesforce</td> 
      <td>Identifica el objeto de usuario de ventas externo de Salesforce propietario de esta oportunidad. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de la API para la oportunidad: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentación de API para sincronizar oportunidades: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar las funciones de contacto de Salesforce con Marketo.

   Las funciones de contacto de Salesforce para una oportunidad de Salesforce se pueden sincronizar a través de la función de oportunidad de Marketo. El registro de función de oportunidad exige los campos _externalOpportunityId_, _role_ y _leadId_.

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
      <td>Este sería el ID de posible cliente de Marketo del contacto de Salesforce sincronizado.<br><br>Una vez que el contacto se ha sincronizado en Marketo, puede usar el identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Contact como externalPersonId y consultar al posible cliente de Marketo mediante la API de REST de Marketo.</td> 
     </tr> 
     <tr> 
      <td>función</td> 
      <td>El campo Función para el contacto de Salesforce</td> 
      <td>Describe la función del contacto en esta oportunidad.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de la API para la oportunidad: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentación de API para sincronizar oportunidades: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar los campos de puntuación de último momento interesante/MSI con SFDC.

   Una vez que los objetos de Salesforce estén correctamente sincronizados con Marketo, puede aprovechar las funciones de MSI. Los campos Último momento interesante/Puntuación de MSI se expondrán en la API de REST para posibles clientes. Estos campos se calculan mediante MSI y son de solo lectura.

   Los campos Último momento interesante/Puntuación de un posible cliente de Marketo deberán sincronizarse regularmente con Salesforce mediante el punto final del posible cliente de la API de REST. Consulte este extremo para un posible cliente de Marketo usando _externalPersonId_ como filterType y pasando el GUID de posible cliente de Salesforce como filterValue.

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
      <td><p>Etiqueta: Último momento interesante Source</p><p>Nombre: Last_Interesting_Moment_Source__c</p></td> 
      <td>Source del último momento interesante para el posible cliente</td> 
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

   Documentación de la API de REST de posibles clientes: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   El uso adecuado de los campos externos es clave para que la sincronización no nativa se realice correctamente. Si no ve los datos en algunas vistas, es probable que un campo determinado no se haya sincronizado correctamente. Por ejemplo, si las actividades y los momentos interesantes de un posible cliente no aparecen al buscar en el widget MSI debajo de su cuenta, es probable que la compañía o la cuenta del posible cliente no se hayan sincronizado correctamente. Realizar una solicitud de GET para este posible cliente al especificar los campos externos le ayudará a comprobar si el posible cliente se sincronizó correctamente. Además, el correo electrónico del vendedor externo de Marketo debe coincidir con el del usuario de Salesforce en cuestión. Es posible que los datos no se muestren en la pestaña Marketo de Salesforce si los correos electrónicos no coinciden.
