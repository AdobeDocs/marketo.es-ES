---
unique-page-id: 2360181
description: Seguimiento de personas y Actividades anónimas - Documentos de marketing - Documentación del producto
title: Seguimiento de personas y Actividades anónimas
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# Seguimiento de personas y Actividades anónimas {#tracking-anonymous-activity-and-people}

La primera vez que alguien visita una [página de aterrizaje](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de marketing (o una página de su sitio web que tiene el código [de seguimiento](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), Marketo crea una *actividad* *anónima* y utiliza una cookie de explorador para rastrearla. Una vez identificado el visitante, se convierte en una persona y se combina el historial asociado con la cookie del explorador.

1. Se crea una actividad anónima cuando alguien:

   * Visita su [página de aterrizaje](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de Marketing por primera vez.
   * Visita una página del sitio que tiene el seguimiento [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Hace clic en el vínculo [Vista como página](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web en un mensaje de correo electrónico de marketing.

   >[!NOTE]
   >
   >A diferencia de otros vínculos de los correos electrónicos de marketing, la Vista como página web no se rastrea como un clic de correo electrónico.

   Una actividad anónima se combina en una persona nueva o existente cuando alguien:

   * Hace clic en un [vínculo de un mensaje de correo electrónico](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)de marketing.
   * Rellena un [formulario](http://docs.marketo.com/display/docs/forms)de marketing.
   * Utiliza la API [](http://developers.marketo.com/rest-api/lead-database/leads/) REST de Marketo o la API [Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) (para desarrolladores) para asociar una actividad anónima con un registro conocido.

   Un nombre de la base de datos puede estar vinculado a muchas cookies porque las personas suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

   >[!NOTE]
   >
   >Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de campo personalizados **no se transfieren** .

   >[!NOTE]
   >
   >**Artículos relacionados**
   >
   >    
   >    
   >    * [Mostrar personas o Visitantes anónimos en informes web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Buceo profundo**
   >
   >
   >Obtenga más información sobre Sistema de informes [](http://docs.marketo.com/display/docs/basic+reporting)básico.

