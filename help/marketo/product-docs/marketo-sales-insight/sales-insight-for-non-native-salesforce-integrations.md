---
unique-page-id: 45417125
description: Perspectiva de ventas para integraciones no nativas de Salesforce - Marketo Docs - Documentación del producto
title: Perspectiva de ventas para integraciones no nativas de Salesforce
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Perspectiva de ventas para integraciones no nativas de Salesforce {#sales-insight-for-non-native-salesforce-integrations}

Si su cuenta de Adobe Marketo Engage está conectada a Salesforce a través de una integración personalizada o no nativa, utilice este artículo para configurar Sales Insight.

>[!PREREQUISITES]
>
>* La función &quot;MSI no nativo&quot; habilitada para su instancia de Marketo antes de comenzar a configurar MSI. Si no es así y ya ha adquirido la función, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si todavía no ha comprado esta función, póngase en contacto con el equipo de cuentas de Adobe (su administrador de cuentas).
>* Una cuenta de Salesforce con [Configuración del paquete MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* API de REST de Marketo [configuración correcta](https://developers.marketo.com/rest-api/){target="_blank"}. Las API de CRUD expuestas serán la base para realizar la sincronización no nativa.
>* Lectura [esta publicación de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para comprender el objeto y las relaciones.
>* Configure los objetos de Salesforce para que muestren el identificador único global que no distingue entre mayúsculas y minúsculas de 18 caracteres en lugar del identificador único global que distingue entre mayúsculas y minúsculas de 15 caracteres.


>[!NOTE]
>
>La configuración de la API de REST en el panel de administración de Marketo MSI no se puede usar para la sincronización no nativa.

## La sincronización no nativa correcta para MSI requiere lo siguiente {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronice el usuario de ventas de Salesforce con Marketo.

   El usuario de ventas de Salesforce es un usuario externo que posee los posibles clientes/contactos en Salesforce. Se debe actualizar un vendedor de Marketo para el usuario de ventas de Salesforce. La variable *externalSalesPersonId* se encarga de la actualización de la persona de ventas.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de persona de ventas de Marketo</strong></td> 
      <td><strong>Campo de usuario de ventas de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales Identificador único global del usuario que no distingue entre mayúsculas y minúsculas</td> 
      <td><p>Identifica el registro de persona de ventas de Marketo en un objeto de usuario de ventas externo de Salesforce.</p><p>Es obligatorio que la persona de ventas se sincronice primero antes de sincronizar los otros objetos para que se creen las relaciones adecuadas.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para el vendedor: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * Documentación de API para sincronizar al vendedor: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Ventas_Personas/syncVentasPersonasUsandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Ventas_Personas/syncVentasPersonasUsandoPOST){target="_blank"}

1. Sincronice las cuentas de Salesforce con Marketo.

   Será necesario actualizar una empresa de Marketo para la cuenta de Salesforce. La variable _externalCompanyId_ y _externalSalesPersonId_ Los campos son obligatorios para la actualización de la empresa.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de empresa de Marketo</strong></td> 
      <td><strong>Campo de cuenta de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Account</td> 
      <td>Identifica un registro de empresa de Marketo en un objeto de cuenta de Salesforce externo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales Identificador único global del usuario que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica un registro de empresa de Marketo en un objeto de usuario de ventas externo de Salesforce que es el propietario de la cuenta.<br><br>También se utiliza en Marketo para asociar la empresa a la persona de ventas propietaria del registro de empresa. Es obligatorio sincronizar primero al Vendedor antes de configurar este campo.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para empresas: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * Documentación de API para sincronizar empresas: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. Sincronice los posibles clientes/contactos de Salesforce con Marketo.

   Tendrá que confirmar un posible cliente de Marketo para el posible cliente o contacto de Salesforce. La variable _externalPersonId_, _externalSalesPersonId_ y _externalCompanyId_ Los campos son obligatorios para la actualización del posible cliente.

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
      <td>Identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Lead/Contact</td> 
      <td>Identifica el registro de posible cliente de Marketo en un objeto externo de contacto/posible cliente de Salesforce.<br><br>Este es un nuevo campo que se introduce para MSI no nativo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales Identificador único global del usuario que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica el objeto de usuario de ventas externo de Salesforce que posee este posible cliente/contacto.<br><br>También relaciona el posible cliente con el vendedor en Marketo. Es obligatorio que el Vendedor se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Account</td> 
      <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece el posible cliente/contacto.<br><br>También relaciona el registro de posibles clientes con una empresa de Marketo. Es obligatorio que la cuenta de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para posibles clientes: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * Documentación de API para sincronizar posibles clientes: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronice las oportunidades de Salesforce con Marketo.

   Deberá mantener una oportunidad de Marketo para la oportunidad de Salesforce. La variable _externalOportunityId_, _externalCompanyId_ y _externalSalesPersonId_ Los campos son obligatorios para la actualización de la oportunidad.

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
      <td>externalOportunityId</td> 
      <td>Identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Lead/Contact</td> 
      <td>Identifica el registro de oportunidad de Marketo en un objeto de oportunidad de Salesforce externo.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Account</td> 
      <td>Identifica el objeto de cuenta de Salesforce externo al que pertenece esta oportunidad. <br><br>Es obligatorio que la cuenta de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales Identificador único global del usuario que no distingue entre mayúsculas y minúsculas</td> 
      <td>Identifica el objeto de usuario de ventas externo de Salesforce propietario de esta oportunidad. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para oportunidad: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * Documentación de API para la sincronización de oportunidades: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Oportunidades/syncOportunidadesUsandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/syncOportunidadesUsandoPOST){target="_blank"}

1. Sincronizar roles de contacto de Salesforce con Marketo.

   Las funciones de contacto de Salesforce para una oportunidad de Salesforce se pueden sincronizar a través de la función de oportunidad de Marketo. El registro de la función de oportunidad ordena el _externalOportunityId_, _función_ y _leadId_ campos.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de rol de oportunidad de Marketo</strong></td> 
      <td><strong>Campo de función de contacto de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>externalOportunityId</td> 
      <td>Identificador único global sin distinción de mayúsculas y minúsculas de Salesforce</td> 
      <td>Identifica la función de oportunidad de Marketo en un objeto de oportunidad de Salesforce externo.<br><br>Es obligatorio que la oportunidad de Salesforce se sincronice correctamente primero.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, sería un ID de posible cliente de Marketo</td> 
      <td>Este sería el ID de posible cliente de Marketo del contacto sincronizado de Salesforce.<br><br>Una vez que el contacto se sincroniza en Marketo, puede utilizar el identificador único global sin distinción de mayúsculas y minúsculas de Salesforce Contact como externalPersonId y la consulta para el posible cliente de Marketo mediante la API de REST de Marketo.</td> 
     </tr> 
     <tr> 
      <td>función</td> 
      <td>El campo Rol del contacto de Salesforce</td> 
      <td>Describe la función del contacto para esta oportunidad.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentación de API para oportunidad: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * Documentación de API para la sincronización de oportunidades: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Oportunidades/syncOportunidadesUsandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/syncOportunidadesUsandoPOST){target="_blank"}

1. Sincronizar los campos de puntuación de último momento interesante/MSI con SFDC.

   Una vez que los objetos de Salesforce se sincronizan correctamente con Marketo, puede aprovechar las funciones de MSI. Los campos Último momento/puntuación interesante de MSI se expondrán en la API de REST para posibles clientes. MSI calcula estos campos y son de solo lectura.

   Los campos Último momento/puntuación interesante de un posible cliente de Marketo deberán sincronizarse regularmente con Salesforce mediante el extremo de posible cliente de la API de REST. Consulte este extremo para un posible cliente de Marketo usando la variable _externalPersonId_ como filterType y pasando el GUID de posible cliente de Salesforce como filterValue.

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
      <td><strong>Campo de posible cliente de Marketo</strong></td> 
      <td><strong>Campo de contacto/posible cliente de Salesforce</strong></td> 
      <td><strong>Descripción</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentType</td> 
      <td>Etiqueta: Último tipo de momento interesante<br>Nombre: Last_Interested_Moment_Type__c</td> 
      <td>Tipo del último momento interesante para el posible cliente</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDate</td> 
      <td><p>Etiqueta: Última fecha de momento interesante</p><p>Nombre: Last_Interested_Moment_Date__c</p></td> 
      <td>Fecha del último momento interesante para el posible cliente</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDesc</td> 
      <td><p>Etiqueta: Última descripción del momento interesante</p><p>Nombre: Last_Interested_Moment_Desc__c</p></td> 
      <td>Descripción del último momento interesante para el posible cliente</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentSource</td> 
      <td><p>Etiqueta: Última fuente de momento interesante</p><p>Nombre: Last_Interested_Moment_Source__c</p></td> 
      <td>Fuente del último momento interesante para el líder</td> 
     </tr> 
     <tr> 
      <td>prioridad</td> 
      <td><p>Etiqueta: Participación</p><p>Nombre: Priority_c</p></td> 
      <td>Prioridad del posible cliente</td> 
     </tr> 
     <tr> 
      <td>relationUrgency</td> 
      <td><p>Etiqueta: Valor de urgencia relativo</p><p>Nombre: Urgency_Value__c</p></td> 
      <td>Urgencia relativa del posible cliente</td> 
     </tr> 
     <tr> 
      <td>relationScoring</td> 
      <td><p>Etiqueta: Valor de puntuación relativo</p><p>Nombre: Relative_Score_Value__c</p></td> 
      <td>Puntuación relativa del posible cliente</td> 
     </tr> 
    </tbody> 
   </table>

   Documentación para la API de REST de posibles clientes: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   El uso correcto de los campos externos es clave para una sincronización no nativa correcta. Si no ve los datos en algunas de las vistas, es probable que un campo determinado no se haya sincronizado correctamente. Por ejemplo, si las actividades de un posible cliente y los momentos interesantes no aparecen al buscar en el widget MSI debajo de su cuenta, es probable que ni la empresa del posible cliente ni la cuenta se hayan sincronizado correctamente. Realizar una solicitud de GET para este posible cliente al especificar los campos externos le ayudará a comprobar si el posible cliente se sincronizó correctamente. Además, el correo electrónico del vendedor externo de Marketo debe coincidir con el correo electrónico de ese usuario en Salesforce. Es posible que no se muestren datos en la ficha Marketo de Salesforce si los mensajes de correo electrónico no coinciden.
