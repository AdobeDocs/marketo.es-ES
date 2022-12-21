---
unique-page-id: 11378871
description: Utilizar mensajes SMS de vídeo en Déclencheur y filtros de listas inteligentes - Documentos de Marketo - Documentación del producto
title: Utilizar mensajes SMS de vídeo en Déclencheur y filtros de listas inteligentes
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Utilizar mensajes SMS de vídeo en Déclencheur y filtros de listas inteligentes {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Tras [crear un mensaje de SMS de vídeo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), querrá usar déclencheur de listas inteligentes y filtros dentro de una campaña inteligente para obtener los beneficios. Así es como.

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Elija una campaña inteligente en la que desee utilizar el recurso SMS. Arrastre un déclencheur, como el **Rellena el formulario**.

   ![](assets/fills-out-form-pull-over.jpg)

## DÉCLENCHEUR de SMS {#sms-triggers}

Hay otros déclencheur SMS disponibles. Los déclencheur SMS aparecen únicamente si está activado el servicio Vibes.

![](assets/new-sms-search2.png)

Estos son algunos ejemplos:

El déclencheur Devoluciones de mensajes SMS inicia un flujo, como el envío de un correo electrónico, cuando se genera un mensaje SMS.

![](assets/sms-message-bounces-real.jpg)

La variable **Suscripción a la lista de vídeos** déclencheur inicia un flujo cuando una persona se suscribe.

![](assets/subscribes-to-vibes-list-real.jpg)

La variable **Vínculo de clics en mensaje SMS** déclencheur inicia un flujo cuando una persona hace clic en un vínculo del mensaje SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtros SMS {#sms-filters}

También puede utilizar filtros de vídeo en listas inteligentes. La variable **Suscrito a la lista de vibraciones** filter encuentra a alguien que *ever* se suscribió a Vibes. Esto incluye tanto las personas que se han dado de baja como las que se han eliminado, aunque las personas eliminadas se omitan del flujo. Este filtro es el más adecuado para los informes.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Por el contrario, la variable **Miembro de la lista de vibraciones** encuentra filtro _any_ actualmente está suscrito a Vibes y es el más adecuado para su uso en campañas o listas inteligentes.

![](assets/image001.png)

>[!NOTE]
>
>Todos los filtros SMS incluyen la variable **Fecha de la actividad** de forma predeterminada.

Después de configurar los déclencheur y filtros de vídeo en la lista inteligente, puede [definir el flujo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definición de la lista inteligente para campañas inteligentes | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Buscar y agregar filtros a una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

