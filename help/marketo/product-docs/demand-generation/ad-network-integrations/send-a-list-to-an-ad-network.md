---
description: Envío de una lista a una red de publicidad - Documentos de Marketo - Documentación del producto
title: Enviar una lista a una red de anuncios
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 6%

---

# Enviar una lista a una red de anuncios {#send-a-list-to-an-ad-network}

Obtenga información sobre cómo enviar una lista estática a [!DNL LinkedIn], [!DNL Facebook] o Google.

## Cómo enviar una lista {#how-to-send-a-list}

1. En Marketo, selecciona tu lista, haz clic en la lista desplegable **[!UICONTROL Acciones de lista]** y selecciona **[!UICONTROL Enviar a la red de publicidad]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Elija entre [!DNL LinkedIn], [!DNL Facebook] o Google (las demás opciones no están disponibles en este momento). En este ejemplo, elegimos **[!DNL LinkedIn]**. Haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Haga clic en el menú desplegable **[!UICONTROL Audiencia]** y seleccione la audiencia que desee.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Si alguna vez necesita comprobarlo, puede ver la audiencia de destino a la que se sincroniza una lista a través de la pestaña Estado.

1. Elija su [!UICONTROL tipo push] deseado y haga clic en **[!UICONTROL Actualizar]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Si selecciona &quot;[!UICONTROL Habilitar la sincronización continua de audiencias]&quot;, Marketo mantiene la lista actualizada en la red de anuncios elegida a medida que cambia la lista en la instancia de Marketo. Ambos agregamos **y** quitamos personas de la audiencia si se agregan o eliminan de la lista estática.

1. ¡Y eso es todo! Haga clic en **[!UICONTROL Aceptar]** para salir.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Preguntas frecuentes {#faq}

**¿Se puede sincronizar una sola lista estática con varias audiencias de publicidad?**

No, una lista solo se puede sincronizar con una sola audiencia de destino.

**Si habilito la sincronización continua con una audiencia de publicidad existente, ¿se reemplazará la audiencia existente?**

No, la audiencia existente se agregará a, no se reemplazará.
