---
unique-page-id: 1147091
description: 'Explicación de la pertenencia al programa: Documentos de Marketo: Documentación del producto'
title: Explicación de la pertenencia al programa
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
source-git-commit: f6212795eec123265c6b6628da9974e97f9f7caf
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 1%

---

# Explicación de la pertenencia al programa {#understanding-program-membership}

>[!NOTE]
>
>Marketo ahora estandariza el idioma en todas las suscripciones, por lo que puede ver posibles clientes en su suscripción y personas o personas en docs.marketing.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Obtenga más información](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**Definición:** Un miembro es una persona que tiene un estado en un programa.

## Cómo las personas se convierten en miembros de un programa {#how-people-become-members-of-a-program}

1. Una persona rellena un [formulario en una página de aterrizaje](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) en el programa.

   1. Persona tendrá automáticamente el primer estado en la progresión.

1. You [importar miembros en el programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) de un archivo CSV.

   1. Persona tendrá automáticamente el primer estado en la progresión.

1. Utilice la variable [cambiar estado del programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) paso de flujo.
1. Una persona registra o asiste a un [seminario web sincronizado con un programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md).
1. Una persona es [creada con la aplicación de registro de Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. Se añade una persona a una campaña SFDC, que es [sincronizada con el programa](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>Para un programa de correo electrónico, una persona se añade a la pertenencia solo cuando se envía el correo electrónico.

## Estados del programa {#program-statuses}

Los estados del programa son los pasos que siguen las personas en un programa (por ejemplo, invitado, contestado, asistido, sin programa). Estos pasos se definen mediante la variable [canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Una persona no puede retroceder a un estado de programa anterior. La progresión del estado es de una sola manera.

## Estados de éxito {#success-statuses}

El objetivo de un programa es crear una interacción significativa con la persona o el cliente potencial. El éxito se marca cuando una persona alcanza el estado que logra ese objetivo.

>[!NOTE]
>
>Para un seminario web, registrarse no es una interacción significativa si realmente no ven el seminario web. La asistencia es un éxito en este caso.

## Programa de adquisición  {#acquisition-program}

Cuando un nuevo nombre entra en el sistema como miembro del programa, Marketo establece automáticamente ese programa como &quot;adquisición&quot;. Esto establece el crédito para [Atribución de primer toque](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [Uso de etiquetas en un programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [Crear un informe de rendimiento del programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

