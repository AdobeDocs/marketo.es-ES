---
unique-page-id: 1900579
description: Deshabilitar el seguimiento de un vínculo de correo electrónico - Documentos de marketing - Documentación del producto
title: Deshabilitar el seguimiento de un vínculo de correo electrónico
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Deshabilitar el seguimiento de un vínculo de correo electrónico {#disable-tracking-for-an-email-link}

A veces no desea habilitar la **URL de seguimiento de marketing** en un vínculo de un correo electrónico. Esto resulta útil cuando la página de destino no admite parámetros de URL y puede resultar en un vínculo dañado.

1. Seleccione su correo electrónico y haga clic en **Editar borrador**.

   ![](assets/one-7.png)

1. Haga clic con el doble en la sección editable que contiene el vínculo.

   ![](assets/two-6.png)

1. Haga clic en el vínculo en cuestión y, a continuación, haga clic en el botón **Insertar/Editar vínculo**.

   ![](assets/three-6.png)

1. En la ventana emergente Editar vínculo, desmarque la casilla **Vínculo de seguimiento**.

   ![](assets/four-4.png)

1. Observará que la casilla **Incluir mkt_tok** desaparece. Haga clic en **Aplicar**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Al desmarcar **Incluir mkt_tok** aún se podrá rastrear el vínculo, pero después de redireccionar, la dirección URL de destino no incluirá el parámetro de cadena de consulta mkt_tok. Este parámetro lo utilizan las Páginas de aterrizaje de marketing y Munchkin para garantizar un seguimiento adecuado de las actividades de personas (como cuando una persona cancela la suscripción de un correo electrónico). Debe evitar usar esta función a menos que vea un comportamiento extraño en su sitio web debido a la presencia del parámetro.

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >¿Desea deshabilitar el rastreo de clics para un vínculo en una **plantilla** de correo electrónico? Utilice este formato:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Si necesita ayuda para implementar esto, consulte a su desarrollador web.

¡Bonito! Ahora deshabilitó el seguimiento de un vínculo.
