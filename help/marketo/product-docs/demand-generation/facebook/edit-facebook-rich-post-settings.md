---
unique-page-id: 2950555
description: 'Editar configuración de publicación enriquecida de Facebook: documentos de Marketo: documentación del producto'
title: Editar configuración de publicación enriquecida de Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
feature: Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Editar configuración de publicación enriquecida de Facebook {#edit-facebook-rich-post-settings}

Personalice las publicaciones cuando las personas le compartan en Facebook.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

Marketo [aplicaciones sociales](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) permita que los posibles clientes compartan sus páginas de aterrizaje con sus conexiones en redes sociales como Facebook, Twitter, etc. Las etiquetas OpenGraph de facebook (etiquetas OG) le permiten especificar qué información de la página de aterrizaje se incluye en las publicaciones de Facebook.

## Seleccionar opciones de publicación enriquecida {#select-rich-post-options}

Puede especificar los tipos de información de página que se utilizarán en las publicaciones enriquecidas de Facebook generadas por los recursos compartidos desde la página de aterrizaje.

1. Seleccionar **Mensaje de facebook** en el editor de su **YouTube** botón de vídeo o social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Seleccione entre las siguientes opciones para el mensaje de Facebook.

   * Añadir contenido estático: seleccione esta opción para introducir el título, el pie de ilustración y la descripción manualmente.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Añadir contenido dinámico: su aplicación social puede utilizar el de la página de aterrizaje `<TITLE>`, `<CAPTION>`, y `<DESCRIPTION>` para rellenar la publicación enriquecida.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Deberían existir ya en el origen de la página, pero para obtener más control, puede agregar etiquetas de organización de Facebook específicas a la página de aterrizaje.

   * No añadir contenido enriquecido: limita las publicaciones de Facebook de la página de aterrizaje únicamente al mensaje principal y al vínculo.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Añadir etiquetas OG de Facebook a una página de aterrizaje {#add-facebook-og-tags-to-a-landing-page}

Para controlar los elementos de página que se incluirán en los recursos compartidos de Facebook desde la página de aterrizaje, puede agregar etiquetas OG (Abrir gráfico) de Facebook para el título, el pie de ilustración y la descripción de la página de aterrizaje.

1. Abra la página de aterrizaje que contiene su **Vídeo de YouTube** o botón social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   El **Diseñador de páginas de aterrizaje** se abre en una nueva ventana.

1. Seleccionar **Acciones de página de aterrizaje** > **Editar metaetiquetas de página**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Añada el HTML que define og:title, og:caption y og:description. Copie y pegue estas líneas y reemplace el texto del marcador de posición:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenga cuidado de utilizar la sintaxis de HTML adecuada al añadir las etiquetas OG.
