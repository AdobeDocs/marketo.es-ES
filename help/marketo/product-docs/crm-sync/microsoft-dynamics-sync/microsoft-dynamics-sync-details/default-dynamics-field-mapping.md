---
description: 'Asignación de campos de Dynamics predeterminada: documentos de Marketo, documentación del producto'
title: Asignación de campos de Dynamics predeterminada
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 2%

---

# Asignación de campos de Dynamics predeterminada {#default-dynamics-field-mapping}

Al sincronizar inicialmente la cuenta de Marketo Engage con Microsoft, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Dynamics y Marketo.  Marketo también sincronizará los campos personalizados con los posibles clientes, las cuentas, las oportunidades y los contactos.

## Campos de leads {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Fecha de creación]</td>
      <td>[!UICONTROL Creado El]</td>
      <td>creado el</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>salutación</td>
    </tr>
    <tr>
      <td>[!UICONTROL Primero]</td>
      <td>[!UICONTROL Nombre]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Medio]</td>
      <td>[!UICONTROL Segundo nombre]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último]</td>
      <td>[!UICONTROL Apellidos]</td>
      <td>apellido</td>
    </tr>
    <tr>
      <td>[!UICONTROL Correo electrónico]</td>
      <td>[!UICONTROL Correo electrónico]</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Puesto]</td>
      <td>[!UICONTROL Título de trabajo]</td>
      <td>puesto</td>
    </tr>
    <tr>
      <td>[!UICONTROL Teléfono]</td>
      <td>[!UICONTROL Teléfono profesional]</td>
      <td>teléfono1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Teléfono móvil]</td>
      <td>teléfono móvil</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fax]</td>
      <td>[!UICONTROL Fax]</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección]</td>
      <td>[!UICONTROL Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Ciudad]</td>
      <td>[!UICONTROL Ciudad]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado]</td>
      <td>[!UICONTROL Estado/Provincia]</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>[!UICONTROL País]</td>
      <td>[!UICONTROL País/Región]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código postal]</td>
      <td>[!UICONTROL Código postal]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Source]</td>
      <td>[!UICONTROL Lead Source]</td>
      <td>lead sourcecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado de persona]</td>
      <td>[!UICONTROL Estado]</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>[!UICONTROL Motivo de estado]</td>
      <td>[!UICONTROL Motivo de estado]</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>[!UICONTROL Notas de persona]</td>
      <td>[!UICONTROL Descripción]</td>
      <td>Descripción</td>
    </tr>
    <tr>
      <td>[!UICONTROL No llamar]</td>
      <td>[!UICONTROL No permitir llamadas telefónicas]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cancelado la suscripción]</td>
      <td>[!UICONTROL No enviar correo electrónico masivo]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Clasificación de persona]</td>
      <td>[!UICONTROL Clasificación]</td>
      <td>lead quality code</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección Microsoft 2]</td>
      <td>[!UICONTROL Street 2]</td>
      <td>dirección1_línea2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección Microsoft 3]</td>
      <td>[!UICONTROL Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft No enviar correo electrónico]</td>
      <td>[!UICONTROL No permitir correos electrónicos]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL No permitir faxes]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft No enviar material de marketing]</td>
      <td>[!UICONTROL Material de marketing]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Teléfono particular]</td>
      <td>teléfono2</td>
    </tr>
    <tr>
      <td>Método de contacto preferido de [!UICONTROL Microsoft]</td>
      <td>Método de contacto preferido de </td>
      <td>preferredcontactmethod code</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Topic]</td>
      <td>[!UICONTROL Tema]</td>
      <td>sujeto</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fecha de último momento interesante]</td>
      <td>[!UICONTROL Fecha de último momento interesante]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último momento interesante desc]</td>
      <td>[!UICONTROL Último momento interesante desc]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último origen de momento interesante]</td>
      <td>[!UICONTROL Último origen de momento interesante]</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último tipo de momento interesante]</td>
      <td>[!UICONTROL Último tipo de momento interesante]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Nombre de la compañía]</td>
      <td>companyname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Puntuación relativa]</td>
      <td>[!UICONTROL Puntuación relativa]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Prioridad]</td>
      <td>[!UICONTROL Prioridad]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgencia]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Asunto]</td>
      <td>[!UICONTROL Tema]</td>
      <td>sujeto</td>
    </tr>
    <tr>
      <td>[!UICONTROL Ingresos anuales]</td>
      <td>[!UICONTROL Ingresos anuales]</td>
      <td>ingresos</td>
    </tr>
  </tbody>
