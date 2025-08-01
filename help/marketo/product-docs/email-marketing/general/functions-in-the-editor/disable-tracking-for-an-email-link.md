---
unique-page-id: 1900579
description: Deshabilitar el seguimiento de un vínculo de correo electrónico - Documentos de Marketo - Documentación del producto
title: Deshabilitar el seguimiento de un vínculo de correo electrónico
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Deshabilitar el seguimiento de un vínculo de correo electrónico {#disable-tracking-for-an-email-link}

A veces no se desea habilitar la **URL de seguimiento de Marketo** en un vínculo de un mensaje de correo electrónico. Esto resulta útil cuando la página de destino no admite parámetros de URL y puede provocar que se rompa un vínculo.

Además, si un correo electrónico se envió hace más de 365 días **y** nadie ha hecho clic en ninguno de sus vínculos en los últimos 180 días, Marketo Engage elimina la ruta a la dirección URL de nuestra base de datos, lo que provocará que se rompa el vínculo. Por lo tanto, si necesita que el vínculo sea permanente, debe deshabilitar el seguimiento.

1. Seleccione su correo electrónico y haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/one-7.png)

1. Haga doble clic en la sección editable que contiene el vínculo.

   ![](assets/two-6.png)

1. Haga clic en el vínculo en cuestión y, a continuación, en el botón **Insertar/Editar vínculo**.

   ![](assets/three-6.png)

1. En la ventana emergente Editar vínculo, desmarque la casilla de verificación **[!UICONTROL Rastrear vínculo]**.

   ![](assets/four-4.png)

1. Observará que la casilla **[!UICONTROL Incluir mkt_tok]** desaparece. Haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Si desmarca solo **Incluir mkt_tok** se seguirá permitiendo el seguimiento del vínculo, pero después del redireccionamiento, la dirección URL de destino no incluirá el parámetro de cadena de consulta mkt_tok. Este parámetro lo utilizan las páginas de aterrizaje de Marketo y Munchkin para garantizar un seguimiento adecuado de las actividades de la persona (como cuando una persona cancela la suscripción de un correo electrónico). Debe evitar utilizar esta función a menos que vea un comportamiento extraño en el sitio web debido a que el parámetro está presente.

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >Si desea deshabilitar el rastreo de clics para un vínculo en una plantilla de correo electrónico o la [versión de texto](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"} de un correo electrónico, agregue `mktNoTrack` al *principio* de la cadena, no al final, como en este ejemplo: `<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`. De lo contrario, podría hacer que el vínculo desapareciera. Si necesita ayuda para implementar el código anterior, consúltelo con su desarrollador web.
