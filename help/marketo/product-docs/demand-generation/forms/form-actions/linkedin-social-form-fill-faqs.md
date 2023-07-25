---
unique-page-id: 10098238
description: 'Preguntas frecuentes sobre el relleno de formularios sociales de linkedIn: documentos de Marketo, documentación del producto'
title: Preguntas frecuentes sobre linkedIn Social Form Fill
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Preguntas frecuentes sobre linkedIn Social Form Fill {#linkedin-social-form-fill-faqs}

La política de API revisada de linkedIn requería que elimináramos LinkedIn Social Form Fill de nuestro producto.

## Cosas importantes que saber {#important-things-to-know}

* Los botones de rellenado de formularios de linkedIn Social ya no eran una opción para agregarlos a Marketo el 28 de abril de 2016

* Se ha eliminado el botón Rellenar formulario social de LinkedIn de todos los formularios que lo tenían habilitado

## ¿Por qué se ha eliminado esta funcionalidad de mi suscripción a Marketo? {#why-was-this-functionality-removed-from-my-marketo-subscription}

LinkedIn ha realizado algunos cambios importantes en su programa para desarrolladores. Como parte de estos cambios, Marketo ya no puede admitir esta funcionalidad para los clientes.

## ¿Qué ha pasado si no he eliminado los botones de rellenado de formulario social de LinkedIn de mis formularios que tenían habilitado el formulario social? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

El 28 de abril de 2016, eliminamos el botón Rellenar formulario social de LinkedIn de los formularios que aún tenían habilitado el formulario social.

## He estado insertando esta funcionalidad en los formularios desde que nos convertimos en clientes de Marketo. ¿Cómo sé qué formularios utilizaban Rellenado de formularios de LinkedIn Social? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Antes de realizar este cambio, enviamos notificaciones semanales a su bandeja de entrada de notificaciones con una lista de formularios que utilizaban LinkedIn Social Form Fill. El objetivo de estas alertas era ayudarle a identificar dónde utilizaba esta funcionalidad.

## ¿Siguen funcionando los botones de uso compartido en redes sociales de LinkedIn? {#do-linkedin-social-sharing-buttons-still-work}

Sí. El cambio solo afecta a la funcionalidad LinkedIn Social Form Fill.

## ¿Facebook y Twitter Social Form Fill siguen funcionando? {#do-facebook-and-twitter-social-form-fill-still-work}

Sí. Facebook y el relleno de formulario social de Twitter no han cambiado.

## ¿Ha pasado algo con los datos que ya capturamos a través del rellenado del formulario social de LinkedIn? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

No, estos datos ya se almacenaron en el registro de persona en Marketo y no se vieron afectados por este cambio.

## ¿Dónde puedo encontrar más información sobre la política de API de LinkedIn? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Siga este vínculo para obtener más información sobre los cambios realizados por LinkedIn en su política de API: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## ¿Cómo puedo ponerme en contacto con LinkedIn si tengo alguna pregunta? {#how-can-i-contact-linkedin-with-questions}

Siga este vínculo para ponerse en contacto con LinkedIn en relación con sus soluciones de marketing: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Si Marketo quitó esta funcionalidad de mis formularios el 28 de abril, ¿mis formularios y las páginas de aterrizaje afectadas se pusieron en modo de borrador? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

No, los formularios de los que hemos eliminado esta funcionalidad siguen publicados.

## Si LinkedIn era la única red seleccionada, ¿cambiará el aspecto de mi formulario? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

No, solo se eliminará el botón LinkedIn del formulario. Siempre que se aplica Relleno de formulario social a un formulario, existe un contenedor creado encima que contiene los botones Relleno de formulario social. Antes del 28 de abril de 2016, si LinkedIn era la única opción, la apariencia del contenedor se parecía a esta imagen:

![--](assets/one.png)

Después del 28 de abril de 2016, ahora hay un contenedor vacío en la parte superior de cualquier formulario en el que se haya eliminado Rellenar formulario social de LinkedIn:

![--](assets/two.png)

>[!NOTE]
>
>Las imágenes anteriores son solo por ejemplo. Puede que no sea exactamente así como se representa el contenedor de botones Rellenar formulario social. Cualquier color de fuente, estilo, etc. ha elegido influenciar en el aspecto del contenedor.

## Si LinkedIn era la única red seleccionada, ¿cómo puedo quitar el contenedor vacío encima del formulario? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

Para quitar el contenedor vacío, edite el formulario, seleccione Facebook o Twitter como opción para Rellenar formulario social y, a continuación, anule la selección de Facebook o Twitter como opción para Rellenar formulario social. Esto restablecerá las opciones sociales dentro del contenedor de rellenado de formulario y lo quitará del formulario.
