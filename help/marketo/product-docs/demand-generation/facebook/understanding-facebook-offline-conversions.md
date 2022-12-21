---
unique-page-id: 11383945
description: 'Explicación de las conversiones sin conexión de Facebook: Documentos de Marketo: Documentación del producto'
title: Explicación de las conversiones sin conexión de Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Explicación de las conversiones sin conexión de Facebook {#understanding-facebook-offline-conversions}

Las campañas de facebook Lead Ads generan posibles clientes y los envían a Marketo para su uso en campañas de marketing. Sin embargo, sin visibilidad de las conversiones sin conexión, el anunciante de Facebook no puede saber qué anuncios son los más efectivos. Aquí hay un ejemplo.

>[!NOTE]
>
>**Ejemplo**
>
>Facebook Lead Ads ejecuta tres anuncios.
>
>* El anuncio 1 genera 20 posibles clientes
>* El anuncio 2 genera 30 posibles clientes
>* El anuncio 3 genera 50 posibles clientes
>
>Basándose solo en estos números, el Ad 3 parece ser el más efectivo.
>
>Sin embargo, al mirar los datos del lado de Marketo, se desarrolla una historia diferente.
>
>* El anuncio 1 genera 10 ventas
>* El anuncio 3 genera 2 ventas
>
>Eso significa que el anuncio 1, a pesar de generar menos posibles clientes, tuvo una tasa de éxito del 50%, mientras que el anuncio 3 apenas fue efectivo.
>
>Sin conversiones fuera de línea, el anunciante probablemente invertiría más dinero en el anuncio 3. Con los datos de conversión sin conexión, es más probable que el anunciante invierta en el anuncio 1.

Puede [configuración de conversiones sin conexión de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) para enviar el rendimiento de la publicidad sin conexión a Facebook.

1. Asegúrese de que [Integración de facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) está actualizado.
1. Asigne etapas del modelo de ciclo de ingresos a las etapas de conversión sin conexión en Facebook.
1. Cuando se genera un posible cliente de Facebook a partir de un anuncio de posible cliente de Facebook y llega a una fase asignada, Marketo envía datos de conversión sin conexión a Facebook varias veces al día mediante una API segura y automatizada. Los datos aparecen en el informe Administrador de anuncios de Facebook.

>[!MORELIKETHIS]
>
>[Configuración de conversiones sin conexión de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
