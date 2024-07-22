---
unique-page-id: 4719316
description: Uso de cuentas de persona - Documentos de Marketo - Documentación del producto
title: Uso de cuentas de persona
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Uso de cuentas de persona {#using-person-accounts}

Las cuentas de persona se pueden configurar en Salesforce para adaptarse a las necesidades de su organización. Así trata el Marketo Engage las cuentas de las personas.

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

Utilice el filtro &quot;Es cuenta de persona&quot; de la lista inteligente para separar las cuentas de persona de las cuentas empresariales estándar.

## ¿Dónde se muestra la información de mis cuentas de persona en Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Las actividades relacionadas con cuentas de persona se muestran en el panel **[!UICONTROL Cuenta]**.

>[!NOTE]
>
>Las opciones **[!UICONTROL Añadir a Marketo Campaign]** y **[!UICONTROL Enviar correo electrónico]** de Marketo Sales Insight no están disponibles actualmente para las cuentas de persona.

## ¿Cómo asocio oportunidades a una cuenta de persona? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo depende de la función de contacto de la oportunidad para determinar a qué persona asociar la oportunidad. Debe agregar la función de contacto de oportunidad de cada cuenta de persona para conectar la oportunidad con la persona adecuada en Marketo. Se recomienda configurar un flujo de trabajo para agregar automáticamente la función de contacto de oportunidad.

## ¿Qué campo de correo electrónico debo usar para las cuentas de persona? {#which-email-field-should-i-use-for-person-accounts}

Hay dos campos de correo electrónico para una cuenta de persona. Utilice el campo **Dirección de correo electrónico** en sus formularios (no la **Dirección de correo electrónico de la persona**) para asegurarse de que la deduplicación de Marketo y otros procesos de correo electrónico funcionen correctamente.
