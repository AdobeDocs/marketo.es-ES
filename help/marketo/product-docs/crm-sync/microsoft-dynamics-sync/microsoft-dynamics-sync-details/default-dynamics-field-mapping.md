---
description: 'Asignación de campos de Dynamics predeterminada: Marketo Docs - Documentación del producto'
title: Asignación de campos de Dynamics predeterminada
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Asignación predeterminada de campos de Dynamics {#default-dynamics-field-mapping}

Al sincronizar inicialmente la cuenta de Marketo con Microsoft, Marketo crea automáticamente estas asociaciones entre los campos integrados de Dynamics y Marketo.  Marketo también sincronizará los campos personalizados de posibles clientes, cuentas, oportunidades y contactos.

## Campos de posible cliente {#lead-fields}

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
   <td>Fecha de creación de Microsoft</td> 
   <td>Creado el</td> 
   <td>creado</td> 
  </tr> 
  <tr> 
   <td>Saludo</td> 
   <td>Saludo</td> 
   <td>salutación</td> 
  </tr> 
  <tr> 
   <td>First</td> 
   <td>Nombre</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Middle</td> 
   <td>Segundo nombre</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Última</td> 
   <td>Apellidos</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico</td> 
   <td>Correo electrónico</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Puesto de trabajo</td> 
   <td>Puesto de trabajo</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Teléfono</td> 
   <td>Teléfono empresarial</td> 
   <td>phone1</td> 
  </tr> 
  <tr> 
   <td>Móvil</td> 
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
   <td>Estado/provincia</td> 
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
   <td>Fuente de persona</td> 
   <td>Origen de posible cliente</td> 
   <td>leader sourccode</td> 
  </tr> 
  <tr> 
   <td>Estado de la persona</td> 
   <td>Estado</td> 
   <td>statcode</td> 
  </tr> 
  <tr> 
   <td>Motivo del estado</td> 
   <td>Motivo del estado</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>Notas de persona</td> 
   <td>Descripción</td> 
   <td>descripción</td> 
  </tr> 
  <tr> 
   <td>No llamar</td> 
   <td>No permitir llamadas telefónicas</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Cancelación de suscripción</td> 
   <td>No enviar correo electrónico masivo</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Clasificación de personas</td> 
   <td>Clasificación</td> 
   <td>leader-qualitycode</td> 
  </tr> 
  <tr> 
   <td>Dirección de Microsoft 2</td> 
   <td>Calle 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Dirección de Microsoft 3</td> 
   <td>Calle 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Email</td> 
   <td>No permitir correos electrónicos</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Fax</td> 
   <td>No permitir faxes</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Microsoft No Enviar Material De Marketing</td> 
   <td>Material de marketing</td> 
   <td>donotsendmm</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>Teléfono doméstico</td> 
   <td>phone2</td> 
  </tr> 
  <tr> 
   <td>Método De Contacto Preferido De Microsoft</td> 
   <td>Método preferido de contacto</td> 
   <td>preferredcontactmethods code</td> 
  </tr> 
  <tr> 
   <td>Tema de Microsoft</td> 
   <td>Tema</td> 
   <td>subject</td> 
  </tr> 
 </tbody> 
</table>

## Campos de contacto {#contact-fields}

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
   <td>Fecha de creación de Microsoft</td> 
   <td>Creado el</td> 
   <td>creado</td> 
  </tr> 
  <tr> 
   <td>Saludo</td> 
   <td>Saludo</td> 
   <td>salutación</td> 
  </tr> 
  <tr> 
   <td>First</td> 
   <td>Nombre</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Middle</td> 
   <td>Segundo nombre</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Última</td> 
   <td>Apellidos</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Correo electrónico</td> 
   <td>Correo electrónico</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Puesto de trabajo</td> 
   <td>Puesto de trabajo</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Teléfono</td> 
   <td>Teléfono empresarial</td> 
   <td>phone1</td> 
  </tr> 
  <tr> 
   <td>Móvil</td> 
   <td>Teléfono móvil</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>Dirección</td> 
   <td>Dirección 1: Calle 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>Ciudad</td> 
   <td>Dirección 1: Ciudad</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Estado</td> 
   <td>Dirección 1: Estado/provincia</td> 
   <td>address1_stateorprovincia</td> 
  </tr> 
  <tr> 
   <td>País</td> 
   <td>Dirección 1: País/región</td> 
   <td>address1_country</td> 
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
   <td>Motivo del estado</td> 
   <td>Motivo del estado</td> 
   <td>statuscode</td> 
  </tr> 
   <tr> 
   <td>No llamar</td> 
   <td>No permitir llamadas telefónicas</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Cancelación de suscripción</td> 
   <td>No enviar correo electrónico masivo</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Dirección de Microsoft 2</td> 
   <td>Dirección 1: Calle 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Dirección de Microsoft 3</td> 
   <td>Dirección 1: Calle 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Email</td> 
   <td>No permitir correos electrónicos</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>Teléfono doméstico</td> 
   <td>phone2</td> 
  </tr> 
  <tr> 
   <td>Método De Contacto Preferido De Microsoft</td> 
   <td>Método Preferido De Contacto</td> 
   <td>preferredcontactmethods code</td> 
  </tr> 
 </tbody> 
</table>

## Campos de cuenta {#account-fields}

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
   <td>Dirección 1: País/región</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Código postal de facturación</td> 
   <td>Dirección 1: Código postal</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Dirección de facturación de Microsoft 2</td> 
   <td>Dirección 1: Calle 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Dirección de facturación de Microsoft 3</td> 
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
   <td>Estado de la empresa Microsoft</td> 
   <td>Estado</td> 
   <td>statcode</td> 
  </tr> 
  <tr> 
   <td>Ingresos anuales</td> 
   <td>Ingresos anuales</td> 
   <td>ingresos</td> 
  </tr> 
  <tr> 
   <td>Notas de la empresa</td> 
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
 </tbody> 
</table>

## Campos del sistema relacionados con Microsoft en Marketo (solo lectura) {#microsoft-related-system-fields-in-marketo}

Estos campos se crean en Marketo, pero los clientes no pueden ajustarlos.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Campo Marketo</th> 
   <th>Descripción</th> 
  </tr> 
  <tr> 
   <td>Tipo de Microsoft</td> 
   <td>Posible cliente o contacto. Si está vacío, el posible cliente solo existe como persona en Marketo</td> 
  </tr> 
  <tr> 
   <td>Fecha de creación de Microsoft</td> 
   <td>Fecha de creación en MS Dynamics (puede diferir de Creado en Marketo)</td> 
  </tr> 
  <tr> 
   <td>Microsoft se elimina</td> 
   <td>Persona que solía estar en Microsoft pero que fue borrada y ahora solo vive en Marketo</td> 
  </tr> 
 </tbody> 
</table>
