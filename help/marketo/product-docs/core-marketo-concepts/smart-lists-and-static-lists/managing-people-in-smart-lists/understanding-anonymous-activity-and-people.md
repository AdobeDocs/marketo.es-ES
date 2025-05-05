---
unique-page-id: 1147322
description: Explicación de la actividad anónima y las personas - Documentos de Marketo - Documentación del producto
title: Explicación de la actividad anónima y las personas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Explicación de la actividad anónima y las personas {#understanding-anonymous-activity-and-people}

La primera vez que alguien visite una página de aterrizaje de Marketo (o una página de su sitio web que tenga el [Código de seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), Marketo creará una *actividad anónima* y usará una cookie de explorador para rastrearla. Una vez identificada, se convierte en una persona y el historial asociado con la cookie de su explorador se combina con.

>[!IMPORTANT]
>
>Al habilitar la función de Beta **Munchkin V2 Anonymous Replay Activity on Known**, se garantiza que las campañas activadas por la promoción anónima de posibles clientes se reproducirán siempre después de que el posible cliente anónimo se combine correctamente en el registro conocido. Como resultado, los campos personalizados modificados por los pasos Cambiar valor de datos en cualquier campaña reproducida se conservarán en el registro conocido.

**Se crea una actividad Anonymous** cuando alguien:

* Visita la página de aterrizaje de Marketo la primera vez.
* Visita una página de tu sitio que tiene [seguimiento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Hace clic en el vínculo [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} de un correo electrónico de Marketo.

>[!NOTE]
>
>A diferencia de otros vínculos en correos electrónicos de Marketo, [Ver como página web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} no se rastrea como un clic en un correo electrónico.

Una actividad anónima se combina con una persona nueva o existente cuando alguien:

* Hace clic en un vínculo [de un correo electrónico de Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Rellena un [formulario](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} de Marketo.
* Utiliza la API [&#128279;](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} de Marketo SOAP (para desarrolladores) para asociar a una persona anónima con un registro conocido.

Un nombre de la base de datos puede estar vinculado a muchas cookies porque los usuarios suelen utilizar distintos dispositivos y exploradores para visitar el sitio.

>[!NOTE]
>
>Cuando los registros anónimos se combinan en un registro de persona nuevo o existente, los valores de los campos personalizados *no* se transferirán.
