---
unique-page-id: 2360181
description: Seguimiento de actividades y personas anónimas - Documentos de Marketo - Documentación del producto
title: Seguimiento de actividades y personas anónimas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Seguimiento de actividades y personas anónimas {#tracking-anonymous-activity-and-people}

La primera vez que alguien visita un Marketo [página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (o una página de su sitio web que tenga la variable [Código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crea un _actividad anónima_ y utiliza una cookie del explorador para rastrearla. Una vez identificado el visitante, se convierte en una persona y el historial asociado con la cookie del explorador se combina en.

1. Se crea una actividad anónima cuando alguien:

   * Visita su Marketo [página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) la primera vez.
   * Visita una página del sitio que tenga [Seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Haga clic en el [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) en un correo electrónico de Marketo.

   >[!NOTE]
   >
   >A diferencia de otros vínculos de los correos electrónicos de Marketo, Ver como página web no se rastrea como un clic de correo electrónico.

   Una actividad anónima se fusiona en una persona nueva o existente cuando alguien:

   * Clics a [vínculo en un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Rellena una Marketo [formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Utiliza Marketo [API de REST](https://developers.marketo.com/rest-api/lead-database/leads/) o [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API (para desarrolladores) para asociar una actividad anónima a un registro conocido.

   Un nombre de la base de datos puede estar vinculado a muchas cookies porque la gente suele utilizar distintos dispositivos y navegadores para visitar el sitio.

   >[!NOTE]
   >
   >Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de campo personalizados **not** transferencia.

   >[!MORELIKETHIS]
   >
   >[Mostrar personas o visitantes anónimos en informes web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
