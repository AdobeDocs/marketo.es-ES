---
description: 'Uso de mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes: Documentos de Marketo: documentación del producto'
title: Usar mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 6b8c54dbe95c7bc6e2f68a48de11306f3f678cb6
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Usar mensajes SMS de Vibes en Déclencheur y filtros de listas inteligentes {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

NUEVO DOC

Después de usted [creación de un mensaje SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, querrá usar déclencheur y filtros de listas inteligentes dentro de una campaña inteligente para obtener las ventajas. Así es como.

1. En Mi Marketo, haga clic en **Actividades de marketing**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Elija una campaña inteligente en la que desee utilizar sus recursos SMS. Arrastre sobre un déclencheur. En este ejemplo utilizamos lo siguiente **Rellena el formulario**.

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

El **Devoluciones de mensajes SMS** El déclencheur inicia un flujo, como el envío de un correo electrónico, cuando se devuelve un mensaje SMS.

![](assets/sms-message-bounces-real.jpg)

El **Suscribe a la lista de vídeos** El déclencheur inicia un flujo cuando una persona se suscribe.

![](assets/subscribes-to-vibes-list-real.jpg)

El **Vínculo de clics en el mensaje SMS** El déclencheur inicia un flujo cuando una persona hace clic en un vínculo del mensaje SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtros SMS {#sms-filters}

También puede utilizar los filtros de Vibes en las listas inteligentes. El **Suscrito a la lista de vídeos** El filtro encuentra a cualquiera que tenga *siempre* suscrito a Vibes. Esto incluye tanto a las personas sin suscribir como a las eliminadas, aunque estas se omitan del flujo. Este filtro es el más adecuado para los informes.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Por el contrario, la variable **Miembro de la lista de vibraciones** el filtro encuentra _cualquiera_ está suscrito actualmente a Vibes y es más adecuado para usarlo en campañas inteligentes o listas.

![](assets/image001.png)

>[!NOTE]
>
>Todos los filtros de SMS incluyen el **Fecha de la actividad** restricción de forma predeterminada.

Después de configurar los déclencheur y filtros de Vibes en la lista inteligente, puede [definición del flujo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definición de listas inteligentes para campañas inteligentes | DÉCLENCHEUR](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Buscar y agregar filtros a una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
