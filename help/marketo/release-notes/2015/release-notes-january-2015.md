---
unique-page-id: 4720758
description: Notas de la versión - Enero de 2015 - Documentos de marketing - Documentación del producto
title: 'Notas de la versión: enero de 2015'
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Notas de la versión: Enero de 2015 {#release-notes-january}

Las siguientes funciones se incluyen en la versión de enero de 2015. Verifique la disponibilidad de las funciones en la edición de marketing. Después de la versión, asegúrese de volver a buscar vínculos a artículos detallados para cada función.

## Actualizaciones de automatización de mercadotecnia {#marketing-automation-updates}

**Nuevas fotos de Rick DeCosta!**

Rick es un cliente de Marketing de SmartBear y tiene una [increíble colección de fotos](https://www.flickr.com/photos/rickdecosta). ¡Échenlos!

## Páginas de aterrizaje fáciles de usar para dispositivos móviles {#mobile-friendly-landing-pages}

Ahora puede [crear vistas móviles para páginas de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) desde el editor de páginas de aterrizaje. Distribuya su mensaje de forma eficaz, independientemente del dispositivo, y aumente la participación adaptando su contenido para facilitar el consumo sobre la marcha. Esta función se despliega gradualmente durante la semana siguiente a la versión.

`<iframe width="420" height="315" src="//www.youtube-nocookie.com/embed/aPQHlG2X6c0" frameborder="0" allowfullscreen></iframe>`

**Nuevas llamadas de API de ReST**

Tres nuevas llamadas para la API de Lead &amp; Actividad ReST:

* Eliminar posible cliente
* Obtener posibles clientes por ID de Programa
* Obtener posibles clientes eliminados

Además, existe una nueva opción para sincronizar posible cliente, para escribir el cambio de posible cliente de forma asincrónica para una llamada de API más rápida. Los detalles completos estarán disponibles después de la versión en [developer.marketo.com](http://developers.marketo.com)

**Compatibilidad con objetos personalizados de secuencias de comandos de correo electrónico**

Ahora acceda a los objetos personalizados asociados con el objeto Account desde las secuencias de comandos de correo electrónico.

## Personalización en tiempo real {#real-time-personalization}

**Remercadotecnia personalizada para Google y Facebook**

La remercadotecnia muestra publicidades a las personas que han visitado el sitio web. Ahora puede personalizar sus campañas de remarketing en [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) y [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) con los datos de Personalización en tiempo real. Remercadotecnia a audiencias de diferentes industrias, listas de cuentas con nombre, tamaños de compañías o cualquier dato de posibles clientes conocidos.

[Módulo de Lista de cuentas con nombre](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Las mejoras en el módulo Cuentas con nombre mejorarán las tasas de coincidencia y las validaciones para los usuarios. Las adiciones incluyen:

* Organizaciones que coinciden desde la lista de cuenta con nombre mediante la dirección de correo electrónico del posible cliente (también para clientes solo RTP)
* Compatibilidad con hasta 100.000 registros por cuenta
* Plantilla de archivo CSV para vista y descarga

![](assets/image2015-1-14-11-3a12-3a16.png)

Opciones de etiqueta RTP actualizadas

[Las opciones de etiqueta](http://docs.marketo.com/display/docs/rtp+tag+implementation) RTP en Configuración de cuenta se han actualizado para incluir:

1. CDN y asincrónico (etiqueta recomendada)
1. CDN y sincrónico (alta velocidad)
1. Etiqueta asincrónica sin CDN
1. Etiqueta sincrónica sin CDN

Para un mejor rendimiento, se recomienda colocar la etiqueta en la parte superior del encabezado en la página web posterior `<head>`. Todas las etiquetas permiten el uso de la API [](http://developers.marketo.com/documentation/websites/rtp-js-api/)RTP. Para obtener información sobre cómo implementar la etiqueta RTP, consulte [aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
