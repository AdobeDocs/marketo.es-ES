---
description: 'Asignación de campos de Dynamics predeterminada: documentos de Marketo, documentación del producto'
title: Asignación de campos de Dynamics predeterminada
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 40%

---

# Asignación de campos de Dynamics predeterminada {#default-dynamics-field-mapping}

Al sincronizar inicialmente la cuenta de Marketo Engage con Microsoft, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Dynamics y Marketo.  Marketo también sincronizará los campos personalizados con los posibles clientes, las cuentas, las oportunidades y los contactos.

## Campos de clientes potenciales {#lead-fields}

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
      <td>Microsoft - Fecha de creación</td>
      <td>Creado el</td>
      <td>creado el</td>
    </tr>
    <tr>
      <td>Saludo</td>
      <td>Saludo</td>
      <td>salutación</td>
    </tr>
    <tr>
      <td>Primer nombre</td>
      <td>Nombre</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Medio</td>
      <td>Segundo nombre</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Apellido</td>
      <td>Apellido</td>
      <td>apellido</td>
    </tr>
    <tr>
      <td>Correo electrónico</td>
      <td>Correo electrónico</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>Cargo</td>
      <td>Cargo</td>
      <td>puesto</td>
    </tr>
    <tr>
      <td>Teléfono</td>
      <td>Teléfono comercial</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Teléfono móvil</td>
      <td>Teléfono móvil</td>
      <td>teléfono móvil</td>
    </tr>
    <tr>
      <td>Fax</td>
      <td>Fax</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>Dirección</td>
      <td>Calle 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Ciudad</td>
      <td>Ciudad</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Estado</td>
      <td>Estado/Provincia</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>País</td>
      <td>País o región</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal</td>
      <td>Código postal</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Origen de la persona</td>
      <td>Origen del cliente potencial</td>
      <td>lead sourcecode</td>
    </tr>
    <tr>
      <td>Estado de la persona</td>
      <td>Estado</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>Razón del estado</td>
      <td>Razón del estado</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>Notas de la persona</td>
      <td>Descripción</td>
      <td>descripción</td>
    </tr>
    <tr>
      <td>No llamar</td>
      <td>No permitir llamadas telefónicas</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Suscripción cancelada</td>
      <td>No enviar correos electrónicos masivos</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Calificación de la persona</td>
      <td>Calificación</td>
      <td>lead quality code</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección 2</td>
      <td>Calle 2</td>
      <td>dirección1_línea2</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección 3</td>
      <td>Calle 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft - No enviar email</td>
      <td>No permitir correos electrónicos</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft - No enviar fax</td>
      <td>No Permitir Faxes</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Microsoft - No enviar material de marketing</td>
      <td>Material de marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft - Teléfono particular</td>
      <td>Teléfono particular</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Método De Contacto Preferido De Microsoft</td>
      <td>Método preferido de contacto</td>
      <td>preferredcontactmethod code</td>
    </tr>
    <tr>
      <td>Microsoft - Tema</td>
      <td>Tema</td>
      <td>sujeto</td>
    </tr>
    <tr>
      <td>Fecha de último momento interesante</td>
      <td>Fecha de último momento interesante</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Último momento interesante desc</td>
      <td>Último momento interesante desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Último origen de momento interesante</td>
      <td>Último origen de momento interesante</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>Tipo de último momento interesante</td>
      <td>Tipo de último momento interesante</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Compañía</td>
      <td>Nombre de la empresa</td>
      <td>companyname</td>
    </tr>
    <tr>
      <td>Puntaje relativo</td>
      <td>Puntaje relativo</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Prioridad</td>
      <td>Prioridad</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgencia relativa</td>
      <td>urgencia</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Asunto</td>
      <td>Tema</td>
      <td>sujeto</td>
    </tr>
    <tr>
      <td>Ingresos anuales</td>
      <td>Ingresos anuales</td>
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
      <td>Propietario</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creado el</td>
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
      <td>Microsoft - Fecha de creación</td>
      <td>Creado el</td>
      <td>creado el</td>
    </tr>
    <tr>
      <td>Saludo</td>
      <td>Saludo</td>
      <td>salutación</td>
    </tr>
    <tr>
      <td>Primer nombre</td>
      <td>Nombre</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Medio</td>
      <td>Segundo nombre</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Apellido</td>
      <td>Apellido</td>
      <td>apellido</td>
    </tr>
    <tr>
      <td>Correo electrónico</td>
      <td>Correo electrónico</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>Cargo</td>
      <td>Cargo</td>
      <td>puesto</td>
    </tr>
    <tr>
      <td>Teléfono</td>
      <td>Teléfono comercial</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Teléfono móvil</td>
      <td>Teléfono móvil</td>
      <td>teléfono móvil</td>
    </tr>
    <tr>
      <td>Dirección</td>
      <td>Dirección 1: Calle 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Ciudad</td>
      <td>Dirección 1: Ciudad</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Estado</td>
      <td>Dirección 1: Estado/Provincia</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>País</td>
      <td>Dirección 1: País/Región</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal</td>
      <td>Dirección 1: Código postal</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Estado de la persona</td>
      <td>Estado</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>Razón del estado</td>
      <td>Razón del estado</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>No llamar</td>
      <td>No permitir llamadas telefónicas</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Suscripción cancelada</td>
      <td>No enviar correos electrónicos masivos</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección 2</td>
      <td>Dirección 1: Calle 2</td>
      <td>dirección1_línea2</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección 3</td>
      <td>Dirección 1: Calle 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft - No enviar email</td>
      <td>No permitir correos electrónicos</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft - Teléfono particular</td>
      <td>Teléfono particular</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Método De Contacto Preferido De Microsoft</td>
      <td>Método De Contacto Preferido</td>
      <td>preferredcontactmethod code</td>
    </tr>
    <tr>
      <td>Fecha de último momento interesante</td>
      <td>Fecha de último momento interesante</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Tipo de último momento interesante</td>
      <td>Tipo de último momento interesante</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Último origen de momento interesante</td>
      <td>Último origen de momento interesante</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>Último momento interesante desc</td>
      <td>Último momento interesante desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Microsoft - No enviar material de marketing</td>
      <td>Material de marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft - No enviar fax</td>
      <td>Microsoft - No enviar fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Prioridad</td>
      <td>Prioridad</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgencia relativa</td>
      <td>urgencia</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Puntaje relativo</td>
      <td>Puntaje relativo</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Notas de la persona</td>
      <td>Descripción</td>
      <td>descripción</td>
    </tr>
    <tr>
      <td>Calificación de persona</td>
      <td>Puntaje del cliente potencial</td>
      <td>mkt_lead_score</td>
    </tr>
    <tr>
      <td>Notas de la persona</td>
      <td>Descripción</td>
      <td>descripción</td>
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
      <td>Propietario</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creado el</td>
      <td>creado el</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Nombre de la empresa</td>
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
      <td>Cuenta (a)</td>
      <td>Cuenta</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>Dirección de facturación</td>
      <td>Dirección 1: Calle 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Ciudad de facturación</td>
      <td>Dirección 1: Ciudad</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>País de facturación</td>
      <td>Dirección 1: País/Región</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal de facturación</td>
      <td>Dirección 1: Código postal</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección de facturación 2</td>
      <td>Dirección 1: Calle 2</td>
      <td>dirección1_línea2</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección de facturación 3</td>
      <td>Dirección 1: Calle 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Teléfono principal</td>
      <td>Teléfono principal</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Tipo de negocio</td>
      <td>Tipo de negocio</td>
      <td>business stypecode</td>
    </tr>
    <tr>
      <td>Número de cuenta de Microsoft</td>
      <td>Número de cuenta</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>Microsoft - Estado de la compañía</td>
      <td>Estado</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>Ingresos anuales</td>
      <td>Ingresos anuales</td>
      <td>ingresos</td>
    </tr>
    <tr>
      <td>Notas de la compañía</td>
      <td>Descripción</td>
      <td>descripción</td>
    </tr>
    <tr>
      <td>Industria</td>
      <td>Industria</td>
      <td>código de industria</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Sitio web</td>
      <td>Sitio web</td>
      <td>sitio web</td>
    </tr>
    <tr>
      <td>Cantidad de empleados</td>
      <td>Número de empleados</td>
      <td>número de empleados</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Compañía</td>
      <td>Nombre de la cuenta</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Cantidad de empleados</td>
      <td>Número de empleados</td>
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
      <td>Propietario</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creado el</td>
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
      <td>Cerrar probabilidad</td>
      <td>Probabilidad</td>
      <td>probabilidad cercana</td>
    </tr>
    <tr>
      <td>Fase</td>
      <td>estado</td>
      <td>código de estado</td>
    </tr>
    <tr>
      <td>Fecha de cierre real</td>
      <td>Fecha de cierre real</td>
      <td>actual-cerrado</td>
    </tr>
    <tr>
      <td>Nombre</td>
      <td>Tema</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Valor estimado</td>
      <td>Est. Ingresos</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>Descripción</td>
      <td>Descripción</td>
      <td>descripción</td>
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
      <td>Propietario</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>Oportunidad</td>
      <td>OpportunityId</td>
    </tr>
    <tr>
      <td>Cliente potencial</td>
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
      <td>Microsoft - Tipo</td>
      <td>Posible cliente o contacto. Si está vacío, el posible cliente solo existe como persona en Marketo</td>
    </tr>
    <tr>
      <td>Microsoft - Fecha de creación</td>
      <td>Fecha de creación en MS Dynamics (puede ser diferente de Creación en Marketo)</td>
    </tr>
    <tr>
      <td>Se ha eliminado Microsoft</td>
      <td>La persona estaba en Microsoft, pero se eliminó y ahora solo vive en Marketo</td>
    </tr>
  </tbody>
</table>
