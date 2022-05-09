---
description: 'Asignación de campos de Dynamics predeterminada: Documentos de Marketo: Documentación del producto'
title: Asignación de campos de Dynamics predeterminada
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
source-git-commit: d87809e12f153d025f8d013ea52e06c0b6530154
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 38%

---

# Asignación de campos de Dynamics predeterminada {#default-dynamics-field-mapping}

Cuando sincroniza inicialmente su cuenta de Marketo con Microsoft, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Dynamics y Marketo.  Marketo también sincronizará los campos personalizados de posibles clientes, cuentas, oportunidades y contactos.

## Campos de posibles clientes {#lead-fields}

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
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Microsoft - Fecha de creación</td>
      <td>Creado el</td>
      <td>creado</td>
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
      <td>lastname</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Correo electrónico</td>
      <td>email address1</td>
    </tr>
    <tr>
      <td>Cargo</td>
      <td>Puesto de trabajo</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Teléfono</td>
      <td>Teléfono comercial</td>
      <td>phone1</td>
    </tr>
    <tr>
      <td>Teléfono móvil</td>
      <td>Teléfono móvil</td>
      <td>mobilephone</td>
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
      <td>address1_stateorprovincia</td>
    </tr>
    <tr>
      <td>País</td>
      <td>País/región</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal</td>
      <td>Código postal</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Origen de la persona</td>
      <td>Origen del lead</td>
      <td>leader sourccode</td>
    </tr>
    <tr>
      <td>Estado de la persona</td>
      <td>Estado</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>Razón del estado</td>
      <td>Razón del estado</td>
      <td>statuscode</td>
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
      <td>No enviar correo electrónico masivo</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Calificación de la persona</td>
      <td>Calificación</td>
      <td>leader-qualitycode</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección 2</td>
      <td>Calle 2</td>
      <td>address1_line2</td>
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
      <td>No permitir faxes</td>
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
      <td>phone2</td>
    </tr>
    <tr>
      <td>Método De Contacto Preferido De Microsoft</td>
      <td>Método preferido de contacto</td>
      <td>preferredcontactmethods code</td>
    </tr>
    <tr>
      <td>Microsoft - Tema</td>
      <td>Tema</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>Última fecha interesante</td>
      <td>Última fecha interesante</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Último momento interesante desc</td>
      <td>Último momento interesante desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Última fuente de momento interesante</td>
      <td>Última fuente de momento interesante</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>Último tipo de momento interesante</td>
      <td>Último tipo de momento interesante</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Compañía</td>
      <td>Nombre de la compañía</td>
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
      <td>subject</td>
    </tr>
    <tr>
      <td>Ingresos anuales</td>
      <td>Ingresos anuales</td>
      <td>ingresos</td>
    </tr>
  </tbody>
</table>

Los campos de posibles clientes que se indican a continuación se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Propietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creado en</td>
      <td>creado</td>
    </tr>
  </tbody>
</table>

## Campos de contacto {#contact-fields}

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
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Microsoft - Fecha de creación</td>
      <td>Creado el</td>
      <td>creado</td>
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
      <td>lastname</td>
    </tr>
    <tr>
      <td>Correo electrónico</td>
      <td>Correo electrónico</td>
      <td>email address1</td>
    </tr>
    <tr>
      <td>Cargo</td>
      <td>Cargo</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Teléfono</td>
      <td>Teléfono comercial</td>
      <td>phone1</td>
    </tr>
    <tr>
      <td>Teléfono móvil</td>
      <td>Teléfono móvil</td>
      <td>mobilephone</td>
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
      <td>address1_stateorprovincia</td>
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
      <td>statcode</td>
    </tr>
    <tr>
      <td>Razón del estado</td>
      <td>Razón del estado</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>No llamar</td>
      <td>No permitir llamadas telefónicas</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Suscripción cancelada</td>
      <td>No enviar correo electrónico masivo</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección 2</td>
      <td>Dirección 1: Calle 2</td>
      <td>address1_line2</td>
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
      <td>phone2</td>
    </tr>
    <tr>
      <td>Método De Contacto Preferido De Microsoft</td>
      <td>Método Preferido De Contacto</td>
      <td>preferredcontactmethods code</td>
    </tr>
    <tr>
      <td>Última fecha interesante</td>
      <td>Última fecha interesante</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Último tipo de momento interesante</td>
      <td>Último tipo de momento interesante</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Última fuente de momento interesante</td>
      <td>Última fuente de momento interesante</td>
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
      <td>descripción </td>
    </tr>
    <tr>
      <td>Calificación de persona</td>
      <td>Puntaje del cliente potencial</td>
      <td>mkt_leader score</td>
    </tr>
    <tr>
      <td>Notas de la persona</td>
      <td>Descripción</td>
      <td>descripción </td>
    </tr>
  </tbody>
</table>

Los campos Contacto siguientes se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Propietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creado en</td>
      <td>creado</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Nombre de la compañía</td>
    </tr>
  </tbody>
</table>

## Campos de la cuenta {#account-fields}

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
      <th>Nombre de la API de MS Dynamics</th>
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
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft - Dirección de facturación 3</td>
      <td>Dirección 1: Calle 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Teléfono principal</td>
      <td>Teléfono principal</td>
      <td>phone1</td>
    </tr>
    <tr>
      <td>Tipo de negocio</td>
      <td>Tipo de negocio</td>
      <td>businessstypecode</td>
    </tr>
    <tr>
      <td>Número de cuenta de Microsoft</td>
      <td>Número de cuenta</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>Microsoft - Estado de la compañía</td>
      <td>Estado</td>
      <td>statcode</td>
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
      <td>industrycode</td>
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
      <td>numererofjobs</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Compañía</td>
      <td>name</td>
      <td>Nombre de la cuenta</td>
    </tr>
    <tr>
      <td>Cantidad de empleados</td>
      <td>Número de empleados</td>
      <td>numererofjobs</td>
    </tr>
  </tbody>
</table>

Los campos Cuenta siguientes se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Propietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creado en</td>
      <td>creado</td>
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
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Cerrar probabilidad</td>
      <td>Probablidad</td>
      <td>closeprobability</td>
    </tr>
    <tr>
      <td>Etapa</td>
      <td>status</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>Fecha de cierre real</td>
      <td>Fecha de cierre real</td>
      <td>actualclosedate</td>
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

Los campos Cuenta siguientes se sincronizan para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo de MS Dynamics</th>
      <th>Nombre de la API de MS Dynamics</th>
    </tr>
    <tr>
      <td>Propietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>Oportunidad</td>
      <td>idOportunidad</td>
    </tr>
    <tr>
      <td>Cliente potencial</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Campos del sistema relacionados con Microsoft en Marketo (solo lectura) {#microsoft-related-system-fields}

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
      <td>Fecha de creación en MS Dynamics (puede diferir de Creado en Marketo)</td>
    </tr>
    <tr>
      <td>Microsoft se elimina</td>
      <td>La persona solía estar en Microsoft, pero se eliminó y ahora solo reside en Marketo</td>
    </tr>
  </tbody>
</table>
