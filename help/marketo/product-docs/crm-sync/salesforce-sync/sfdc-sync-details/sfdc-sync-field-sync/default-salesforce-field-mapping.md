---
unique-page-id: 4719314
description: Asignación de campos predeterminada de Salesforce - Documentos de Marketo - Documentación del producto
title: Asignación de campos de Salesforce predeterminada
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Asignación de campos predeterminada de Salesforce {#default-salesforce-field-mapping}

Cuando sincroniza inicialmente su cuenta de Marketo con Salesforce, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Salesforce y Marketo. Marketo también sincronizará los campos personalizados de posibles clientes, cuentas, oportunidades y contactos.

## Campos de posible cliente {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad | Ciudad |
| Empresa | Nombre de la empresa |
| Fecha convertida | Fecha convertida de SFDC |
| País | País |
| Fecha de creación | Fecha de creación de SFDC |
| Descripción | Notas de persona |
| Correo electrónico | Dirección de correo electrónico |
| Fax | Número de fax |
| Nombre | Nombre |
| Opción de exclusión de correo electrónico | Cancelación de suscripción |
| Industria | Industria |
| Convertido | SFDC se convierte |
| Eliminado | SFDC se elimina |
| Apellidos | Apellidos |
| Origen de posible cliente | Fuente |
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

| Campo SFDC | Campo Marketo |
|---|---|
| Fecha de nacimiento | Fecha de nacimiento |
| Fecha de creación | Fecha de creación de SFDC |
| Descripción del contacto | Notas de persona |
| Correo electrónico | Dirección de correo electrónico |
| Fax empresarial | Número de fax |
| Nombre | Nombre |
| Opción de exclusión de correo electrónico | Cancelación de suscripción |
| Eliminado | SFDC se elimina |
| Apellidos | Apellidos |
| Origen de posible cliente | Fuente |
| Puntuación de posible cliente | Puntuación |
| MailingCity | Ciudad |
| MailingCountry | País |
| MailingPostalCode | Código postal |
| MailingState | Estado |
| MailingStreet | Dirección |
| Teléfono móvil | Número de teléfono móvil |
| Teléfono empresarial | Número de teléfono |
| Saludo | Saludo |
| Título | Puesto de trabajo |

## Campos de cuenta {#account-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad de facturación | Ciudad de facturación |
| País de facturación | País de facturación |
| Código postal de facturación | Código postal de facturación |
| Estado/provincia de facturación | Estado de facturación |
| Calle de facturación | Dirección de facturación |
| Descripción de la cuenta | Notas de la empresa |
| Industria | Industria |
| Eliminado | SFDC se elimina |
| Nombre de la cuenta | Nombre de la empresa |
| Empleados | Número de empleados |
| Teléfono de la cuenta | Teléfono principal |
| Código SIC | Código SIC |
| Sitio de la cuenta | Sitio |
| Tipo de cuenta | Tipo de SFDC |
| Sitio web | Sitio web |

## Campos del sistema relacionados con Salesforce en Marketo (solo lectura) {#salesforce-related-system-fields-in-marketo-read-only}

Estos campos se crean en Marketo, pero los clientes no pueden ajustarlos.

| Campo | Descripción |
|---|---|
| SFDC Id | El ID de Salesforce de 18 caracteres |
| Tipo de SFDC | Posible cliente o contacto. Si está vacío, el posible cliente solo existe como persona en Marketo |
| Fecha de creación de SFDC | Fecha de creación en SFDC (puede diferir de Creado en Marketo) |
| SFDC se elimina | La persona solía estar en SFDC pero se eliminó y ahora solo reside en Marketo |
