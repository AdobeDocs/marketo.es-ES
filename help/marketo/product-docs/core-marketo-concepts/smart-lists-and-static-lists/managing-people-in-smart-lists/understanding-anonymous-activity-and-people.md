---
unique-page-id: 1147322
description: Explicación de la actividad anónima y las personas - Documentos de Marketo - Documentación del producto
title: Explicación de la actividad anónima y las personas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Explicación de la actividad anónima y las personas {#understanding-anonymous-activity-and-people}

La primera vez que alguien visite una página de aterrizaje de Marketo (o una página de su sitio web que tenga el [Código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea un _actividad anónima_ y utiliza una cookie del explorador para realizar el seguimiento. Una vez identificada, se convierte en una persona y el historial asociado con la cookie de su explorador se combina con.

>[!IMPORTANT]
>
>Activación de la función beta **Actividad de reproducción anónima de Munchkin V2 conocida** garantiza que las campañas activadas por la promoción anónima de posibles clientes siempre se reproduzcan después de que el posible cliente anónimo se fusione correctamente en el registro conocido. Como resultado, los campos personalizados modificados por los pasos Cambiar valor de datos en cualquier campaña reproducida se conservarán en el registro conocido.

**Un anónimo** La actividad se crea cuando alguien:

* Visita la página de aterrizaje de Marketo la primera vez.
* Visita una página del sitio que tiene [Seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Hace clic en [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) en un correo electrónico de Marketo.

>[!NOTE]
>
>A diferencia de otros vínculos en correos electrónicos de Marketo, [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) no se rastrea como un clic en el correo electrónico.

Una actividad anónima se combina con una persona nueva o existente cuando alguien:

* Clics en una [vínculo en un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Rellena un Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utiliza Marketo [JABÓN](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API (para desarrolladores) para asociar una persona anónima con un registro conocido.

Un nombre de la base de datos puede estar vinculado a muchas cookies porque los usuarios suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

>[!NOTE]
>
>Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de los campos personalizados **no** transferencia terminada.
