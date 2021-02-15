---
unique-page-id: 10617187
description: Explicación de la configuración de privacidad - Documentos de marketing - Documentación del producto
title: Explicación de la configuración de privacidad
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Explicación de la configuración de privacidad {#understanding-privacy-settings}

## Información general {#overview}

Marketing proporciona a los especialistas en mercadotecnia una manera de obtener el consentimiento de los visitantes Web para rastrearlos. Existen dos maneras de exclusión, o puede elegir que se le rastree mediante IP anónima.

* Los visitantes Web seleccionan la función No rastrear (DNT) en su explorador (y el especialista en mercadotecnia cumple la solicitud del visitante Web de No rastrear)
* Los visitantes Web utilizan una cookie exclusión proporcionada por un especialista en mercadotecnia en un sitio Web

O bien, el especialista en mercadotecnia puede realizar el seguimiento de los usuarios, pero puede utilizar una IP anónima.

Estos métodos pueden afectar al valor y la funcionalidad de Marketing en áreas específicas. Sin embargo, si el especialista en mercadotecnia *no cambia nada en la configuración de Marketing, la funcionalidad de Marketing sigue siendo la misma.*

## Configuración del explorador para no rastrear {#browser-settings-for-do-not-track}

Los visitantes Web pueden configurar su explorador para evitar el seguimiento por cualquier sitio Web seleccionando &quot;No rastrear&quot; (DNT). Esto evita el seguimiento de este navegador y dispositivo en particular. Consulte la configuración de privacidad del explorador para obtener más información.

En Munchkin, un especialista en mercadotecnia puede [decidir si admite o ignora la configuración de DNT del explorador](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

En Personalización web, un especialista en mercadotecnia puede decidir si [admite o ignora la configuración de DNT del explorador](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## exclusión desde un sitio Web específico {#opt-out-from-a-specific-website}

También puede permitir que los visitantes del sitio exclusión el seguimiento del sitio web desde el sitio web, independientemente de si **El explorador no realiza el seguimiento** está configurado o no. Esto permite al visitante del sitio especificar sus preferencias de seguimiento directamente desde el sitio web.

Para ello, debe agregar un parámetro a un vínculo exclusión en una página web que tenga habilitado el seguimiento de munchkin. Puede ser cualquier página web, pero el vínculo de la página web debe contener el siguiente parámetro:

?marketo_opt_out=true

A continuación se muestran ejemplos de una página web con un vínculo de exclusión y una página de aterrizaje para después de hacer clic en el vínculo. El tuyo variará.

Esta es una página web con un botón con el parámetro &quot;?marketo_opt_out=true&quot; en el vínculo de exclusión.

![](assets/opt-out-1.png)

Puede crear y publicar una página de aterrizaje como una página de seguimiento para cuando se haga clic en el vínculo con el parámetro &quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

Cuando se hace clic en el vínculo, Marketo agrega una cookie llamada **mkto_opt_out** al explorador del visitante que deshabilita el seguimiento de Munchkin para el visitante del sitio que hace clic en el vínculo con el parámetro anterior.

Para validar que la cookie se puede plantar, verifique que es un lead de cookie y haga clic en el vínculo. A continuación, compruebe las cookies del explorador para verificar que se agregó la cookie **mkto_opt_out**.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Actualmente, esto solo funciona con las versiones 152 y posteriores de Munchkin.

## adhesión {#opt-in}

Los especialistas en marketing pueden permitir que los usuarios adhesión mediante las funciones de Marketing en correos electrónicos, formularios, páginas de aterrizaje y otros métodos.

## Seguimiento mediante una IP anónima {#tracking-using-an-anonymized-ip}

Los especialistas en marketing pueden preservar la privacidad rastreando a los usuarios con una dirección IP anónima. Para hacerlo, agregue este código al RTP o al Javascript Munchkin que está incrustado en el sitio web.

* Para Munchkin, simplemente agregue {&quot;anonymizeIP&quot;,true} a la función init.

   >[!NOTE]
   >
   >El uso de este parámetro requiere que Munchkin V2 esté habilitado. Para habilitarla para su suscripción, póngase en contacto con [Asistencia técnica de marketing](https://nation.marketo.com/community/support_solutions).

* En Personalización web (RTP), agregue esto a javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
