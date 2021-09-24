---
unique-page-id: 4720758
description: 'Notas de la versión, enero de 2015: Documentos de Marketo: Documentación del producto'
title: Notas de la versión, enero de 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 1%

---

# Notas de la versión: Enero de 2015 {#release-notes-january}

Las siguientes funciones se incluyen en la versión de enero de 2015. Compruebe la disponibilidad de las funciones en Marketo Edition. Después de la versión, asegúrese de volver para encontrar vínculos a artículos detallados para cada función.

## Actualizaciones de automatización de marketing {#marketing-automation-updates}

**Páginas de aterrizaje fáciles de usar en dispositivos móviles**

Ahora puede [crear vistas móviles para páginas de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) desde el editor de páginas de aterrizaje. Entregue su mensaje de forma eficaz, independientemente del dispositivo y aumente la participación adaptando su contenido para facilitar el consumo en cualquier momento. Esta función se implementará gradualmente durante la semana siguiente a la publicación.

[-Vídeo de información guiada de la página de aterrizaje-](https://youtu.be/aPQHlG2X6c0)

**Nuevas llamadas a la API Rest**

Tres nuevas llamadas para la API de Lead &amp; Activity ReST:

* Eliminar lead
* Obtener posibles clientes por ID de programa
* Obtener posibles clientes eliminados

Además, existe una nueva opción para el posible cliente de sincronización, para escribir el cambio de posible cliente asincrónicamente y así realizar una llamada API más rápida. Los detalles completos estarán disponibles después de la versión en [developers.marketo.com](https://developers.marketo.com)

**Compatibilidad con objetos personalizados con secuencias de comandos de correo electrónico**

Ahora acceda a los objetos personalizados asociados con el objeto Account desde dentro de las secuencias de comandos de correo electrónico.

## Personalización en tiempo real {#real-time-personalization}

**Remarketing personalizado para Google y Facebook**

El remarketing muestra anuncios a las personas que han visitado el sitio web. Ahora puede personalizar sus campañas de remarketing en [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) y [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) utilizando los datos de la personalización en tiempo real. Remarquete a audiencias de diferentes industrias, listas de cuentas con nombre, tamaños de empresa o cualquier dato de posibles clientes conocidos.

[Módulo de lista de cuentas con nombre](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Las mejoras en el módulo Cuentas con nombre mejorarán las tasas de coincidencia y las validaciones para los usuarios. Las adiciones incluyen:

* Coincidencia de organizaciones de la lista de cuentas con nombre mediante la dirección de correo electrónico del posible cliente (también para clientes solo RTP)
* Compatibilidad con hasta 100.000 registros por cuenta
* Plantilla de archivo CSV para ver y descargar

![](assets/image2015-1-14-11-3a12-3a16.png)

**Opciones de etiqueta RTP actualizadas**

Las opciones de etiqueta RTP en Configuración de cuenta se han actualizado para incluir:

1. CDN y asíncrono (etiqueta recomendada)
1. CDN y sincrónico (alta velocidad)
1. Etiqueta asíncrona sin CDN
1. Etiqueta sincrónica sin CDN

Para obtener el mejor rendimiento, se recomienda colocar la etiqueta en la parte superior del encabezado en la página web después de `<head>`. Todas las etiquetas permiten el uso de la [API RTP](https://developers.marketo.com/documentation/websites/rtp-js-api/). Para obtener información sobre cómo implementar la etiqueta RTP, consulte [aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
