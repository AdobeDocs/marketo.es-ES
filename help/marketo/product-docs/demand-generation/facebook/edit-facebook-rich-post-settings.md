---
unique-page-id: 2950555
description: Editar la configuración de anuncios enriquecidos de Facebook - Documentos de marketing - Documentación del producto
title: Editar configuración de anuncios enriquecidos de Facebook
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Editar configuración de anuncios enriquecidos de Facebook {#edit-facebook-rich-post-settings}

Personalice las publicaciones cuando las personas [lo compartan](http://docs.marketo.com/display/docs/social) en Facebook.

>[!NOTE]
>
>**Disponibilidad**
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

Las aplicaciones [](http://docs.marketo.com/display/docs/social) sociales de marketing permiten que tus leads compartan tus páginas de aterrizaje con sus conexiones en redes sociales como Facebook, Twitter, etc. Las etiquetas OpenGraph de Facebook (OG) permiten especificar qué información de la página de aterrizaje se incluye en las publicaciones de Facebook.

## Seleccionar opciones de anuncio enriquecido {#select-rich-post-options}

Puede especificar los tipos de información de página que se utilizarán en las publicaciones enriquecidas de Facebook generadas por los compartidos de su página de aterrizaje.

1. Seleccione Mensaje **de** Facebook en el editor para el vídeo o botón social de **YouTube** .

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Seleccione una de las siguientes opciones para el mensaje de Facebook.

   * Añadir contenido estático: Seleccione esta opción para introducir manualmente el título, el rótulo y la descripción.

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Añadir contenido dinámico: La aplicación social puede utilizar las etiquetas `<TITLE>`, `<CAPTION>`y `<DESCRIPTION>` de su página de aterrizaje para completar la publicación enriquecida.

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >Éstos ya deberían existir en el origen de la página, pero para obtener más control, puede [agregar etiquetas OG de Facebook específicas a la página de aterrizaje](edit-facebook-rich-post-settings.md).

   * No agregar contenido enriquecido: Limita las publicaciones de Facebook de su página de aterrizaje solo al mensaje y vínculo principales.

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## Añadir etiquetas OG de Facebook en una Página de aterrizaje {#add-facebook-og-tags-to-a-landing-page}

Para controlar los elementos de página que se incluirán en los elementos compartidos de Facebook desde la página de aterrizaje, puede agregar etiquetas OG (Open Graph) de Facebook para título, rótulo y descripción a la página de aterrizaje.

1. Abra la página de aterrizaje que contenga el vídeo **o el botón social de** YouTube.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   El Diseñador de **Páginas de aterrizaje** se abre en una ventana nueva.

1. Seleccione Acciones **de** Página de aterrizaje > **Editar etiquetas** de meta de página**.**

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Añada el HTML que define og:title, og:caption y og:description. Copie y pegue estas líneas y sustituya el texto del marcador de posición:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenga cuidado de utilizar la sintaxis HTML adecuada al agregar las etiquetas OG.
