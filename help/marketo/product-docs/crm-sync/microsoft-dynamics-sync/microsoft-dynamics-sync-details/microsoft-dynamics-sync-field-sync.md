---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronización de campos - Documentos de marketing - Documentación del producto
title: Sincronización de Microsoft Dynamics - Sincronización de campos
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronización de campos {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

La sincronización de marketing a Dynamics es muy potente. Aquí están los detalles.

## ¿Cómo se mantienen sincronizados los detalles de campo entre los dos sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La sincronización es bidireccional para entidades de contacto y posibles clientes. Si realiza cambios en un posible cliente o contacto en Dynamics o en una persona de Marketing, las actualizaciones se reflejarán en ambos sistemas.

Para las entidades de cuenta, usuario, oportunidad, equipo y personalizadas, la sincronización es unidireccional: Dinámica a Marketing. Si realiza cambios en estas entidades en Dynamics, las actualizaciones se reflejarán en Marketing.

## ¿Qué sucede si se realizan cambios en el mismo campo en ambos sistemas al mismo tiempo? (Colisión de datos) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Aunque esto es raro, Marketo ganará para las personas (posibles clientes) y Dynamics ganará para los contactos. Esto se debe a que consideramos que el departamento de mercadotecnia tiene autoridad para las personas, mientras que el sistema oficial de registro de contactos está en el departamento de ventas (CRM). Para las entidades de sincronización unidireccional, Dynamics siempre ganará.

## ¿Puedo crear un campo en Dynamics con Marketing? {#can-i-create-a-field-in-dynamics-using-marketo}

No, no se admite actualmente.

## He creado un campo en Dynamics. ¿Puedo sincronizarlo con Marketing? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sí, puede [sincronizar el campo](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) siempre que el usuario de sincronización tenga acceso a él en Dynamics.

¿Qué campos se sincronizarán con Marketing?

Puede [seleccionar los campos que sincronizar](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante la configuración.

## ¿Qué sucede si necesito agregar un campo personalizado después de sincronizar Marketing y Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Puede agregar campos en cualquier momento y esperar que los datos se actualicen de Dynamics a Marketing. Consulte [Uso de sincronización rápida con Microsoft Dynamics para ver un nuevo campo](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) personalizado para obtener más información.

>[!MORELIKETHIS]
>
>* [Usar sincronización rápida con Microsoft Dynamics para un nuevo campo personalizado](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



