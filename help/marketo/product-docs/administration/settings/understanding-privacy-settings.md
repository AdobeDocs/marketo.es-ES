---
unique-page-id: 10617187
description: 'Explicación de la configuración de privacidad: Documentos de Marketo: Documentación del producto'
title: Información sobre la configuración de privacidad
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Información sobre la configuración de privacidad {#understanding-privacy-settings}

## Resumen {#overview}

Marketo proporciona a los especialistas en marketing una forma de obtener el consentimiento de los visitantes web para rastrearlos. Existen dos formas de exclusión o puede elegir que se le rastree mediante una IP anónima.

* Los visitantes web seleccionan la función No rastrear (DNT) en su navegador (y el especialista en marketing acepta la solicitud del visitante web de No rastrear)
* Los visitantes web utilizan una cookie de exclusión proporcionada por un especialista en marketing en un sitio web

O bien, el especialista en marketing puede rastrear usuarios, pero usar una IP anónima.

Estos métodos pueden afectar al valor y la funcionalidad de Marketo en áreas específicas. Sin embargo, si el experto en marketing *no* si cambia cualquier cosa en la configuración de Marketo, la funcionalidad de Marketo permanece igual.

## Configuración del explorador para No rastrear {#browser-settings-for-do-not-track}

Los visitantes web pueden configurar su navegador para evitar el seguimiento por cualquier sitio web eligiendo &quot;No rastrear&quot; (DNT). Esto evita el seguimiento de este navegador y dispositivo en particular. Consulte la configuración de privacidad del explorador para obtener más información.

En Munchkin, un comerciante puede [decidir si admite o ignora la configuración DNT del navegador](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

En la personalización web, un especialista en marketing puede decidir si [admiten o ignoran la configuración de DNT del navegador](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Exclusión de un sitio web específico {#opt-out-from-a-specific-website}

También puede permitir que los visitantes del sitio excluyan el seguimiento del sitio web, independientemente de si lo desean o no **El explorador no rastrea** están configuradas. Esto permite al visitante del sitio especificar sus preferencias de seguimiento directamente desde el sitio web.

Para ello, debe añadir un parámetro a un vínculo de exclusión en una página web que tenga habilitado el seguimiento de munchkin. Puede ser cualquier página web, pero el vínculo de la página web debe contener el siguiente parámetro:

?marketing_opt_out=true

A continuación se muestran ejemplos de una página web con un vínculo de no participación y una página de aterrizaje para después de hacer clic en el vínculo. El tuyo variará.

Aquí hay una página web con un botón con el parámetro &quot;?marketo_opt_out=true&quot; en el vínculo de exclusión.

![](assets/opt-out-1.png)

Puede crear y publicar una página de aterrizaje como página de seguimiento cuando haga clic en el vínculo con el parámetro &quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

Cuando se hace clic en el vínculo, Marketo agrega una cookie llamada **mkto_opt_out** al explorador del visitante que deshabilita el seguimiento de Munchkin para el visitante del sitio que hace clic en el vínculo con el parámetro anterior.

Para validar que la cookie se puede plantar, compruebe que es un posible cliente con cookies y haga clic en el vínculo . A continuación, compruebe las cookies del explorador para comprobar que la variable **mkto_opt_out** se ha añadido la cookie .

![](assets/opt-out-3.png)

>[!NOTE]
>
>Actualmente, esto solo funciona con las versiones 152 y posteriores de Munchkin.

## Opt-in {#opt-in}

Los especialistas en marketing pueden permitir a los usuarios activar la opción mediante las funciones de Marketo en correos electrónicos, formularios, páginas de aterrizaje y otros métodos.

## Seguimiento con una IP anónima {#tracking-using-an-anonymized-ip}

Los especialistas en marketing pueden preservar la privacidad haciendo un seguimiento de los usuarios con una dirección IP anónima. Para ello, añada este código al Javascript RTP o Munchkin que está incrustado en el sitio web.

* Para Munchkin, simplemente agregue {&quot;anonymizeIP&quot;,true} a la función init.

   >[!NOTE]
   >
   >El uso de este parámetro requiere que Munchkin V2 esté habilitado. Para habilitarlo para su suscripción, póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/community/support_solutions).

* Para la personalización web (RTP), añádalo a javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
