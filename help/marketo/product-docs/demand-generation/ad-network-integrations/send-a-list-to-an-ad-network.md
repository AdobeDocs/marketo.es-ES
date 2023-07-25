---
description: Envío de una lista a una red de publicidad - Documentos de Marketo - Documentación del producto
title: Enviar una lista a una red de publicidad
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Enviar una lista a una red de publicidad {#send-a-list-to-an-ad-network}

Obtenga información sobre cómo enviar una lista estática a LinkedIn, Facebook o Google.

## Cómo enviar una lista {#how-to-send-a-list}

1. En Marketo, seleccione la lista y haga clic en **Enumerar acciones** y seleccione... **Enviar a la red de publicidad**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Elija entre LinkedIn, Facebook o Google (el resto de opciones no están disponibles en este momento). En este ejemplo, elegimos **LinkedIn**. Clic **Siguiente**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Haga clic en la lista desplegable Audiencia y seleccione la audiencia que desee.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Si alguna vez necesita comprobarlo, puede ver la audiencia de destino a la que se sincroniza una lista a través de la pestaña Estado.

1. Elija el tipo de push que desee y haga clic en **Actualizar**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Si selecciona &quot;Habilitar sincronización continua de audiencia&quot;, Marketo mantiene la lista actualizada en la red de publicidad elegida a medida que cambia la lista en la instancia de Marketo. Los dos añadimos **y** eliminar personas de la audiencia si se añaden o eliminan de la lista estática.

1. ¡Y eso es todo! Clic **OK** para salir.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Preguntas frecuentes {#faq}

**¿Se puede sincronizar una sola lista estática con varias audiencias de publicidad?**

No, una lista solo se puede sincronizar con una sola audiencia de destino.

**Si habilito la sincronización continua con una audiencia de publicidad existente, ¿se reemplazará la audiencia existente?**

No, la audiencia existente se agregará a, no se reemplazará.
