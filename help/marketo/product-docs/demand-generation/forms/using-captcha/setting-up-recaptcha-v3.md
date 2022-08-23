---
description: Configuración de reCAPTCHA v3 - Marketo Docs - Documentación del producto
title: Configuración de reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: cdc8d5f3322b9d19d50f9f4bd8156b7e3a627977
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Configuración de reCAPTCHA v3 {#setting-up-recaptcha-v3}

reCAPTCHA v3 es una experiencia sin fricciones que puntúa los envíos de formularios en función de lo sospechosos que sean sin utilizar el texto, la imagen o los botones. [Más información](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target=&quot;_blank&quot;}.

## Recuperar el centro de datos y el ID de Munchkin {#retrieve-your-data-center-and-munchkin-id}

Para el paso 6 de la sección de configuración inicial de reCAPTCHA v3 que aparece a continuación, necesitará el centro de datos y el ID de Munchkin de su suscripción al Marketo Engage. Así es como encontrarlos.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Haga clic en **Mi cuenta**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Desplácese hacia abajo hasta Información de asistencia.

   ![](assets/setting-up-recaptcha-v3-3.png)

## Configuración inicial de reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Los siguientes pasos se realizan fuera de Marketo.

1. Vaya a [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} y haga clic en el Admin Console v3.

1. Inicie sesión o regístrese con una cuenta de Google.

1. Haga clic en el botón Crear (signo +) para crear una clave nueva.

1. Cree una etiqueta para identificar la clave que se utilizará para el Marketo Engage.

1. Elegir tipo **reCAPTCHA v3**. Actualmente, el Marketo Engage no admite reCAPTCHA v2.

1. Añada cada dominio que utiliza la suscripción del Marketo Engage. Los dominios no configurados aquí devolverán errores en los formularios en los que se habilite reCAPTCHA. Recuerde reemplazar las palabras &quot;centro de datos&quot; y &quot;munchkinID&quot; por las palabras [datos de su suscripción](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * cualquier dominio y alias de página de aterrizaje configurado en la suscripción

   >[!NOTE]
   >
   >Por ejemplo, si el centro de datos de su cuenta es &quot;jst&quot;, el dominio que desea lista de permitidos sería `app-sjst.marketo.com`. Si su ID de Munchkin es 123-ABC-789, el dominio que lista de permitidos sería `123-ABC-789.mktoweb.com`.

1. Establezca un propietario y una dirección de correo electrónico adicional que deben recibir alertas sobre este servicio.

1. Acepte las condiciones de servicio de reCAPTCHA.

1. Haga clic en **Submit**.

>[!NOTE]
>
>Mantenga la clave del sitio y la clave secreta a mano para la configuración del Marketo Engage.

## Configuración de CAPTCHA en el Marketo Engage {#setting-up-captcha-in-marketo-engage}

1. En Marketo, haga clic en **Administrador**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Select **CAPTCHA** en el árbol.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Haga clic en **Editar** en la configuración de CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Haga clic en la lista desplegable CAPTCHA y seleccione reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Inserte la clave secreta y la clave del sitio. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/setting-up-recaptcha-v3-8.png)
