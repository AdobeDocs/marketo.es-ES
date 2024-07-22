---
unique-page-id: 1900579
description: Deshabilitar el seguimiento de un vínculo de correo electrónico - Documentos de Marketo - Documentación del producto
title: Deshabilitar el seguimiento de un vínculo de correo electrónico
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Deshabilitar el seguimiento de un vínculo de correo electrónico {#disable-tracking-for-an-email-link}

A veces no se desea habilitar la **URL de seguimiento de Marketo** en un vínculo de un mensaje de correo electrónico. Esto resulta útil cuando la página de destino no admite parámetros de URL y puede provocar que se rompa un vínculo.

1. Seleccione su correo electrónico y haga clic en **Editar borrador**.

   ![](assets/one-7.png)

1. Haga doble clic en la sección editable que contiene el vínculo.

   ![](assets/two-6.png)

1. Haga clic en el vínculo en cuestión y, a continuación, en el botón **Insertar/Editar vínculo**.

   ![](assets/three-6.png)

1. En la ventana emergente Editar vínculo, desmarque la casilla de verificación **Rastrear vínculo**.

   ![](assets/four-4.png)

1. Observará que la **caja Include mkt_tok** desaparece. Haga clic en **Aplicar**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Si desmarca solo **Incluir mkt_tok** se seguirá permitiendo el seguimiento del vínculo, pero después del redireccionamiento, la dirección URL de destino no incluirá el parámetro de cadena de consulta mkt_tok. Este parámetro lo utilizan las páginas de aterrizaje de Marketo y Munchkin para garantizar un seguimiento adecuado de las actividades de la persona (como cuando una persona cancela la suscripción de un correo electrónico). Debe evitar utilizar esta función a menos que vea un comportamiento extraño en el sitio web debido a que el parámetro está presente.

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >¿Desea deshabilitar el rastreo de clics para un vínculo en un mensaje de correo electrónico **template**? Utilice este formato:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Si necesita ayuda para implementar esto, consúltelo con su desarrollador web.

¡Bonito! Ahora ha desactivado el seguimiento de un vínculo.
