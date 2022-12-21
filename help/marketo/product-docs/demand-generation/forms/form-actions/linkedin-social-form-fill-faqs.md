---
unique-page-id: 10098238
description: Preguntas frecuentes sobre el llenado de formularios de linkedIn Social - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre el llenado de formularios de linkedIn Social
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Preguntas frecuentes sobre el llenado de formularios de linkedIn Social {#linkedin-social-form-fill-faqs}

La directiva de API revisada de linkedIn nos obligaba a eliminar el Relleno de formularios sociales de LinkedIn de nuestro producto.

## Aspectos importantes que hay que saber {#important-things-to-know}

* Los botones de Relleno de formularios sociales de linkedIn ya no eran una opción para agregarlos a Marketo el 28 de abril de 2016

* Se ha eliminado el botón Relleno de formularios sociales de LinkedIn de todos los formularios que lo tenían activado

## ¿Por qué se ha eliminado esta funcionalidad de mi suscripción a Marketo? {#why-was-this-functionality-removed-from-my-marketo-subscription}

linkedIn ha realizado algunos cambios importantes en su programa para desarrolladores. Como parte de estos cambios, Marketo ya no es compatible con esta funcionalidad para los clientes.

## ¿Qué ha pasado si no eliminé los botones de Relleno de formularios sociales de LinkedIn de mis formularios que tenían activado Formulario social? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

El 28 de abril de 2016, se eliminó el botón Rellenar formularios sociales de LinkedIn de los formularios que aún tenían activado Formulario social .

## He estado insertando esta funcionalidad en los formularios desde que nos convertimos en clientes de Marketo. ¿Cómo sé qué formularios estaban usando LinkedIn Social Form Fill? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Antes de realizar este cambio, enviamos notificaciones semanales a la bandeja de entrada de las notificaciones con una lista de formularios que utilizaban LinkedIn Social Form Fill. Estas alertas estaban pensadas para ayudarle a identificar dónde utilizaba esta funcionalidad.

## ¿Siguen funcionando los botones de uso compartido en LinkedIn Social? {#do-linkedin-social-sharing-buttons-still-work}

Sí. El cambio solo afecta a la funcionalidad de relleno del formulario de LinkedIn Social .

## ¿Sigue funcionando el llenado de formularios sociales de Facebook y Twitter? {#do-facebook-and-twitter-social-form-fill-still-work}

Sí. El relleno del formulario social de facebook y Twitter no ha cambiado.

## ¿Ocurrió algo con los datos que ya capturamos a través de LinkedIn Social Form Fill? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

No, estos datos ya se habían almacenado en el registro de persona en Marketo y no se vieron afectados por este cambio.

## ¿Dónde puedo encontrar más información sobre la política de API de LinkedIn? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Siga este vínculo para obtener más información sobre los cambios que LinkedIn ha realizado en su política de API: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## ¿Cómo puedo ponerme en contacto con LinkedIn con preguntas? {#how-can-i-contact-linkedin-with-questions}

Siga este vínculo para ponerse en contacto con LinkedIn sobre sus soluciones de marketing: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Si Marketo eliminó esta funcionalidad de mis formularios el 28 de abril, ¿se pusieron en modo borrador mis formularios y las páginas de aterrizaje afectadas? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

No, los formularios de los que hemos eliminado esta funcionalidad permanecieron publicados.

## Si LinkedIn era la única red seleccionada, ¿cambiará el aspecto de mi formulario? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

No, solo se eliminará el botón LinkedIn del formulario. Siempre que se aplica Relleno de formulario social a un formulario, se crea un contenedor encima que contiene los botones Relleno de formulario social . Antes del 28 de abril de 2016, si LinkedIn era la única opción, el aspecto del contenedor se asemejaba a esta imagen:

![--](assets/one.png)

A partir del 28 de abril de 2016, ahora queda un contenedor vacío en la parte superior de cualquier formulario en el que se haya eliminado Relleno de formularios sociales de LinkedIn :

![--](assets/two.png)

>[!NOTE]
>
>Las imágenes anteriores son solo por ejemplo. Puede que no sea exactamente como se renderiza el contenedor de botones de relleno de formulario social. Cualquier color de fuente, estilo, etc. ha elegido influir en el aspecto del contenedor.

## Si LinkedIn era la única red seleccionada, ¿cómo puedo quitar el contenedor vacío encima del formulario? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

Para quitar el contenedor vacío, edite el formulario, seleccione Facebook o Twitter como opción para Relleno de formulario social y, a continuación, anule la selección de Facebook o Twitter como opción para Relleno de formulario social. Esto restablecerá las opciones sociales dentro del contenedor de relleno de formulario y lo quitará del formulario.
