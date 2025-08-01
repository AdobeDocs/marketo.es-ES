---
unique-page-id: 45417125
description: '[!DNL Sales Insight] para integraciones no nativas  [!DNL Salesforce] Documentos de Marketo - Documentación del producto'
title: '[!DNL Sales Insight] para integraciones  [!DNL Salesforce] no nativas'
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---

# [!DNL Sales Insight] para integraciones no nativas de [!DNL Salesforce] {#sales-insight-for-non-native-salesforce-integrations}

Si su cuenta de Adobe Marketo Engage está conectada a [!DNL Salesforce] mediante una integración personalizada o no nativa, use este artículo para configurar [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* La función &quot;MSI no nativo&quot; habilitada para su instancia de Marketo antes de comenzar a configurar MSI. Si no es así y ya compraste la función, comunícate con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Si todavía no ha adquirido esta función, póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas).
>* Una cuenta de Salesforce con [paquete MSI configurado](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* La API de REST de Marketo [se configuró correctamente](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. Las API de CRUD expuestas constituirán la base para realizar la sincronización no nativa.
>* Lea [esta publicación de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para comprender el objeto y las relaciones.
>* Configure [!DNL Salesforce] objetos para que muestren el identificador único global que distingue entre mayúsculas y minúsculas de 18 caracteres, en lugar del identificador único global que distingue entre mayúsculas y minúsculas de 15 caracteres.

>[!NOTE]
>
>La configuración de la API de REST en el panel de administración de MSI de Marketo no se puede usar para la sincronización no nativa.

## La sincronización no nativa correcta para MSI requiere lo siguiente {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizar el usuario de ventas [!DNL Salesforce] con Marketo.

   El usuario de ventas [!DNL Salesforce] es un usuario externo propietario de los contactos o posibles clientes de [!DNL Salesforce]. Se debe actualizar un vendedor de Marketo para el usuario de ventas [!DNL Salesforce]. El campo *externalSalesPersonId* se exige para el mantenimiento del vendedor.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de vendedor de Marketo</strong></td>
        <td><strong>Campo de usuario de ventas <span class="dnl">Salesforce</span></strong></td>
      <td><strong>Descripción</strong></td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que distingue entre mayúsculas y minúsculas en las ventas del usuario</td>
      <td><p>Identifica el registro de vendedor de Marketo en un objeto de usuario de ventas <span class="dnl">Salesforce</span> externo.</p><p>Se exige que el vendedor se sincronice primero antes de sincronizar los otros objetos, de modo que se creen las relaciones adecuadas.</p></td>
     </tr>
    </tbody>
   </table>

   * Documentación de API para el vendedor: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentación de API para sincronizar el vendedor: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizar las cuentas de [!DNL Salesforce] con Marketo.

   Se tendrá que actualizar una compañía de Marketo para la cuenta [!DNL Salesforce]. Los campos _externalCompanyId_ y _externalSalesPersonId_ son obligatorios para la actualización de la compañía.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de compañía de Marketo</strong></td>
        <td><strong>Campo de cuenta <span class="dnl">Salesforce</span></strong></td>
      <td><strong>Descripción</strong></td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que no distingue entre mayúsculas y minúsculas en la cuenta</td>
        <td>Identifica un registro de compañía de Marketo en un objeto de cuenta <span class="dnl">Salesforce</span> externo.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que distingue entre mayúsculas y minúsculas en las ventas del usuario</td>
        <td>Identifica un registro de Marketo Company en un objeto de usuario de ventas <span class="dnl">Salesforce</span> externo que es el propietario de la cuenta.<br><br>También se usa en Marketo para asociar la compañía al vendedor que posee el registro de compañía. Es obligatorio sincronizar primero el vendedor antes de establecer este campo.</td>
     </tr>
    </tbody>
   </table>

   * Documentación de API para compañías: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentación de API para sincronizar compañías: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Sincronizar los contactos o posibles clientes de [!DNL Salesforce] con Marketo.

   Deberá actualizar un posible cliente de Marketo para el posible cliente/contacto [!DNL Salesforce]. Los campos _externalPersonId_, _externalSalesPersonId_ y _externalCompanyId_ son obligatorios para la actualización del posible cliente.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de posible cliente de Marketo</strong></td>
        <td><strong><span class="dnl">Campo de contacto/posible cliente de Salesforce</span></strong></td>
      <td><strong>Descripción</strong></td>
     </tr>
     <tr>
      <td>externalPersonId</td>
        <td>Identificador único global que distingue entre mayúsculas y minúsculas de <span class="dnl">Salesforce</span></td>
        <td>Identifica el registro de posible cliente de Marketo en un objeto de contacto o posible cliente de <span class="dnl">Salesforce</span> externo.<br><br>Este es un nuevo campo que se introduce para MSI no nativo.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que distingue entre mayúsculas y minúsculas en las ventas del usuario</td>
        <td>Identifica al objeto de usuario de ventas externo <span class="dnl">Salesforce</span> propietario de este posible cliente/contacto.<br><br>También relaciona al posible cliente con el vendedor en Marketo. Se requiere que el Vendedor se sincronice correctamente primero.</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que no distingue entre mayúsculas y minúsculas en la cuenta</td>
        <td>Identifica el objeto de cuenta <span class="dnl">Salesforce</span> externo al que pertenece el posible cliente/contacto.<br><br>También relaciona el registro de posibles clientes con una compañía en Marketo. Es obligatorio que la cuenta de Salesforce se sincronice correctamente primero.</td>
     </tr>
    </tbody>
   </table>

   * Documentación de API para posibles clientes: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentación de API para sincronizar posibles clientes: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Sincronizar [!DNL Salesforce] oportunidades con Marketo.

   Deberá actualizar una oportunidad de Marketo para la oportunidad [!DNL Salesforce]. Los campos _externalOpportunityId_, _externalCompanyId_ y _externalSalesPersonId_ son obligatorios para la actualización de la oportunidad.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de objeto de oportunidad de Marketo</strong></td>
        <td><strong><span class="dnl">Campo de objeto de oportunidad Salesforce</span></strong></td>
      <td><strong>Descripción</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
      <td>Identificador único global que no distingue entre mayúsculas y minúsculas y de contacto de Salesforce</td>
      <td>Identifica el registro de oportunidad de Marketo en un objeto de oportunidad de Salesforce externo.</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que no distingue entre mayúsculas y minúsculas en la cuenta</td>
        <td>Identifica el objeto de cuenta <span class="dnl">Salesforce</span> externo al que pertenece esta oportunidad. <br><br>Es obligatorio que la cuenta de <span class="dnl">Salesforce</span> se sincronice correctamente primero.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador único global que distingue entre mayúsculas y minúsculas en las ventas del usuario</td>
        <td>Identifica el objeto de usuario de ventas externo <span class="dnl">Salesforce</span> propietario de esta oportunidad. </td>
     </tr>
    </tbody>
   </table>

   * Documentación de la API para la oportunidad: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentación de API para sincronizar oportunidades: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar [!DNL Salesforce] roles de contacto con Marketo.

   Los roles de contacto de [!DNL Salesforce] para una oportunidad [!DNL Salesforce] se pueden sincronizar a través del rol de oportunidad de Marketo. El registro de función de oportunidad exige los campos _externalOpportunityId_, _role_ y _leadId_.

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
        <td><span class="dnl">Salesforce</span> Identificador único global que no distingue entre mayúsculas y minúsculas de oportunidad</td>
        <td>Identifica la función de oportunidad de Marketo en un objeto de oportunidad <span class="dnl">Salesforce</span> externo.<br><br>Es obligatorio que la oportunidad <span class="dnl">Salesforce</span> se sincronice correctamente primero.</td>
     </tr>
     <tr>
      <td>leadId</td>
      <td>N/D, sería un ID de posible cliente de Marketo</td>
        <td>Este sería el ID de posible cliente de Marketo del contacto <span class="dnl">Salesforce</span> sincronizado.<br><br>Una vez que el contacto está sincronizado en Marketo, puede usar el identificador único global sin distinción de mayúsculas y minúsculas de <span class="dnl">Salesforce</span> Contact como externalPersonId y consultar al posible cliente de Marketo mediante la API REST de Marketo.</td>
     </tr>
     <tr>
      <td>función</td>
        <td>El campo Rol del contacto <span class="dnl">Salesforce</span></td>
      <td>Describe la función del contacto en esta oportunidad.</td>
     </tr>
    </tbody>
   </table>

   * Documentación de la API para la oportunidad: [https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentación de API para sincronizar oportunidades: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar los campos de puntuación de último momento interesante/MSI con SFDC.

   Una vez que los objetos de [!DNL Salesforce] se hayan sincronizado correctamente con Marketo, puede aprovechar las características de MSI. Los campos Último momento interesante/Puntuación de MSI se expondrán en la API de REST para posibles clientes. Estos campos se calculan mediante MSI y son de solo lectura.

   Los campos Último momento interesante/Puntuación de un posible cliente de Marketo deberán sincronizarse regularmente con [!DNL Salesforce] mediante el punto final del posible cliente de la API de REST. Consulte este extremo para un posible cliente de Marketo usando _externalPersonId_ como filterType y pasando el GUID de posible cliente [!DNL Salesforce] como filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   A continuación, puede utilizar los valores de estos campos para sincronizarlos con el objeto de posible cliente/contacto [!DNL Salesforce].

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de posible cliente de Marketo</strong></td>
        <td><strong><span class="dnl">Campo de contacto/posible cliente de Salesforce</span></strong></td>
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

   El uso adecuado de los campos externos es clave para que la sincronización no nativa se realice correctamente. Si no ve los datos en algunas vistas, es probable que un campo determinado no se haya sincronizado correctamente. Por ejemplo, si las actividades y los momentos interesantes de un posible cliente no aparecen al buscar en el widget MSI debajo de su cuenta, es probable que la compañía o la cuenta del posible cliente no se hayan sincronizado correctamente. Realizar una solicitud de GET para este posible cliente al especificar los campos externos le ayudará a comprobar si el posible cliente se sincronizó correctamente. Además, el correo electrónico del vendedor externo de Marketo debe coincidir con el del usuario de Salesforce. Es posible que los datos no se muestren en la pestaña Marketo de Salesforce si los correos electrónicos no coinciden.
