---
unique-page-id: 11378871
description: 'Uso de mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes: Documentos de Marketo: documentación del producto'
title: Usar mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
feature: Mobile Marketing
source-git-commit: 444a184e48bf7034c6e0ef277c9a4dd1fb33bd86
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Usar mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Después de usted [crear un mensaje SMS de Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), querrá usar filtros y déclencheur de listas inteligentes dentro de una campaña inteligente para obtener los beneficios. Así es como.

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Elija una campaña inteligente en la que desee utilizar su recurso SMS. Arrastre el cursor sobre un déclencheur, como el popular **Rellena el formulario**.

   ![](assets/fills-out-form-pull-over.jpg)

## DÉCLENCHEUR de SMS {#sms-triggers}

Hay otros déclencheur SMS disponibles. Los déclencheur SMS solo aparecen si el servicio Vibes está habilitado.

![](assets/new-sms-search2.png)

A continuación se muestran algunos ejemplos:

El déclencheur de mensajes SMS devueltos inicia un flujo, como el envío de un correo electrónico, cuando se devuelve un mensaje SMS.

![](assets/sms-message-bounces-real.jpg)

El **Suscribe a la lista de vídeos** El déclencheur inicia un flujo cuando una persona se suscribe.

![](assets/subscribes-to-vibes-list-real.jpg)

El **Vínculo de clics en el mensaje SMS** El déclencheur inicia un flujo cuando una persona hace clic en un vínculo del mensaje SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtros SMS {#sms-filters}

También puede utilizar los filtros de Vibes en las listas inteligentes. El **Suscrito a la lista de vídeos** El filtro encuentra a cualquiera que tenga *siempre* suscrito a Vibes. Esto incluye tanto a las personas sin suscribir como a las eliminadas, aunque estas se omitan del flujo. Este filtro es el más adecuado para los informes.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Por el contrario, la variable **Miembro de la lista de vibraciones** el filtro encuentra _cualquiera_ está suscrito a Vibes y es más adecuado para usarlo en campañas o listas inteligentes.

![](assets/image001.png)

>[!NOTE]
>
>Todos los filtros de SMS incluyen el **Fecha de la actividad** restricción de forma predeterminada.

Después de configurar los déclencheur y filtros de Vibes en la lista inteligente, puede [definición del flujo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definición de listas inteligentes para campañas inteligentes | DÉCLENCHEUR](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Buscar y agregar filtros a una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
