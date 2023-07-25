---
unique-page-id: 11383945
description: 'Explicación de las conversiones sin conexión de Facebook: documentos de Marketo: documentación del producto'
title: Explicación de las conversiones sin conexión Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Explicación de las conversiones sin conexión Facebook {#understanding-facebook-offline-conversions}

Las campañas de facebook Lead Ads generan posibles clientes y los envían a Marketo para su uso en campañas de marketing. Sin embargo, sin visibilidad de las conversiones sin conexión, el anunciante de Facebook no puede saber qué anuncios son los más efectivos. A continuación se muestra un ejemplo.

>[!NOTE]
>
>**Ejemplo**
>
>Facebook Lead Ads publica tres anuncios.
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

Puede [Configuración de conversiones sin conexión de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) para enviar el rendimiento de anuncios sin conexión a Facebook.

1. Asegúrese de que su [Integración de facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) está actualizado.
1. Asigne fases en el modelo del ciclo de ingresos a las fases de conversión sin conexión en Facebook.
1. Cuando se genera un posible cliente de Facebook a partir de un anuncio de Facebook y este alcanza una fase asignada, Marketo devuelve los datos de conversión sin conexión a Facebook varias veces al día mediante una API segura y automatizada. Los datos aparecen en el informe Administrador de Facebook Ads.

>[!MORELIKETHIS]
>
>[Configurar conversiones sin conexión de Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
