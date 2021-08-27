---
unique-page-id: 4719316
description: Uso de cuentas de persona - Documentos de Marketo - Documentación del producto
title: Uso de cuentas de persona
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Uso de cuentas de persona {#using-person-accounts}

Las cuentas de persona se pueden configurar en Salesforce para adaptarlas a las necesidades de su organización. Así es como Marketo trata las cuentas de personas.

>[!NOTE]
>
>Las cuentas predeterminadas de Salesforce son cuentas empresariales. El administrador de Salesforce debe configurar las cuentas de persona por separado.

## ¿Qué es una cuenta de persona? {#what-is-a-person-account}

Una cuenta de persona es muy similar al objeto de cuenta de Salesforce. Sin embargo, una cuenta de persona tiene acceso a los campos de cuenta y a los campos de contacto.

## ¿Qué sucede cuando se sincroniza una cuenta de persona con Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Una cuenta de persona se sincroniza con Marketo como empresa y como persona.

>[!NOTE]
>
>Los campos personalizados de una cuenta de persona se copian tanto en la empresa como en la persona en Marketo.

## ¿Cómo diferencio las cuentas de empresa y las cuentas de persona? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilice el filtro **Es cuenta de persona** de la lista inteligente para separar las cuentas de persona de las cuentas empresariales estándar.

## ¿Dónde se muestra la información de mis cuentas personales en Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Las actividades relacionadas con cuentas de persona se muestran en el panel **Cuenta**.

>[!NOTE]
>
>Las opciones **Add to Marketo Campaign** y **Send Email** de Marketo Sales Insight no están disponibles actualmente para cuentas de persona.

## ¿Cómo asocio oportunidades a una cuenta de persona? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo depende de la función de contacto de oportunidad para determinar a qué persona debe asociar la oportunidad. Debe añadir la función de contacto de oportunidad para cada cuenta de persona para conectar la oportunidad a la persona adecuada en Marketo. Se recomienda configurar un flujo de trabajo para añadir automáticamente la función de contacto de oportunidad.

## ¿Qué campo de correo electrónico debo usar para las cuentas de persona? {#which-email-field-should-i-use-for-person-accounts}

Hay dos campos de correo electrónico para una cuenta de persona. Utilice el campo **Email Address** de los formularios (no el **Person Email Address**) para garantizar que la deduplicación de Marketo y el procesamiento de otros correos electrónicos funcionen correctamente.
