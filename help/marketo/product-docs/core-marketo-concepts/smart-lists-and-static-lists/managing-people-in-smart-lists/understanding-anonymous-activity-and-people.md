---
unique-page-id: 1147322
description: 'Información sobre la actividad anónima y las personas: Documentos de Marketo: Documentación del producto'
title: Explicación de la actividad y las personas anónimas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Información sobre la actividad anónima y las personas {#understanding-anonymous-activity-and-people}

La primera vez que alguien visita una página de aterrizaje de Marketo (o una página de su sitio web que tiene el [Código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea una _actividad anónima_ y utiliza una cookie del explorador para rastrearla. Una vez identificada, se convierte en una persona y el historial asociado con la cookie de su explorador se combina.

**Se crea una actividad** anónima cuando alguien:

* Visita su página de aterrizaje de Marketo por primera vez.
* Visita una página del sitio que tiene [Munchkin tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Hace clic en el vínculo [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) en un correo electrónico de Marketo.

>[!NOTE]
>
>A diferencia de otros vínculos de los correos electrónicos de Marketo, [View as Web Page](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) no se rastrea como un clic de correo electrónico.

Una actividad anónima se fusiona en una persona nueva o existente cuando alguien:

* Hace clic en un enlace [en un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Rellena un [Formulario](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md) de Marketo.
* Utiliza la API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) de Marketo (para desarrolladores) para asociar una persona anónima a un registro conocido.

Un nombre de la base de datos puede estar vinculado a muchas cookies porque la gente suele utilizar distintos dispositivos y navegadores para visitar el sitio.

>[!NOTE]
>
>Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de campo personalizados **no** se transfieren.
