---
description: Asignación de campos Veeva predeterminada - Documentos de Marketo - Documentación del producto
title: Asignación de campos Veeva predeterminada
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 40%

---

# Asignación de campos Veeva predeterminada {#default-veeva-field-mapping}

Al sincronizar inicialmente la cuenta de Marketo Engage con Veeva, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Veeva y Marketo. Marketo también sincronizará los campos personalizados en sus cuentas y contactos.

## Campos de contactos {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo de SFDC</th>
      <th>Campo de Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Birthdate</td>
      <td>Fecha de nacimiento</td>
    </tr>
    <tr>
      <td>Fecha de creación</td>
      <td>Fecha de creación en SFDC</td>
    </tr>
    <tr>
      <td>Descripción de contacto</td>
      <td>Notas de la persona</td>
    </tr>
    <tr>
      <td>Correo electrónico</td>
      <td>Dirección de email</td>
    </tr>
    <tr>
      <td>Fax del trabajo</td>
      <td>Número de fax</td>
    </tr>
    <tr>
      <td>Nombre</td>
      <td>Nombre</td>
    </tr>
    <tr>
      <td>No participar en el correo electrónico</td>
      <td>Suscripción cancelada</td>
    </tr>
    <tr>
      <td>Eliminado</td>
      <td>SFDC eliminado</td>
    </tr>
    <tr>
      <td>Apellido</td>
      <td>Apellido</td>
    </tr>
    <tr>
      <td>Origen del cliente potencial</td>
      <td>Origen</td>
    </tr>
    <tr>
      <td>Puntaje del cliente potencial</td>
      <td>Puntuación</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>Ciudad</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>País</td>
    </tr>
    <tr>
      <td>MailingPostalCode</td>
      <td>Código postal</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>Estado</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>Dirección</td>
    </tr>
    <tr>
      <td>Teléfono móvil</td>
      <td>Número de teléfono móvil</td>
    </tr>
    <tr>
      <td>Teléfono comercial</td>
      <td>Número de teléfono</td>
    </tr>
    <tr>
      <td>Saludo</td>
      <td>Saludo</td>
    </tr>
    <tr>
      <td>Título</td>
      <td>Cargo</td>
    </tr>
  </tbody>
</table>

## Campos de cuentas {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo de SFDC</th>
      <th>Campo de Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ingresos anuales</td>
      <td>Ingresos anuales</td>
    </tr>
    <tr>
      <td>Ciudad de facturación</td>
      <td>Ciudad de facturación</td>
    </tr>
    <tr>
      <td>País de facturación</td>
      <td>País de facturación</td>
    </tr>
    <tr>
      <td>Código postal de facturación</td>
      <td>Código postal de facturación</td>
    </tr>
    <tr>
      <td>Estado o provincia de facturación</td>
      <td>Estado de facturación</td>
    </tr>
    <tr>
      <td>Calle de facturación</td>
      <td>Dirección de facturación</td>
    </tr>
    <tr>
      <td>Descripción de cuenta</td>
      <td>Notas de la compañía</td>
    </tr>
    <tr>
      <td>Industria</td>
      <td>Industria</td>
    </tr>
    <tr>
      <td>Eliminado</td>
      <td>SFDC eliminado</td>
    </tr>
    <tr>
      <td>Nombre de la cuenta</td>
      <td>Nombre de la compañía</td>
    </tr>
    <tr>
      <td>Empleados</td>
      <td>Cantidad de empleados</td>
    </tr>
    <tr>
      <td>Teléfono de cuenta</td>
      <td>Teléfono principal</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
    </tr>
    <tr>
      <td>Sitio de cuenta</td>
      <td>Sitio</td>
    </tr>
    <tr>
      <td>Tipo de cuenta</td>
      <td>Tipo de SFDC</td>
    </tr>
    <tr>
      <td>Sitio web</td>
      <td>Sitio web</td>
    </tr>
  </tbody>
</table>

## Campos del sistema relacionados con Veeva en Marketo (solo lectura) {#veeva-related-system-fields-in-marketo}

Estos campos se crean en Marketo, pero los clientes no los pueden ajustar.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Veeva Id</td>
      <td>El ID de Salesforce de 18 caracteres</td>
    </tr>
    <tr>
      <td>Tipo Veeva</td>
      <td>Contacto. Si está vacío, el posible cliente solo existe como persona en Marketo</td>
    </tr>
    <tr>
      <td>Fecha de creación de Veeva</td>
      <td>Fecha de creación en SFDC (puede ser diferente de Creación en Marketo)</td>
    </tr>
    <tr>
      <td>Veeva se ha eliminado</td>
      <td>La persona solía estar en SFDC, pero se ha eliminado y ahora solo vive en Marketo</td>
    </tr>
  </tbody>
</table>
