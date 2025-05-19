---
unique-page-id: 1147091
description: Explicación de la pertenencia al programa - Documentos de Marketo - Documentación del producto
title: Explicación de la pertenencia al programa
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 93d6e498ee69a1a9fdee7956ac351764cf18a87a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Explicación de la pertenencia al programa {#understanding-program-membership}

>[!NOTE]
>
>**Definición:** Un miembro es una persona que tiene un estado en un programa.

## Cómo se convierten las personas en miembros de un programa {#how-people-become-members-of-a-program}

1. Una persona rellena un formulario [en una página de aterrizaje](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} del programa.

   * La persona tendrá automáticamente el primer estado de la progresión.

1. Usted [importa miembros al programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"} desde un archivo CSV.

   * La persona tendrá automáticamente el primer estado de la progresión.

1. Utiliza el paso de flujo [cambiar el estado del programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}.
1. Una persona se registra o asiste a un [seminario web sincronizado con un programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md){target="_blank"}.
1. Se ha [creado una persona mediante la aplicación de protección de Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md){target="_blank"}.
1. Se agrega una persona a una campaña de SFDC, que está [sincronizada con el programa](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}.

>[!NOTE]
>
>Para un programa de correo electrónico, una persona se agrega a la pertenencia solo cuando se envía el correo electrónico.

## Estados de programa {#program-statuses}

Los estados de los programas son los pasos que siguen las personas en un programa (por ejemplo, Invitado, Confirmado o Asistido, Sin presentación). Estos pasos los define el [canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Una persona no puede retroceder a un estado de programa anterior. La progresión del estado es solo de una manera.

## Estados de éxito {#success-statuses}

El propósito de un programa es crear una interacción significativa con la persona o el cliente potencial. El éxito se marca cuando una persona alcanza el estado que logra ese objetivo.

>[!NOTE]
>
>Para un seminario web, registrarse no es una interacción significativa si realmente no ve el seminario web. En este caso, atender es un éxito.

## Programa de adquisición {#acquisition-program}

Cuando un nuevo nombre entra en el sistema como miembro de un programa, Marketo establece automáticamente ese programa como &quot;adquisición&quot;. Esto establece el crédito de [atribución de primer toque](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Usar etiquetas en un programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/use-tags-in-a-program.md){target="_blank"}
>* [Crear un informe de rendimiento de programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md){target="_blank"}
