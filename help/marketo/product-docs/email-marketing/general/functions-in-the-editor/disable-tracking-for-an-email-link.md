---
unique-page-id: 1900579
description: 'Desactivación del seguimiento de un vínculo de correo electrónico: documentos de Marketo: documentación del producto'
title: Desactivación del seguimiento de un vínculo de correo electrónico
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Desactivación del seguimiento de un vínculo de correo electrónico {#disable-tracking-for-an-email-link}

A veces no se desea habilitar la variable **URL de seguimiento de Marketo** en un vínculo de un correo electrónico. Esto resulta útil cuando la página de destino no admite parámetros de URL y puede provocar que se rompan los vínculos.

1. Seleccione el correo electrónico y haga clic en **Editar borrador**.

   ![](assets/one-7.png)

1. Haga doble clic en la sección editable que contiene el vínculo.

   ![](assets/two-6.png)

1. Haga clic en el vínculo en cuestión y, a continuación, haga clic en el botón **Insertar/Editar vínculo** botón.

   ![](assets/three-6.png)

1. En la ventana emergente Editar vínculo, desmarque la casilla **Seguimiento de vínculos** casilla de verificación.

   ![](assets/four-4.png)

1. Verá el **Cuadro Incluir mkt_tok** desaparece. Haga clic en **Aplicar**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Desmarcando solo **Incluir mkt_tok** seguirá permitiendo que se rastree el vínculo, pero después de la redirección, la dirección URL de destino no incluirá el parámetro de cadena de consulta mkt_tok . Marketo Landing Pages and Munchkin utiliza este parámetro para garantizar un seguimiento adecuado de las actividades de las personas (como cuando una persona cancela la suscripción de un correo electrónico). Debería evitar usar esta función a menos que esté viendo un comportamiento extraño en su sitio web debido a que el parámetro está presente.

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Desea desactivar el rastreo de clics de un vínculo en un correo electrónico **plantilla**? Utilice este formato:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Si necesita ayuda para implementar esto, consulte con su desarrollador web.

¡Muy bien! Ahora ha desactivado el seguimiento de un vínculo.
