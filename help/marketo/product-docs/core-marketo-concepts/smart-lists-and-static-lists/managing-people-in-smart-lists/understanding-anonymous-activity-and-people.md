---
unique-page-id: 1147322
description: 'Información sobre la actividad anónima y las personas: Documentos de Marketo: Documentación del producto'
title: Explicación de la actividad y las personas anónimas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Explicación de la actividad y las personas anónimas {#understanding-anonymous-activity-and-people}

La primera vez que alguien visita una página de aterrizaje de Marketo (o una página del sitio web que tenga la variable [Código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea un _actividad anónima_ y utiliza una cookie del explorador para rastrearla. Una vez identificada, se convierte en una persona y el historial asociado con la cookie de su explorador se combina.

>[!IMPORTANT]
>
>Activación de la función beta **Actividad de reproducción anónima de Munchkin V2 en conocidos** garantiza que las campañas activadas por la promoción de posibles clientes anónimas siempre se reproduzcan después de que el posible cliente anónimo se fusione correctamente en el registro conocido. Como resultado, los campos personalizados cambiados por los pasos Cambiar valor de datos en cualquier campaña reproducida se mantendrán en el registro conocido.

**Anonymous** actividad se crea cuando alguien:

* Visita su página de aterrizaje de Marketo por primera vez.
* Visita una página del sitio que tenga [Seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Haga clic en el [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) en un correo electrónico de Marketo.

>[!NOTE]
>
>A diferencia de otros vínculos de los correos electrónicos de Marketo, [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) no se rastrea como un clic de correo electrónico.

Una actividad anónima se fusiona en una persona nueva o existente cuando alguien:

* Clics a [vínculo en un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Rellena una Marketo [Formulario](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utiliza Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API (para desarrolladores) para asociar una persona anónima a un registro conocido.

Un nombre de la base de datos puede estar vinculado a muchas cookies porque la gente suele utilizar distintos dispositivos y navegadores para visitar el sitio.

>[!NOTE]
>
>Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de campo personalizados **not** transferencia.
