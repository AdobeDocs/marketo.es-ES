---
description: Asignación de campos predeterminada de Veva - Documentos de Marketo - Documentación del producto
title: Asignación de campos de veeva predeterminada
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 38%

---

# Asignación de campos de veeva predeterminada {#default-veeva-field-mapping}

Cuando sincroniza inicialmente la cuenta de Marketo Engage con Veeva, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Veva y Marketo. Marketo también sincronizará los campos personalizados en sus cuentas y contactos.

## Campos de contacto {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo SFDC</th>
      <th>Campo Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fecha de nacimiento</td>
      <td>Fecha de nacimiento</td>
    </tr>
    <tr>
      <td>Fecha de creación</td>
      <td>Fecha de creación en SFDC</td>
    </tr>
    <tr>
      <td>Descripción del contacto</td>
      <td>Notas de la persona</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Dirección de email</td>
    </tr>
    <tr>
      <td>Fax empresarial</td>
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
      <td>Origen del lead</td>
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

## Campos de la cuenta {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo SFDC</th>
      <th>Campo Marketo</th>
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
      <td>Estado/provincia de facturación</td>
      <td>Estado de facturación</td>
    </tr>
    <tr>
      <td>Calle de facturación</td>
      <td>Dirección de facturación</td>
    </tr>
    <tr>
      <td>Descripción de la cuenta</td>
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
      <td>Teléfono de la cuenta</td>
      <td>Teléfono principal</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
    </tr>
    <tr>
      <td>Sitio de la cuenta</td>
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

## Campos del sistema relacionados con Veva en Marketo (solo lectura) {#veeva-related-system-fields-in-marketo}

Estos campos se crean en Marketo, pero los clientes no pueden ajustarlos.

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
      <td>Id De Véeva</td>
      <td>El ID de Salesforce de 18 caracteres</td>
    </tr>
    <tr>
      <td>Tipo de veeva</td>
      <td>Contacto. Si está vacío, el posible cliente solo existe como persona en Marketo</td>
    </tr>
    <tr>
      <td>Fecha de creación de Veeva</td>
      <td>Fecha de creación en SFDC (puede diferir de Creado en Marketo)</td>
    </tr>
    <tr>
      <td>Veva se elimina</td>
      <td>La persona solía estar en SFDC pero se eliminó y ahora solo reside en Marketo</td>
    </tr>
  </tbody>
</table>
