---
unique-page-id: 2950555
description: Editar configuración de publicaciones enriquecidas de Facebook - Documentos de Marketo - Documentación del producto
title: Editar configuración de publicaciones enriquecidas de Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Editar configuración de publicación enriquecida de [!DNL Facebook] {#edit-facebook-rich-post-settings}

Personalizar publicaciones cuando las personas lo compartan en [!DNL Facebook].

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

Las _aplicaciones sociales_ de Marketo permiten que tus clientes potenciales compartan tus páginas de aterrizaje con sus conexiones en redes sociales como Facebook, Twitter, etc. Las etiquetas OpenGraph de Facebook (etiquetas OG) le permiten especificar qué información de la página de aterrizaje se incluye en las publicaciones de Facebook.

## Seleccionar opciones de publicación enriquecida {#select-rich-post-options}

Puede especificar los tipos de información de página que se usarán en las [!DNL Facebook] publicaciones enriquecidas generadas por los recursos compartidos desde la página de aterrizaje.

1. Seleccione **[!UICONTROL Mensaje de Facebook]** en el editor de su vídeo o botón social **[!DNL YouTube*]*.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Seleccione entre las siguientes opciones para su mensaje [!DNL Facebook].

   * Añadir contenido estático: seleccione esta opción para introducir el título, el pie de ilustración y la descripción manualmente.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Agregar contenido dinámico: su aplicación social puede utilizar las etiquetas `<TITLE>`, `<CAPTION>` y `<DESCRIPTION>` de su página de aterrizaje para rellenar la publicación enriquecida.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Deberían existir en el origen de la página, pero para tener más control, puede agregar etiquetas OG específicas de [!DNL Facebook] a la página de aterrizaje.

   * No agregar contenido enriquecido: Limita las [!DNL Facebook] publicaciones de la página de aterrizaje únicamente al mensaje principal y al vínculo.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Agregar etiquetas OG [!DNL Facebook] a una página de aterrizaje {#add-facebook-og-tags-to-a-landing-page}

Para controlar los elementos de página que se incluirán en los recursos compartidos de [!DNL Facebook] desde la página de aterrizaje, puede agregar etiquetas OG (Abrir gráfico) de [!DNL Facebook] para título, rótulo y descripción a la página de aterrizaje.

1. Abra la página de aterrizaje que contiene su **[!DNL YouTube]vídeo** o botón social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   La **[!UICONTROL página de aterrizaje Designer]** se abre en una nueva ventana.

1. Seleccione **[!UICONTROL Acciones de página de aterrizaje]** > **[!UICONTROL Editar metaetiquetas de página]**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Agregue el HTML que define og:title, og:caption y og:description. Copie y pegue estas líneas y reemplace el texto del marcador de posición:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenga cuidado de utilizar la sintaxis de HTML adecuada al añadir las etiquetas OG.
