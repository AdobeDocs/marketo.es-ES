---
unique-page-id: 4719314
description: Asignación de campo predeterminada de Salesforce - Documentos de marketing - Documentación de producto
title: Asignación de campo de Salesforce predeterminada
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Asignación de campo predeterminada de Salesforce {#default-salesforce-field-mapping}

Cuando inicialmente sincroniza su cuenta de Marketing con Salesforce, Marketing crea automáticamente estas asociaciones entre los campos integrados de Salesforce y Marketing. Marketo también sincronizará los campos personalizados de los posibles clientes, las cuentas, las oportunidades y los contactos.

## Campos de posibles clientes {#lead-fields}

| Campo SFDC | Campo Comercialización |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad | Ciudad |
| Compañía | Nombre de compañía |
| Fecha de conversión | Fecha de conversión de SFDC |
| País | País |
| Fecha de creación | Fecha de creación de SFDC |
| Descripción | Notas de persona |
| Correo electrónico | Dirección de correo electrónico |
| Fax | Número de fax |
| Nombre | Nombre |
| Exclusión correo electrónico | No suscrito |
| Industria | Industria |
| Convertido | SFDC convertido |
| Eliminado | SFDC se elimina |
| Apellido | Apellido |
| Origen de posible cliente | Origen |
| Puntuación de posible cliente | Puntuación |
| Teléfono móvil | Número de teléfono móvil |
| Empleados | Número de empleados |
| Teléfono | Número de teléfono |
| Código postal | Código postal |
| Clasificación | Clasificación |
| Saludo | Saludo |
| Estado/provincia | Estado |
| Estado | Estado |
| Calle | Dirección |
| Título | Puesto de trabajo |
| Sitio web | Sitio web |

## Campos de contacto {#contact-fields}

| Campo SFDC | Campo Comercialización |
|---|---|
| Fecha de nacimiento | Fecha de nacimiento |
| Fecha de creación | Fecha de creación de SFDC |
| Descripción de contacto | Notas de persona |
| Correo electrónico | Dirección de correo electrónico |
| Fax de empresa | Número de fax |
| Nombre | Nombre |
| Exclusión correo electrónico | No suscrito |
| Eliminado | SFDC se elimina |
| Apellido | Apellido |
| Origen de posible cliente | Origen |
| Puntuación de posible cliente | Puntuación |
| MailingCity | Ciudad |
| MailingCountry | País |
| MailingPostalCode | Código postal |
| MailingState | Estado |
| MailingStreet | Dirección |
| Teléfono móvil | Número de teléfono móvil |
| Teléfono de empresa | Número de teléfono |
| Saludo | Saludo |
| Título | Puesto de trabajo |

## Campos de cuenta {#account-fields}

| Campo SFDC | Campo Comercialización |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad de facturación | Ciudad de facturación |
| País de facturación | País de facturación |
| Código postal de facturación | Código postal de facturación |
| Estado o provincia de facturación | Estado de facturación |
| Calle de facturación | Dirección de facturación |
| Descripción de la cuenta | Notas de compañía |
| Industria | Industria |
| Eliminado | SFDC se elimina |
| Nombre de la cuenta | Nombre de compañía |
| Empleados | Número de empleados |
| Teléfono de la cuenta | Teléfono principal |
| Código SIC | Código SIC |
| Sitio de cuenta | Sitio |
| Tipo de cuenta | Tipo SFDC |
| Sitio web | Sitio web |

## Campos del sistema relacionados con Salesforce en Marketing (solo lectura) {#salesforce-related-system-fields-in-marketo-read-only}

Estos campos se crean en Marketing, pero los clientes no pueden ajustarlos.

| Campo | Descripción |
|---|---|
| Id. de SFDC | ID de Salesforce de 18 caracteres |
| Tipo SFDC | Posible cliente o contacto. Si está vacío, el lead existe solo como persona en Marketing |
| Fecha de creación de SFDC | Fecha de creación en SFDC (puede diferir de Creado en Marketing) |
| SFDC se elimina | Persona que solía estar en SFDC pero que fue eliminada y ahora solo vive en Marketing |
