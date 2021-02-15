---
unique-page-id: 2360181
description: Seguimiento de personas y Actividades anónimas - Documentos de marketing - Documentación del producto
title: Seguimiento de personas y Actividades anónimas
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Seguimiento de personas y Actividades anónimas {#tracking-anonymous-activity-and-people}

La primera vez que alguien visita una [página de aterrizaje](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de Marketing (o una página de su sitio Web que tiene el [código de seguimiento de Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crea una *actividad anónima* *y utiliza una cookie de explorador para rastrearla.* Una vez identificado el visitante, se convierte en una persona y se combina el historial asociado con la cookie del explorador.

1. Se crea una actividad anónima cuando alguien:

   * Visita su página de aterrizaje [de Marketing](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) por primera vez.
   * Visita una página del sitio que tiene [seguimiento de Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Hace clic en el vínculo [Vista como página Web](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) en un mensaje de correo electrónico de marketing.

   >[!NOTE]
   >
   >A diferencia de otros vínculos de los correos electrónicos de marketing, la Vista como página web no se rastrea como un clic de correo electrónico.

   Una actividad anónima se combina en una persona nueva o existente cuando alguien:

   * Hace clic en un vínculo [en un mensaje de correo electrónico de Marketing](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Rellena un formulario [de Marketing](https://docs.marketo.com/display/docs/forms).
   * Utiliza la API [REST](https://developers.marketo.com/rest-api/lead-database/leads/) o [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) de Marketing para asociar una actividad anónima con un registro conocido.

   Un nombre de la base de datos puede estar vinculado a muchas cookies porque las personas suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

   >[!NOTE]
   >
   >Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de campo personalizados **no** se transfieren.

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Mostrar personas o Visitantes anónimos en informes web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Buceo profundo**
   >
   >
   >Obtenga más información sobre [Sistema de informes básico](https://docs.marketo.com/display/docs/basic+reporting).

