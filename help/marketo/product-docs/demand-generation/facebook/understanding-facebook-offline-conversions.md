---
unique-page-id: 11383945
description: 'Explicación de las conversiones sin conexión de Facebook: documentos de Marketo: documentación del producto'
title: Explicación de las conversiones sin conexión de Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Explicación de [!DNL Facebook] conversiones sin conexión {#understanding-facebook-offline-conversions}

Las campañas de anuncios de posibles clientes de Facebook generan posibles clientes y los envían a Marketo para su uso en campañas de marketing. Sin embargo, sin visibilidad de las conversiones sin conexión, el anunciante de [!DNL Facebook] no puede saber qué anuncios son los más efectivos. A continuación se muestra un ejemplo.

>[!NOTE]
>
>**Ejemplo**
>
>[!UICONTROL Facebook Lead Ads] publica tres anuncios.
>
>* El anuncio 1 genera 20 posibles clientes
>* Ad 2 genera 30 posibles clientes
>* El anuncio 3 genera 50 posibles clientes
>
>Basándose únicamente en estos números, el Anuncio 3 parece el más efectivo.
>
>Sin embargo, cuando se ven los datos en el lado del Marketo, se desarrolla una historia diferente.
>
>* El anuncio 1 genera 10 ventas
>* El anuncio 3 genera 2 ventas
>
>Esto significa que el Anuncio 1, a pesar de generar menos posibles clientes, tuvo una tasa de éxito del 50 %, mientras que el Anuncio 3 apenas fue efectivo.
>
>Sin conversiones fuera de línea, el anunciante probablemente invertiría más dinero en el anuncio 3. Con los datos de conversión sin conexión, es más probable que el anunciante invierta en el anuncio 1.

Puede [configurar conversiones de Facebook sin conexión](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) para enviar el rendimiento de anuncios sin conexión a [!DNL Facebook].

1. Asegúrese de que la integración de [[!DNL Facebook] [!UICONTROL LaunchPoint]](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) esté actualizada.
1. Asignar fases del modelo del ciclo de ingresos a fases de conversión sin conexión en [!DNL Facebook].
1. Cuando se genera un posible cliente [!DNL Facebook] a partir de un anuncio de posible cliente [!DNL Facebook] y llega a una fase asignada, Marketo devuelve los datos de conversión sin conexión a [!DNL Facebook] varias veces al día mediante una API segura y automatizada. Los datos aparecen en el informe de [!DNL Facebook] Ads Manager.

>[!MORELIKETHIS]
>
>[Configurar [!DNL Facebook] conversiones sin conexión](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
