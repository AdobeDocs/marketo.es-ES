---
unique-page-id: 2360181
description: Seguimiento de actividades y personas anónimas - Documentos de Marketo - Documentación del producto
title: Seguimiento de actividades y personas anónimas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Seguimiento de actividades y personas anónimas {#tracking-anonymous-activity-and-people}

La primera vez que alguien visita un Marketo [página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (o una página de su sitio web que tenga el [Código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crea un _actividad anónima_ y utiliza una cookie del explorador para realizar el seguimiento. Una vez identificado el visitante, se convierte en una persona y el historial asociado con la cookie del explorador se combina con.

1. Se crea una actividad anónima cuando alguien:

   * Visita su Marketo [página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) la primera vez.
   * Visita una página del sitio que tiene [Seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Hace clic en [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) en un correo electrónico de Marketo.

   >[!NOTE]
   >
   >A diferencia de otros vínculos de los correos electrónicos de Marketo, Ver como página web no se rastrea como un clic en un correo electrónico.

   Una actividad anónima se combina con una persona nueva o existente cuando alguien:

   * Clics en una [vínculo en un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Rellena un Marketo [formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Utiliza Marketo [API DE REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) o [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) API (para desarrolladores) para asociar una actividad anónima con un registro conocido.

   Un nombre de la base de datos puede estar vinculado a muchas cookies porque los usuarios suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

   >[!NOTE]
   >
   >Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de los campos personalizados **no** transferencia terminada.

   >[!MORELIKETHIS]
   >
   >[Mostrar personas o visitantes anónimos en los informes web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
