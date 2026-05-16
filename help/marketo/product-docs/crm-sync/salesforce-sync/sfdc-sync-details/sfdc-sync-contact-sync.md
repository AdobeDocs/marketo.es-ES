---
unique-page-id: 2953457
description: Obtenga información acerca de cómo funciona la sincronización de contactos entre Salesforce y Marketo. Comprenda la sincronización bidireccional, convierta a las personas en contactos y fuerce la sincronización con acciones de flujo.
title: 'Sincronización de SFDC: sincronización de contactos'
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/bddyM2G50v-Hgdy1oHw8xIPw1zij-2JvGSU7se3-UfI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 1%

---

# Sincronización de SFDC: sincronización de contactos {#sfdc-sync-contact-sync}

Marketo sincroniza toda la base de datos con [!DNL Salesforce]. Se sincroniza, luego espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días. A continuación se proporcionan algunos detalles acerca de cómo Marketo trata específicamente a [!DNL Salesforce] contactos.

## Dirección de sincronización {#sync-direction}

La sincronización de contactos es bidireccional. Si realiza cambios en un contacto en [!DNL Salesforce] o Marketo, las actualizaciones se reflejarán en ambos sistemas.

## ¿Qué sucede si se realizan cambios en ambos sistemas al mismo tiempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Somos amables y dejamos que [!DNL Salesforce] gane. Es poco frecuente que se produzca este tipo de colisión de datos.

## ¿Puedo convertir a una persona en un contacto en Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sí, usar la acción de flujo **[Convertir persona](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>Convertir a una persona en Marketo resultará en una nueva cuenta y oportunidad en [!DNL Salesforce]. Si no desea duplicar cuentas, use [!DNL Salesforce] para convertir.

## ¿Puedo forzar manualmente una sincronización de un contacto? {#can-i-manually-force-a-sync-of-a-contact}

Sí, usar la acción de flujo **[Sincronizar persona con SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** y se sincronizará en tiempo real.

## ¿Se sincronizan todos y cada uno de los campos estándar con Marketo? {#does-every-single-standard-field-sync-to-marketo}

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización de Marketo tenga acceso.

## ¿Marketo respetará las reglas de validación de [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Sí, si hay un conflicto, registrará el resultado en el registro de actividad de posibles clientes.