</table>

Los campos de posibles clientes siguientes se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Propietario] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Creado El]</td>
      <td>creado el</td>
    </tr>
  </tbody>
</table>

## Campos de contactos {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Fecha de creación]</td>
      <td>[!UICONTROL Creado El]</td>
      <td>creado el</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>salutación</td>
    </tr>
    <tr>
      <td>[!UICONTROL Primero]</td>
      <td>[!UICONTROL Nombre]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Medio]</td>
      <td>[!UICONTROL Segundo nombre]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último]</td>
      <td>[!UICONTROL Apellidos]</td>
      <td>apellido</td>
    </tr>
    <tr>
      <td>[!UICONTROL Correo electrónico]</td>
      <td>[!UICONTROL Correo electrónico]</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Puesto]</td>
      <td>[!UICONTROL Puesto]</td>
      <td>puesto</td>
    </tr>
    <tr>
      <td>[!UICONTROL Teléfono]</td>
      <td>[!UICONTROL Teléfono profesional]</td>
      <td>teléfono1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Teléfono móvil]</td>
      <td>teléfono móvil</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección]</td>
      <td>[!UICONTROL Dirección 1: Calle 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Ciudad]</td>
      <td>[!UICONTROL Dirección 1: Ciudad]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado]</td>
      <td>[!UICONTROL Dirección 1: estado/provincia]</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>[!UICONTROL País]</td>
      <td>[!UICONTROL Dirección 1: País/Región]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código postal]</td>
      <td>[!UICONTROL Dirección 1: Código postal]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado de persona]</td>
      <td>[!UICONTROL Estado]</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>[!UICONTROL Motivo de estado]</td>
      <td>[!UICONTROL Motivo de estado]</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>[!UICONTROL No llamar]</td>
      <td>[!UICONTROL No permitir llamadas telefónicas]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cancelado la suscripción]</td>
      <td>[!UICONTROL No enviar correo electrónico masivo]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección Microsoft 2]</td>
      <td>[!UICONTROL Dirección 1: Calle 2]</td>
      <td>dirección1_línea2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección Microsoft 3]</td>
      <td>[!UICONTROL Dirección 1: Calle 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft No enviar correo electrónico]</td>
      <td>[!UICONTROL No permitir correos electrónicos]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Teléfono particular]</td>
      <td>teléfono2</td>
    </tr>
    <tr>
      <td>Método de contacto preferido de [!UICONTROL Microsoft]</td>
      <td>Método de contacto preferido de </td>
      <td>preferredcontactmethod code</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fecha de último momento interesante]</td>
      <td>[!UICONTROL Fecha de último momento interesante]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último tipo de momento interesante]</td>
      <td>[!UICONTROL Último tipo de momento interesante]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último origen de momento interesante]</td>
      <td>[!UICONTROL Último origen de momento interesante]</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último momento interesante desc]</td>
      <td>[!UICONTROL Último momento interesante desc]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft No enviar material de marketing]</td>
      <td>[!UICONTROL Material de marketing]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Prioridad]</td>
      <td>[!UICONTROL Prioridad]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgencia]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Puntuación relativa]</td>
      <td>[!UICONTROL Puntuación relativa]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Notas de persona]</td>
      <td>[!UICONTROL Descripción]</td>
      <td>description </td>
    </tr>
    <tr>
      <td>[!UICONTROL Puntuación de persona]</td>
      <td>[!UICONTROL Puntuación de posibles clientes]</td>
      <td>mkt_lead_score</td>
    </tr>
    <tr>
      <td>[!UICONTROL Notas de persona]</td>
      <td>[!UICONTROL Descripción]</td>
      <td>description </td>
    </tr>
  </tbody>
</table>

