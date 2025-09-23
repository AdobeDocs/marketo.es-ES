---
unique-page-id: 2953459
description: 'Sincronización de SFDC: sincronización de cuentas, documentos de Marketo: documentación del producto'
title: 'Sincronización de SFDC: sincronización de cuenta'
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# Sincronización de SFDC: sincronización de cuentas {#sfdc-sync-account-sync}

Marketo también sincroniza la información de su cuenta con [!DNL Salesforce]. ¡Aquí hay algunas cosas específicas que debe saber!

## ¿En qué sentido se sincroniza la información? {#which-way-does-the-information-sync}

Solo una forma: de SFDC a Marketo.

## ¿Cómo funcionan las actualizaciones? {#how-do-the-updates-work}

Si actualiza un campo Cuenta para un contacto en Marketo, cambia los valores de todos los contactos que pertenecen a esa cuenta en Marketo. No se sincroniza con SFDC. Sin embargo, la próxima vez que esa cuenta se actualice en SFDC, los cambios anularán toda la información de la cuenta en Marketo.

## ¿Puede un contacto pertenecer a varias cuentas?  {#can-a-contact-belong-to-multiple-accounts}

No. Una cuenta puede tener muchos contactos, un contacto solo puede tener una cuenta.

## ¿Puedo crear cuentas desde Marketo? {#can-i-create-accounts-from-marketo}

En su mayoría, no. Sin embargo, si usa el paso de flujo [Convertir persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} en una persona, se creará un nuevo contacto, una nueva cuenta y una nueva oportunidad.

>[!CAUTION]
>
>Este paso de flujo tiene un caso de uso muy limitado. Si no estás seguro, probablemente no deberías usarlo.

## ¿Un cambio en un campo de cuenta de [!DNL Salesforce] genera un registro de actividad Cambiar valor de datos para cada contacto?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Sobre todo, sí. Sin embargo, si una cuenta tiene más de 5000 contactos y un campo en esa cuenta cambia en SFDC, sincronizamos el cambio, pero no registramos la actividad de más de 5000 contactos.
