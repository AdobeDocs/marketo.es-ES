---
unique-page-id: 4719316
description: Uso de cuentas de persona - Documentos de Marketo - Documentación del producto
title: Uso de cuentas de persona
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Uso de cuentas de persona {#using-person-accounts}

Las cuentas de persona se pueden configurar en Salesforce para adaptarse a las necesidades de su organización. Así es como Marketo trata las cuentas de personas.

>[!NOTE]
>
>Las cuentas predeterminadas de Salesforce son cuentas comerciales. El administrador de Salesforce debe configurar las cuentas de persona por separado.

## ¿Qué es una cuenta de persona? {#what-is-a-person-account}

Una cuenta de persona es muy similar al objeto de cuenta en Salesforce. Sin embargo, una cuenta de persona tiene acceso tanto a los campos de cuenta como a los de contacto.

## ¿Qué sucede cuando se sincroniza una cuenta de persona con Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Una cuenta de persona se sincroniza con Marketo como empresa y como persona.

>[!NOTE]
>
>Los campos personalizados de una cuenta de persona se copian tanto a la empresa como a la persona en Marketo.

## ¿Cómo diferencio las cuentas de empresa y las cuentas de persona? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilice el **Es cuenta de persona** filtre en la lista inteligente para separar las cuentas de persona de las cuentas empresariales estándar.

## ¿Dónde se muestra la información de mis cuentas de persona en Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Las actividades relacionadas con cuentas de persona se muestran en la variable **Cuenta** panel.

>[!NOTE]
>
>Datos de ventas de Marketo **Añadir a Marketo Campaign** y **Enviar correo electrónico** Las opciones de no están disponibles actualmente para cuentas de persona.

## ¿Cómo asocio oportunidades a una cuenta de persona? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo depende de la función de contacto de la oportunidad para determinar a qué persona asociar la oportunidad. Debe agregar la función de contacto de oportunidad de cada cuenta de persona para conectar la oportunidad con la persona adecuada en Marketo. Se recomienda configurar un flujo de trabajo para agregar automáticamente la función de contacto de oportunidad.

## ¿Qué campo de correo electrónico debo usar para las cuentas de persona? {#which-email-field-should-i-use-for-person-accounts}

Hay dos campos de correo electrónico para una cuenta de persona. Utilice el **Correo electrónico** en los formularios (no en el campo **Dirección de correo electrónico de persona**) para garantizar que la deduplicación de Marketo y otro procesamiento de correo electrónico funcionen correctamente.
