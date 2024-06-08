---
unique-page-id: 4720758
description: 'Notas de la versión, enero de 2015, Documentos de Marketo: documentación del producto'
title: Notas de la versión, enero de 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Notas de la versión: enero de 2015 {#release-notes-january}

En la versión de enero de 2015 se incluyen las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition. Después del lanzamiento, asegúrese de volver para encontrar vínculos a artículos detallados para cada función.

## Actualizaciones de automatización de marketing {#marketing-automation-updates}

**Páginas de aterrizaje fáciles de móviles**

Ahora puede [crear vistas móviles para páginas de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) desde el editor de páginas de aterrizaje. Ofrezca su mensaje de forma eficaz independientemente del dispositivo y aumente la participación adaptando su contenido para facilitar el consumo sobre la marcha. Esta función se implementará gradualmente durante la semana siguiente al lanzamiento.

[-Vídeo de introducción a la página de aterrizaje-](https://youtu.be/aPQHlG2X6c0)

**Nuevas llamadas de API de REST**

Tres nuevas llamadas para la API de REST de posible cliente y actividad:

* Eliminar lead
* Obtener posibles clientes por ID de programa
* Obtener posibles clientes eliminados

Además, hay una nueva opción para Sincronizar posible cliente, para escribir el cambio de posible cliente asincrónicamente para una llamada de API más rápida. Todos los detalles estarán disponibles tras el lanzamiento en [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/home](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/home)

**Compatibilidad con objeto personalizado de scripts de correo electrónico**

Ahora, acceda a los objetos personalizados asociados con el objeto de cuenta desde los scripts de correo electrónico.

## Personalización en tiempo real {#real-time-personalization}

**Remarketing personalizado para Google y Facebook**

El remarketing muestra anuncios a personas que han visitado su sitio web. Ahora puede personalizar sus campañas de remarketing en [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) y [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) uso de datos de Real-Time Personalization. Remarketing para audiencias de diferentes industrias, listas de cuentas con nombre, tamaños de empresas o cualquier dato de posibles clientes conocidos.

[Módulo de lista de cuentas con nombre](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Las mejoras en el módulo Cuentas con nombre mejorarán las tasas de coincidencia y las validaciones para los usuarios. Las adiciones incluyen:

* Organizaciones coincidentes de la lista de cuentas con nombre mediante la dirección de correo electrónico del posible cliente (también para clientes solo RTP)
* Compatibilidad con hasta 100.000 registros por cuenta
* Plantilla de archivo CSV para ver y descargar

![](assets/image2015-1-14-11-3a12-3a16.png)

**Opciones de etiqueta RTP actualizadas**

Las opciones de la etiqueta RTP de Configuración de cuenta se han actualizado para incluir lo siguiente:

1. CDN y asincrónico (etiqueta recomendada)
1. CDN y sincrónico (alta velocidad)
1. Etiqueta asíncrona sin CDN
1. Etiqueta sincrónica sin CDN

Para obtener el mejor rendimiento, se recomienda colocar la etiqueta de en la parte superior del encabezado de la página web después de `<head>`. Todas las etiquetas permiten el uso de [API de RTP](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation). Para obtener información sobre cómo implementar la etiqueta RTP, consulte [aquí](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
