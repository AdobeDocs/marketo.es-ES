---
unique-page-id: 2360181
description: Obtenga información acerca del seguimiento de actividades y personas anónimas en Marketo Engage, incluido el seguimiento de actividades y eventos anónimos. Utilice esta guía para completar el siguiente paso.
title: Seguimiento de actividades anónimas y personas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 8%

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
