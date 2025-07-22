---
description: Configuración de reCAPTCHA v3 - Documentos de Marketo - Documentación del producto
title: Configuración de reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 2%

---

# Configurando [!UICONTROL reCAPTCHA v3] {#setting-up-recaptcha-v3}

ReCAPTCHA v3 es una experiencia sin fricción que puntúa los envíos en función de lo sospechosos que sean sin utilizar desafíos de texto, imagen o botón. [Más información](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Recupere su [!UICONTROL centro de datos] y [!UICONTROL ID de Munchkin] {#retrieve-your-data-center-and-munchkin-id}

Para el paso 6 de la sección de configuración inicial de [!UICONTROL reCAPTCHA v3] que figura a continuación, necesitarás el [!UICONTROL centro de datos] y el [!UICONTROL ID de Munchkin] de tu suscripción a Marketo Engage. Así es como se encuentran.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Haga clic en **[!UICONTROL Mi cuenta]**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Desplácese hacia abajo hasta [!UICONTROL Información de soporte técnico].

   ![](assets/setting-up-recaptcha-v3-3.png)

## Configuración inicial de [!UICONTROL reCAPTCHA v3] {#initial-recaptcha-v3-setup}

Los siguientes pasos se realizan fuera de Marketo.

1. Vaya a [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} y haga clic en la versión 3 de Admin Console.

1. Iniciar sesión o registrarse con una cuenta de Google.

1. Haga clic en el botón [!UICONTROL Crear] (+ signo) para crear una clave nueva.

1. Cree una etiqueta para identificar la clave que se va a utilizar para Marketo Engage.

1. Elija el tipo **[!UICONTROL reCAPTCHA v3]**. Marketo Engage no es compatible actualmente con reCAPTCHA v2.

1. Añada cada dominio que utilice la suscripción de Marketo Engage. Los dominios no establecidos aquí devolverán los errores en los formularios en los que reCAPTCHA esté habilitado. Recuerde reemplazar las palabras &quot;datacenter&quot; y &quot;munchkinID&quot; por los [datos de su suscripción](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * cualquier dominio de página de aterrizaje y alias configurados en la suscripción

   >[!NOTE]
   >
   >Por ejemplo, si [!UICONTROL Centro de datos] de su cuenta es &quot;sjst&quot;, el dominio que lista de permitidos sería `app-sjst.marketo.com`. Si su [!UICONTROL Munchkin ID] es 123-ABC-789, el dominio que lista de permitidos sería `123-ABC-789.mktoweb.com`.

1. Establezca un propietario y una dirección de correo electrónico adicional que deban recibir alertas sobre este servicio.

1. Acepte los Términos de servicio de reCAPTCHA.

1. Haga clic en **[!UICONTROL Enviar]**.

   >[!NOTE]
   >
   >Mantenga a mano la clave del sitio y la clave secreta para la configuración de Marketo Engage.

## Configuración de CAPTCHA en Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>Después de seguir estos pasos y [habilitar CAPTCHA en su primer formulario Marketo](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}, asegúrese de probar el formulario de inmediato, ya que cualquier tipo de configuración incorrecta en la configuración de reCAPTCHA puede romper el formulario.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Seleccione **[!UICONTROL CAPTCHA]** en el árbol.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Haz clic en **[!UICONTROL Editar]** en la configuración de [!UICONTROL CAPTCHA].

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Haga clic en el menú desplegable [!UICONTROL CAPTCHA] y elija [!UICONTROL reCAPTCHA v3].

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Inserte la **[!UICONTROL clave secreta]** y la **[!UICONTROL clave del sitio]**. Haga clic en **[!UICONTROL Guardar]** cuando termine.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Habilitar CAPTCHA en Marketo Forms](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
