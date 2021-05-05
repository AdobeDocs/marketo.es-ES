---
unique-page-id: 2950799
description: Información general sobre tokens - Documentos de Marketo - Documentación del producto
title: Información general sobre tokens
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
translation-type: tm+mt
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Información general de tokens {#tokens-overview}

Un token es una variable que se puede utilizar en pasos de flujo de campañas inteligentes de Marketo, correos electrónicos, páginas de aterrizaje, fragmentos y campañas web.

## Explicación de los valores predeterminados {#understanding-default-values}

Al utilizar un token, también desea proporcionar un valor predeterminado. Este es el texto que muestra si una persona no tiene un valor para el campo al que hace referencia.

![](assets/image2014-12-2-13-3a16-3a48.png)

En este ejemplo, el correo electrónico dirá &quot;Saludos, (nombre)&quot; o &quot;Saludos, terrling&quot; (valor predeterminado).

![](assets/two.png)

>[!CAUTION]
>
>Los tokens no funcionan en el encabezado previo al utilizar el editor de correo electrónico de Marketo. Para utilizar un token en el encabezado previo, debe hacerlo a través de su propio HTML en una plantilla de correo electrónico.

>[!NOTE]
>
>Esta lista no es exhaustiva. Los tokens también se crean para cada campo personalizado que tenga en Marketo.

## Tokens de persona {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* Los campos de persona personalizada también funcionan si utiliza su nombre para mostrar, por ejemplo, `{{lead.Custom Field Name}}`

## Tokens de empresa {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* Los campos personalizados de empresa también funcionan si utiliza su nombre para mostrar, por ejemplo. `{{Company.Custom Field Name}}`

## Tokens de campaña {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Tokens del sistema {#system-tokens}

>[!NOTE]
>
>Obtenga más información sobre estos tokens en el [Glosario de tokens del sistema](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Tokens de déclencheur {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>Encuentre más detalles sobre [tokens para momentos interesantes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) basados en los déclencheur utilizados en una campaña inteligente.

## Tokens de programa {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## Mis tokens {#my-tokens}

Mis tokens se definen dentro de un programa y comienzan por `{{my.` seguido del nombre que ha creado para el token. Obtenga más información sobre [Mis tokens en un programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Token de miembro {#member-token}

Los tokens de miembro se utilizan para insertar valores únicos de socios de servicios integrados. Un uso común de los tokens de miembro es para direcciones URL únicas para los asistentes a seminarios web. Cada persona tiene una dirección URL única para acceder al seminario web que se puede insertar con un token `{{member.webinar url}}`. El token `{{member.webinar url}}` resuelve automáticamente la URL de confirmación única de la persona generada por el proveedor de servicios.

* `{{member.webinar url}}`

>[!CAUTION]
>
>El token `{{member.webinar url}}` solo se rellenará si la campaña inteligente que envía el correo electrónico es un recurso secundario del Programa de eventos.
