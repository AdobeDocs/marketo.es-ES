---
unique-page-id: 4720108
description: Habilitar la barra de recomendaciones de contenido - Documentos de marketing - Documentación del producto
title: Habilitar la barra de recomendaciones de contenido
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---


# Habilitar la barra de recomendaciones de contenido {#enable-the-content-recommendation-bar}

El motor de recomendación de contenido utiliza análisis predictivos y algoritmos de aprendizaje automático para ofrecer contenido relevante a cada visitante web. El motor de recomendaciones predice qué contenido funcionaría mejor por visitante. El contenido del motor se monitorea y controla en la página de Recommendations, lo que le ayuda a optimizar el ROI del contenido.

>[!PREREQUISITES]
>
>Antes de habilitar el contenido predictivo, debe:
>
>* [Preparación del contenido predictivo](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [Aprobar un título para contenido predictivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Habilitar y personalizar la barra de recomendaciones de contenido {#enable-and-customize-the-content-recommendation-bar}

1. Vaya a Configuración **de contenido**.

   ![](assets/settings-dropdown-hand.png)

1. Haga clic en **Barra**.

   ![](assets/content-settings-bar-hand.png)

1. Para habilitar la barra de recomendaciones para una dirección URL, haga clic en **Activado** y, a continuación, en **Guardar**.

   ![](assets/bar-enable.png)

1. Para personalizar una dirección URL, seleccione colores, estilo, formato, flechas para la barra de recomendaciones y páginas para incluir o excluir la barra. Personalice para adaptarse a la marca del sitio web. Haga clic en **Guardar**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Incluir / Excluir dirección URL de visualización**
   >
   >    * La dirección URL de visualización debe ser la ruta del dominio
   >    * No incluya http:// o https://
   >    * Utilice * para comodines
   * Utilizar un punto y coma como separador
   * Ejemplo: /contact_us*; *action=logout*
   * Este campo distingue entre mayúsculas y minúsculas


## Consideraciones sobre la barra de recomendaciones {#recommendation-bar-considerations}

* Para que el motor de Recomendaciones funcione, necesita al menos una parte de contenido para la barra de recomendaciones definida como **Activado** en la página de Recommendations. Si no hay contenido habilitado y la barra está configurada en **Activado**, el efecto de flecha se mostrará en la parte inferior derecha de la página web, pero no aparecerá ningún contenido recomendado.

* Cuanto mayor sea el contenido que se ejecuta en el motor de recomendaciones, mejor será para que el algoritmo pruebe y conozca qué contenido funciona mejor. Se recomienda empezar con entre 10 y 20 fragmentos de contenido en ejecución y activos, y seguir agregando nuevos.
* La parte de contenido que habilite para la recomendación debe incluir la etiqueta RTP Javascript. Esto ayuda al algoritmo a rastrear y optimizar el contenido recomendado.

>[!NOTE]
**Artículos relacionados**
* [Habilitar contenido predictivo para medios enriquecidos por Web](enable-predictive-content-for-web-rich-media.md)

