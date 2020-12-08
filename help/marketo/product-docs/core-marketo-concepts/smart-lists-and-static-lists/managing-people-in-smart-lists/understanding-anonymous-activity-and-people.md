---
unique-page-id: 1147322
description: Explicación de la Actividad y las personas anónimas - Documentos de marketing - Documentación del producto
title: Información sobre la Actividad y las personas anónimas
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---


# Información sobre la Actividad y las personas anónimas {#understanding-anonymous-activity-and-people}

La primera vez que alguien visita una página de Marketing [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (o una página de su sitio web que tiene el código [de seguimiento de](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), Marketo crea una **actividad* anónima y utiliza una cookie de explorador para rastrearla. Una vez identificado, se convierte en una persona y se combina el historial asociado con la cookie del explorador.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

**Se crea una actividad anónima** cuando alguien:

* Visita la página de aterrizaje de Marketing por primera vez.

* Visita una página del sitio que tiene el seguimiento [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).

* Hace clic en el vínculo [Vista como página](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web en un mensaje de correo electrónico de marketing.

>[!NOTE]
>
>A diferencia de otros vínculos de los correos electrónicos de marketing, la [Vista como página](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) web no se rastrea como un clic de correo electrónico.

Una actividad anónima se combina en una persona nueva o existente cuando alguien:

* Hace clic en un [vínculo de un mensaje de correo electrónico](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)de marketing.
* Rellena un [formulario](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)de marketing.
* Utiliza la API [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) o [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) de Marketing para asociar una persona anónima con un registro conocido.

Un nombre de la base de datos puede estar vinculado a muchas cookies porque las personas suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

>[!NOTE]
>
>Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de campo personalizados **no se transfieren** .

