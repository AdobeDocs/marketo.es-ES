---
description: 'Uso de mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes: Documentos de Marketo: documentación del producto'
title: Usar mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Usar mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Después de [crear un mensaje SMS de Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}, querrás usar déclencheur y filtros de listas inteligentes dentro de una campaña inteligente para obtener los beneficios. Así es como.

1. En Mi Marketo, haga clic en **[!UICONTROL Actividades de marketing]**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Elija una campaña inteligente en la que desee utilizar sus recursos SMS. Arrastre sobre un déclencheur. En este ejemplo utilizamos **Rellena el formulario**.

   ![](assets/fills-out-form-pull-over.jpg)

## DÉCLENCHEUR de SMS {#sms-triggers}

Hay otros déclencheur SMS disponibles. Los déclencheur SMS solo aparecen si el servicio Vibes está habilitado.

ENVIAR UN MENSAJE SMS:

* Actividades de marketing > elija Nueva campaña inteligente
   * Lista inteligente > Elegir lista de vibraciones filtro y lógica correcta > Lista de vibraciones: elija una lista de la lista desplegable (lista de bases de datos móviles que se sincroniza desde la plataforma de vibraciones)
      * Puede refinar la segmentación y utilizar déclencheur y filtros de correo electrónico y SMS dentro de una campaña
      * Filtros de vibraciones: suscripción a la lista de vibraciones frente a los miembros de la lista de vibraciones: la lógica es coherente con el correo electrónico
         * Suscrito a la lista de vibraciones: participantes que alguna vez se han suscrito a esa lista de vibraciones aunque ahora se hayan dado de baja.  - se utiliza principalmente para esfuerzos de marketing entre canales
            * Nota: Un mensaje SMS no se enviará a nadie que haya cancelado la suscripción si no está en la lista de la base de datos móvil de Vibes
         * Miembro de la lista de vibraciones: suscriptor activo y confirmado
         * Añadido a la lista: las listas de vibraciones no se rellenarán con este filtro; es para listas de Marketo

![](assets/new-sms-search2.png)

A continuación se muestran algunos ejemplos:

El déclencheur **Devoluciones de mensajes SMS** inicia un flujo, como enviar un correo electrónico, cuando se devuelve un mensaje SMS.

![](assets/sms-message-bounces-real.jpg)

El déclencheur **[!UICONTROL Suscribirse a la lista de vibraciones]** inicia un flujo cuando una persona se suscribe.

![](assets/subscribes-to-vibes-list-real.jpg)

El déclencheur **[!UICONTROL Clicks Link in SMS Message]** inicia un flujo cuando una persona hace clic en un vínculo del mensaje SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtros SMS {#sms-filters}

También puede utilizar los filtros de Vibes en las listas inteligentes. El filtro **[!UICONTROL Suscrito a la lista de vibraciones]** encuentra a cualquiera que se haya suscrito a vibraciones *alguna vez*. Esto incluye tanto a las personas sin suscribir como a las eliminadas, aunque estas se omitan del flujo. Este filtro es el más adecuado para los informes.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Por el contrario, el filtro **Lista de miembros de vibraciones** encuentra a _cualquiera_ suscrito actualmente a vibraciones y es el más adecuado para usarlo en campañas o listas inteligentes.

![](assets/image001.png)

>[!NOTE]
>
>Todos los filtros de SMS incluyen la restricción **[!UICONTROL Fecha de actividad]** de forma predeterminada.

Después de configurar los déclencheur y filtros de Vibes en tu lista inteligente, puedes [definir el flujo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definir lista inteligente para campaña inteligente | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Buscar y agregar filtros a una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
