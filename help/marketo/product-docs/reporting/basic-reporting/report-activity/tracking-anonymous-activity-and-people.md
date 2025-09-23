---
unique-page-id: 2360181
description: Seguimiento de actividades y personas anónimas - Documentos de Marketo - Documentación del producto
title: Seguimiento de actividades anónimas y personas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# Seguimiento de actividades anónimas y personas {#tracking-anonymous-activity-and-people}

La primera vez que alguien visite una [página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de Marketo (o una página de su sitio web que tenga el [código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo creará una _actividad anónima_ y usará una cookie de explorador para realizar el seguimiento. Una vez identificado el visitante, se convierte en una persona y el historial asociado con la cookie del explorador se combina con.

1. Se crea una actividad anónima cuando alguien:

   * Visita tu [página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de Marketo la primera vez.
   * Visita una página de tu sitio que tiene [seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Hace clic en el vínculo [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) de un correo electrónico de Marketo.

   >[!NOTE]
   >
   >A diferencia de otros vínculos de los correos electrónicos de Marketo, Ver como página web no se rastrea como un clic en un correo electrónico.

   Una actividad anónima se combina con una persona nueva o existente cuando alguien:

   * Hace clic en un vínculo [de un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Rellena un [formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) de Marketo.
   * Utiliza la API [REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) o [Munchkin](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) de Marketo (para desarrolladores) para asociar una actividad anónima con un registro conocido.

   Un nombre de la base de datos puede estar vinculado a muchas cookies porque los usuarios suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

   >[!NOTE]
   >
   >Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de los campos personalizados **no** se transferirán.

   >[!MORELIKETHIS]
   >
   >[Mostrar personas o visitantes anónimos en los informes web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
