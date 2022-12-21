---
unique-page-id: 2950555
description: 'Editar la configuración de publicación enriquecida de Facebook: Documentos de Marketo: Documentación del producto'
title: Editar la configuración de publicación enriquecida de Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Editar la configuración de publicación enriquecida de Facebook {#edit-facebook-rich-post-settings}

Personalice las publicaciones cuando las personas lo compartan en Facebook.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más información.

Marketo [aplicaciones sociales](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) permita que los posibles clientes compartan las páginas de aterrizaje con sus conexiones en redes sociales como Facebook, Twitter, etc. Las etiquetas de facebook OpenGraph (etiquetas OG) permiten especificar qué información de la página de aterrizaje se incluye en las publicaciones de Facebook.

## Seleccionar opciones de publicación enriquecida {#select-rich-post-options}

Puede especificar los tipos de información de página que se usarán en los anuncios enriquecidos de Facebook generados por compartidos desde la página de aterrizaje.

1. Select **Mensaje de facebook** en el editor de **YouTube** botón de vídeo o social .

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Seleccione entre las siguientes opciones para el mensaje de Facebook.

   * Añadir contenido estático: Seleccione esta opción para introducir manualmente el título, el rótulo y la descripción.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Añadir contenido dinámico: La aplicación social puede usar el informe de `<TITLE>`, `<CAPTION>`y `<DESCRIPTION>` para rellenar la publicación enriquecida.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Ya deberían existir en el origen de la página, pero para obtener más control, puede añadir etiquetas OG de Facebook específicas a la página de aterrizaje.

   * No añada contenido enriquecido: Limita las publicaciones de Facebook de su página de aterrizaje a solo el mensaje y vínculo principales.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Adición de etiquetas OG de Facebook a una página de aterrizaje {#add-facebook-og-tags-to-a-landing-page}

Para controlar los elementos de página que se incluirán en los elementos compartidos de Facebook desde la página de aterrizaje, puede agregar etiquetas OG (Open Graph) de Facebook para título, rótulo y descripción a la página de aterrizaje.

1. Abra la página de aterrizaje que contenga su **Vídeo de YouTube** o social .

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   La variable **Diseñador de páginas de aterrizaje** se abre en una nueva ventana.

1. Select **Acciones de página de aterrizaje** > **Editar etiquetas de metadatos de página**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Añada el HTML que define og:title, og:caption y og:description. Copie y pegue estas líneas y reemplace el texto del marcador de posición:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenga cuidado de usar la sintaxis de HTML adecuada al agregar las etiquetas OG.
