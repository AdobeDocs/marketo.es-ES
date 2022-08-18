---
description: Configuración de reCAPTCHA v3 - Marketo Docs - Documentación del producto
title: Configuración de reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 24942664d613fa2851bad7a0dd3862027deacf37
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Configuración de reCAPTCHA v3 {#setting-up-recaptcha-v3}

Texto introductorio

## Configuración inicial de reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Texto: Describir v3: los siguientes pasos se realizan fuera del Marketo Engage.

1. Vaya a [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} y haga clic en el Admin Console v3.

1. Inicie sesión o regístrese con una cuenta de Google.

1. Haga clic en el botón Crear (signo +) para crear una clave nueva.

1. Cree una etiqueta para identificar la clave que se utilizará para el Marketo Engage.

1. Elegir tipo **reCAPTCHA v3**. Actualmente, el Marketo Engage no admite reCAPTCHA v2.

1. Añada cada dominio que utiliza la suscripción del Marketo Engage. Los dominios no configurados aquí devolverán errores en los formularios en los que se habilite reCAPTCHA.

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * cualquier dominio y alias de página de aterrizaje configurado en la suscripción

1. Establezca un propietario y una dirección de correo electrónico adicional que deben recibir alertas sobre este servicio.

1. Acepte las condiciones de servicio de reCAPTCHA.

1. Haga clic en **Submit**.

>[!NOTE]
>
>Mantenga la clave del sitio y la clave secreta a mano para la configuración del Marketo Engage.

## Configuración de CAPTCHA en el Marketo Engage {#setting-up-captcha-in-marketo-engage}

1. En Marketo, haga clic en **Administrador**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Select **CAPTCHA** en el árbol.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Haga clic en **Editar** en la configuración de CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-3.png)

1. Haga clic en la lista desplegable CAPTCHA y seleccione reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Inserte la clave secreta y la clave del sitio. Haga clic en **Guardar** cuando haya terminado.

   ![](assets/setting-up-recaptcha-v3-5.png)
