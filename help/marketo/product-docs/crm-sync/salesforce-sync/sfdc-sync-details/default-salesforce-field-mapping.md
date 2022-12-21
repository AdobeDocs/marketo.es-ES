---
unique-page-id: 4719314
description: Asignación de campos predeterminada de Salesforce - Documentos de Marketo - Documentación del producto
title: Asignación de campos de Salesforce predeterminada
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 53%

---

# Asignación de campos de Salesforce predeterminada {#default-salesforce-field-mapping}

Cuando sincroniza inicialmente su cuenta de Marketo con Salesforce, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Salesforce y Marketo. Marketo también sincronizará los campos personalizados de posibles clientes, cuentas, oportunidades y contactos.

## Campos de posibles clientes {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad | Ciudad |
| Compañía | Nombre de la compañía |
| Fecha convertida | Fecha de conversión de SFDC |
| País | País |
| Fecha de creación | Fecha de creación en SFDC |
| Descripción | Notas de la persona |
| Email | Dirección de email |
| Fax | Número de fax |
| Nombre | Nombre |
| No participar en el correo electrónico | Suscripción cancelada |
| Industria | Industria |
| Convertido | SFDC se convierte |
| Eliminado | SFDC eliminado |
| Apellido | Apellido |
| Origen del posible cliente | Origen |
| Puntaje del cliente potencial | Puntuación |
| Teléfono móvil | Número de teléfono móvil |
| Empleados | Cantidad de empleados |
| Teléfono | Número de teléfono |
| Código postal | Código postal |
| Calificación | Calificación |
| Saludo | Saludo |
| Estado/Provincia | Estado |
| Estado | Estado |
| Calle | Dirección |
| Título | Cargo |
| Sitio web | Sitio web |

## Campos de contacto {#contact-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Fecha de nacimiento | Fecha de nacimiento |
| Fecha de creación | Fecha de creación en SFDC |
| Descripción del contacto | Notas de la persona |
| Email | Dirección de email |
| Fax empresarial | Número de fax |
| Nombre | Nombre |
| No participar en el correo electrónico | Suscripción cancelada |
| Eliminado | SFDC eliminado |
| Apellido | Apellido |
| Origen del posible cliente | Origen |
| Puntaje del cliente potencial | Puntuación |
| MailingCity | Ciudad |
| MailingCountry | País |
| MailingPostalCode | Código postal |
| MailingState | Estado |
| MailingStreet | Dirección |
| Teléfono móvil | Número de teléfono móvil |
| Teléfono comercial | Número de teléfono |
| Saludo | Saludo |
| Título | Cargo |

## Campos de la cuenta {#account-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad de facturación | Ciudad de facturación |
| País de facturación | País de facturación |
| Código postal de facturación | Código postal de facturación |
| Estado/provincia de facturación | Estado de facturación |
| Calle de facturación | Dirección de facturación |
| Descripción de la cuenta | Notas de la compañía |
| Industria | Industria |
| Eliminado | SFDC eliminado |
| Nombre de la cuenta | Nombre de la compañía |
| Empleados | Cantidad de empleados |
| Teléfono de la cuenta | Teléfono principal |
| Código SIC | Código SIC |
| Sitio de la cuenta | Sitio |
| Tipo de cuenta | Tipo de SFDC |
| Sitio web | Sitio web |

## Campos del sistema relacionados con Salesforce en Marketo (solo lectura) {#salesforce-related-system-fields-in-marketo-read-only}

Estos campos se crean en Marketo, pero los clientes no pueden ajustarlos.

| Campo | Descripción |
|---|---|
| Identificación de SFDC | El ID de Salesforce de 18 caracteres |
| Tipo de SFDC | Posible cliente o contacto. Si está vacío, el posible cliente solo existe como persona en Marketo |
| Fecha de creación en SFDC | Fecha de creación en SFDC (puede diferir de Creado en Marketo) |
| SFDC se elimina | La persona solía estar en SFDC pero se eliminó y ahora solo reside en Marketo |
