---
unique-page-id: 4719314
description: Asignación de campos de Salesforce predeterminada - Documentos de Marketo - Documentación del producto
title: Asignación de campos de Salesforce predeterminada
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 55%

---

# Asignación de campos de Salesforce predeterminada {#default-salesforce-field-mapping}

Al sincronizar inicialmente la cuenta de Marketo Engage con Salesforce, Marketo realiza automáticamente estas asociaciones entre los campos integrados de Salesforce y Marketo. Marketo también sincronizará los campos personalizados con los posibles clientes, las cuentas, las oportunidades y los contactos.

## Campos de clientes potenciales {#lead-fields}

| Campo de SFDC | Campo de Marketo |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad | Ciudad |
| Compañía | Nombre de la empresa |
| Fecha convertida | Fecha de conversión de SFDC |
| País | País |
| Fecha de creación | Fecha de creación en SFDC |
| Descripción | Notas de la persona |
| Correo electrónico | Dirección de email |
| Fax | Número de fax |
| Nombre | Nombre |
| No participar en el correo electrónico | Suscripción cancelada |
| Industria | Industria |
| Convertido | SFDC se ha convertido |
| Eliminado | SFDC eliminado |
| Apellido | Apellido |
| Origen del cliente potencial | Origen |
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

## Campos de contactos {#contact-fields}

| Campo de SFDC | Campo de Marketo |
|---|---|
| Birthdate | Fecha de nacimiento |
| Fecha de creación | Fecha de creación en SFDC |
| Descripción de contacto | Notas de la persona |
| Correo electrónico | Dirección de email |
| Fax del trabajo | Número de fax |
| Nombre | Nombre |
| No participar en el correo electrónico | Suscripción cancelada |
| Eliminado | SFDC eliminado |
| Apellido | Apellido |
| Origen del cliente potencial | Origen |
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

## Campos de cuentas {#account-fields}

| Campo de SFDC | Campo de Marketo |
|---|---|
| Ingresos anuales | Ingresos anuales |
| Ciudad de facturación | Ciudad de facturación |
| País de facturación | País de facturación |
| Código postal de facturación | Código postal de facturación |
| Estado o provincia de facturación | Estado de facturación |
| Calle de facturación | Dirección de facturación |
| Descripción de cuenta | Notas de la compañía |
| Industria | Industria |
| Eliminado | SFDC eliminado |
| Nombre de la cuenta | Nombre de la empresa |
| Empleados | Cantidad de empleados |
| Teléfono de cuenta | Teléfono principal |
| Código SIC | Código SIC |
| Sitio de cuenta | Sitio |
| Tipo de cuenta | Tipo de SFDC |
| Sitio web | Sitio web |

## Campos de sistema relacionados con Salesforce en Marketo (solo lectura) {#salesforce-related-system-fields-in-marketo-read-only}

Estos campos se crean en Marketo, pero los clientes no los pueden ajustar.

| Campo | Descripción |
|---|---|
| Identificación de SFDC | El ID de Salesforce de 18 caracteres |
| Tipo de SFDC | Posible cliente o contacto. Si está vacío, el posible cliente solo existe como persona en Marketo |
| Fecha de creación en SFDC | Fecha de creación en SFDC (puede ser diferente de Creación en Marketo) |
| Se ha eliminado el SFDC | La persona solía estar en SFDC, pero se ha eliminado y ahora solo vive en Marketo |