Los campos Contacto a continuación se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Propietario] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Creado El]</td>
      <td>creado el</td>
    </tr>
    <tr>
      <td>[!UICONTROL Nombre de la compañía]</td>
      <td>parentcustomerid</td>
    </tr>
  </tbody>
</table>

## Campos de cuentas {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Cuenta (a)]</td>
      <td>[!UICONTROL Cuenta]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección de facturación]</td>
      <td>[!UICONTROL Dirección 1: Calle 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Ciudad de facturación]</td>
      <td>[!UICONTROL Dirección 1: Ciudad]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL País de facturación]</td>
      <td>[!UICONTROL Dirección 1: País/Región]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código postal de facturación]</td>
      <td>[!UICONTROL Dirección 1: Código postal]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección de facturación Microsoft 2]</td>
      <td>[!UICONTROL Dirección 1: Calle 2]</td>
      <td>dirección1_línea2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Dirección de facturación de Microsoft 3]</td>
      <td>[!UICONTROL Dirección 1: Calle 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Teléfono principal]</td>
      <td>[!UICONTROL Teléfono principal]</td>
      <td>teléfono1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Tipo de empresa]</td>
      <td>[!UICONTROL Tipo de empresa]</td>
      <td>business stypecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Número de cuenta de Microsoft]</td>
      <td>[!UICONTROL Número de cuenta]</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado de la compañía de Microsoft]</td>
      <td>[!UICONTROL Estado]</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>[!UICONTROL Ingresos anuales]</td>
      <td>[!UICONTROL Ingresos anuales]</td>
      <td>ingresos</td>
    </tr>
    <tr>
      <td>[!UICONTROL Notas de la compañía]</td>
      <td>[!UICONTROL Descripción]</td>
      <td>Descripción</td>
    </tr>
    <tr>
      <td>[!UICONTROL Industria]</td>
      <td>[!UICONTROL Industria]</td>
      <td>código de industria</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código SIC]</td>
      <td>[!UICONTROL Código SIC]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Sitio web]</td>
      <td>[!UICONTROL Sitio web]</td>
      <td>sitio web</td>
    </tr>
    <tr>
      <td>[!UICONTROL Número de empleados]</td>
      <td>[!UICONTROL Número de empleados]</td>
      <td>número de empleados</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código SIC]</td>
      <td>[!UICONTROL Código SIC]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Nombre de cuenta]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Número de empleados]</td>
      <td>[!UICONTROL Número de empleados]</td>
      <td>número de empleados</td>
    </tr>
  </tbody>
</table>

Los campos de Cuenta a continuación se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Propietario] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Creado El]</td>
      <td>creado el</td>
    </tr>
  </tbody>
</table>

## Campos de oportunidad {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Probabilidad de cierre]</td>
      <td>[!UICONTROL Probabilidad]</td>
      <td>probabilidad cercana</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fase]</td>
      <td>[!UICONTROL Estado]</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fecha de cierre real]</td>
      <td>[!UICONTROL Fecha de cierre real]</td>
      <td>actual-cerrado</td>
    </tr>
    <tr>
      <td>[!UICONTROL Nombre]</td>
      <td>[!UICONTROL Tema]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Valor estimado]</td>
      <td>[!UICONTROL Est. Ingresos]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL Descripción]</td>
      <td>[!UICONTROL Descripción]</td>
      <td>Descripción</td>
    </tr>
  </tbody>
</table>

Los campos de Cuenta a continuación se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de API de MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Propietario] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Oportunidad]</td>
      <td>OpportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cliente potencial]</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Campos de sistema relacionados con Microsoft en Marketo (solo lectura) {#microsoft-related-system-fields}

Los campos siguientes se crean en Marketo, pero los usuarios no pueden ajustarlos.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Descripción</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Type]</td>
      <td>Posible cliente o contacto. Si está vacío, el posible cliente solo existe como persona en Marketo</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Fecha de creación]</td>
      <td>Fecha de creación en [!DNL MS Dynamics] (puede ser diferente de Creado en Marketo)</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft se ha eliminado]</td>
      <td>La persona estaba en Microsoft, pero se eliminó y ahora solo vive en Marketo</td>
    </tr>
  </tbody>
</table>
