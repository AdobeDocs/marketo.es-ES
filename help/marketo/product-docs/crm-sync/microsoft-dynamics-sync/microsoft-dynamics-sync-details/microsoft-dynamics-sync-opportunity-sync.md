---
unique-page-id: 3571844
description: 'Sincronización de Microsoft Dynamics: sincronización de oportunidades, documentos de Marketo, documentación del producto'
title: 'Sincronización de Microsoft Dynamics: sincronización de oportunidad'
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Sincronización de [!DNL Microsoft Dynamics]: sincronización de oportunidad {#microsoft-dynamics-sync-opportunity-sync}

La sincronización de Marketo con [!DNL Dynamics] es muy eficaz. Estos son todos los detalles de la sincronización de oportunidades:

## ¿Cómo se sincronizan los detalles de las oportunidades entre los dos sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronización de oportunidades es de una manera: [!DNL Dynamics] a Marketo. Si realiza cambios en una oportunidad en [!DNL Dynamics], la actualización se reflejará en Marketo.

## ¿Puedo crear una oportunidad en [!DNL Dynamics] mediante Marketo? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

No, debe crear la oportunidad en [!DNL Dynamics] y se sincronizará automáticamente con Marketo.

## ¿Qué campos se sincronizarán con Marketo? {#what-fields-will-sync-to-marketo}

Puede [seleccionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante la instalación.

## ¿Cómo se asocia una cuenta/contacto a una oportunidad? {#how-is-an-account-contact-associated-with-an-opportunity}

El contacto o la cuenta se pueden asociar a una oportunidad de dos formas:

* Al crear una oportunidad, se puede establecer el campo Contacto (campo de búsqueda en el formulario para ponerse en contacto) o Cuenta (campo de búsqueda en el formulario para crear una cuenta). En cualquier caso, estos valores se almacenan en el campo Cliente potencial (customerid) en Dynamics. Este campo no aparece en el formulario de oportunidad, pero se puede añadir desde la configuración. Este campo solo puede contener 1 valor, ya sea contacto o cuenta. Marketo hace lo siguiente:

   * Si se establece el valor del contacto y la cuenta se deja vacía, Marketo crea un(a) `opportunitycontactrole` y establece la cuenta de la oportunidad en la cuenta del contacto. Si el contacto no tiene una cuenta, este campo se deja vacío.
   * Si el valor de la cuenta se establece y el contacto se deja vacío, Marketo solo establecerá la cuenta en la oportunidad de esta cuenta.
   * Si se establecen ambos valores, Dynamics elige la cuenta como valor para customerid, por lo que el comportamiento sería el mismo que arriba.

* A través de las partes interesadas: Dynamics utiliza conexiones para conectar oportunidades de contacto a través de partes interesadas desde la página de creación de oportunidades. Para esto, crearemos un registro `opportunitycontactrole` para cada nuevo inversor.
