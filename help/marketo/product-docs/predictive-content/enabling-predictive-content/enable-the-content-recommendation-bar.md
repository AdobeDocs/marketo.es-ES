---
unique-page-id: 4720108
description: 'Habilitar la barra de recomendaciones de contenido: documentos de Marketo: documentación del producto'
title: Habilitar la barra de recomendaciones de contenido
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Habilitar la barra de recomendaciones de contenido {#enable-the-content-recommendation-bar}

El motor de recomendación de contenido utiliza análisis predictivos y algoritmos de aprendizaje automático para ofrecer contenido relevante a cada visitante web. El motor de recomendaciones predice qué contenido tendría mejor rendimiento por visitante. El contenido del motor se controla y supervisa en la página de Recommendations, lo que le ayuda a optimizar el retorno de la inversión del contenido.

>[!PREREQUISITES]
>
>Antes de activar el contenido predictivo, debe:
>
>* **Prepare su contenido predictivo**
   >
   >   * [Editar contenido predictivo para correos electrónicos](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) o
   >   * [Editar contenido predictivo para medios enriquecidos](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) o
   >   * [Editar contenido predictivo para la barra de recomendaciones](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Aprobar un título para contenido predictivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Habilitar y personalizar la barra de recomendaciones de contenido {#enable-and-customize-the-content-recommendation-bar}

1. Vaya a **Configuración de contenido**.

   ![](assets/settings-dropdown-hand.png)

1. Haga clic en **Barra**.

   ![](assets/content-settings-bar-hand.png)

1. Para habilitar la barra de recomendaciones para una dirección URL, simplemente haga clic en **Activado** y luego **Guardar**.

   ![](assets/bar-enable.png)

1. Para personalizar una dirección URL, seleccione colores, estilo, formato, flechas para la barra de recomendaciones y páginas para incluir o excluir la barra. Personalizar para adaptarse a la marca de su sitio web. Haga clic en **Guardar**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Incluir / Excluir dirección URL de visualización**
   >
   >* La dirección URL de visualización debe ser la ruta del dominio
   >* No incluya https:// o https://
   >* Uso &#42; para comodines
   >* Utilizar un punto y coma como separador
   >* Ejemplo: /contact_us&#42;; &#42;action=logout&#42;
   >* Este campo distingue entre mayúsculas y minúsculas


## Consideraciones sobre la barra de recomendaciones {#recommendation-bar-considerations}

* Necesita al menos un fragmento de contenido para la barra de recomendaciones configurada en **Activado** en la página Recommendations para que funcione el motor de Recomendaciones . Si no hay contenido habilitado y la barra está configurada en **Activado**, el efecto Flecha se mostrará en la parte inferior derecha de la página web, pero no aparecerá ningún contenido recomendado.

* Cuanto más contenido se ejecute en el motor de recomendaciones, mejor será para que el algoritmo pruebe y aprenda qué contenido funciona mejor. Se recomienda empezar con entre 10 y 20 fragmentos de contenido en ejecución y activos, así como seguir añadiendo nuevos.
* La parte de contenido que habilite para la recomendación debe incluir la etiqueta Javascript de RTP. Esto ayuda al algoritmo a rastrear y optimizar el contenido recomendado.

>[!MORELIKETHIS]
>
>[Habilitar contenido predictivo para medios enriquecidos en la Web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
