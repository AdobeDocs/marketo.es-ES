---
description: Configuración de reCAPTCHA v3 - Documentos de Marketo - Documentación del producto
title: Configuración de reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Configuración de reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3 es una experiencia sin fricción que puntúa los envíos en función de lo sospechosos que sean sin utilizar desafíos de texto, imagen o botón. [Más información](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Recuperación del centro de datos y el ID de Munchkin {#retrieve-your-data-center-and-munchkin-id}

Para el paso 6 de la sección de configuración inicial de reCAPTCHA v3 a continuación, necesitará el centro de datos y el ID de Munchkin de su suscripción de Marketo Engage. Así es como se encuentran.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Clic **Mi cuenta**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Desplácese hacia abajo hasta Información de asistencia.

   ![](assets/setting-up-recaptcha-v3-3.png)

## Configuración inicial de reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Los siguientes pasos se realizan fuera de Marketo.

1. Ir a [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} y haga clic en el Admin Console v3.

1. Iniciar sesión o registrarse con una cuenta de Google.

1. Haga clic en el botón Crear (+) para crear una clave nueva.

1. Cree una etiqueta para identificar la clave que se va a utilizar para el Marketo Engage.

1. Elegir tipo **reCAPTCHA v3**. Actualmente, el Marketo Engage no admite reCAPTCHA v2.

1. Añada cada dominio que utilice la suscripción del Marketo Engage. Los dominios no establecidos aquí devolverán los errores en los formularios en los que reCAPTCHA esté habilitado. Recuerde reemplazar las palabras &quot;centro de datos&quot; y &quot;munchkinID&quot; por las palabras [datos de su suscripción](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * cualquier dominio de página de aterrizaje y alias configurados en la suscripción

   >[!NOTE]
   >
   >Por ejemplo, si el centro de datos de su cuenta es &quot;sjst&quot;, el dominio que lista de permitidos sería `app-sjst.marketo.com`. Si su ID de Munchkin es 123-ABC-789, el dominio que lista de permitidos sería `123-ABC-789.mktoweb.com`.

1. Establezca un propietario y una dirección de correo electrónico adicional que deban recibir alertas sobre este servicio.

1. Acepte los Términos de servicio de reCAPTCHA.

1. Clic **Enviar**.

   >[!NOTE]
   >
   >Mantenga a mano la clave del sitio y la clave secreta para la configuración del Marketo Engage.

## Configuración de CAPTCHA en el Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>Después de seguir estos pasos y [habilitar CAPTCHA en su primer formulario de Marketo](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}No obstante, asegúrese de probar el formulario inmediatamente, ya que cualquier tipo de configuración incorrecta en la configuración de reCAPTCHA puede romperlo.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Seleccionar **CAPTCHA** en el árbol.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Clic **Editar** en la configuración de CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Haga clic en el menú desplegable CAPTCHA y seleccione reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Inserte la Clave secreta y la Clave del sitio. Clic **Guardar** cuando termine.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Habilitar CAPTCHA en Marketo Forms](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
