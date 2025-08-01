---
unique-page-id: 11385579
description: 'Creación de patrones de contenido: documentos de Marketo, documentación del producto'
title: Crear patrones de contenido
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Crear patrones de contenido {#create-content-patterns}

Cuando se establecen patrones de contenido, este se detecta automáticamente cuando un visitante web hace clic en la página web de HTML correspondiente al patrón de contenido. Se utiliza para añadir páginas de HTML (publicaciones de blog, comunicados de prensa, artículos de noticias) como piezas de contenido a la página Todo el contenido. Cuando la detección automática se basa en patrones de contenido, detecta y rastrea páginas de HTML relacionadas con el patrón de URL definido cuando un visitante web ve o hace clic en un vínculo a la página. Este fragmento de contenido (la URL, el nombre de página y los metadatos, incluida la URL y la descripción de la imagen) se añade a la página Todo el contenido para preparar contenido predictivo. Para descubrir automáticamente otro contenido, como PDF y vídeo incrustado, debe [habilitar la detección de contenido](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vaya a **[!UICONTROL Configuración de contenido]**.

   ![](assets/settings-dropdown-hand-2.png)

1. Haga clic en **[!UICONTROL Patrones de URL]**.

   ![](assets/click-url-patterns-hand.png)

1. Haga clic en **+** para abrir una fila donde pueda introducir la información.

   ![](assets/content-settings-create-patterns-hand.png)

1. Añada la extensión URL del dominio donde existe la página web. Seleccione la categoría (por ejemplo, [!UICONTROL Blog], [!UICONTROL Artículo], [!UICONTROL Hoja de datos], [!UICONTROL Comunicado de prensa]).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Los elementos de la lista desplegable de la derecha reflejan las categorías que configuró al [crear categorías](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Haga clic en **+** para agregar otra ruta.

   ![](assets/url-patterns-add2.png)

1. Agregue la extensión y la categoría para la ruta adicional y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/url-patterns-save.png)

## Reglas de patrón de contenido {#content-pattern-rules}

* Puede usar un comodín en cualquier lugar de una expresión (por ejemplo: _dominio.com/&#42;_, _dominio.com/&#42;blog&#42;_)

* Se recomienda utilizar /&#42; al final de una expresión para continuar con la detección de patrones (Ejemplo: _domain.com/blog/&#42;_ detecta todas las publicaciones en la carpeta Blog)
* Los patrones de contenido no distinguen entre mayúsculas y minúsculas (Ejemplo: _domain.com/Blog/&#42;_ detecta todas las páginas html de _domain.com/Blog_ y _domain.com/blog_)

* No se detectan los parámetros de URL (esto evita descubrir varios elementos con la misma URL de contenido, pero con parámetros diferentes)

## Ejemplos {#examples}

Para _domain.com_:

<table>
 <tbody>
  <tr>
   <th>Patrón de URL</th>
   <th>Resultado</th>
  </tr>
  <tr>
   <td>blog/*</td>
   <td><p>Detecta todo el contenido que coincide con el patrón domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td>
  </tr>
  <tr>
   <td>article/2017/*</td>
   <td><p>Detecta todo el contenido que coincide con el patrón domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td>
  </tr>
  <tr>
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td>
   <td><p>Detecta cualquier dirección URL que contenga la palabra "hojas de datos":</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td>
  </tr>
  <tr>
   <td>comunicado de prensa</td>
   <td><p>Solo se detecta una página de HTML que coincida exactamente:</p><p>domain.com/press-release</p></td>
  </tr>
  <tr>
   <td colspan="1"> </td>
   <td colspan="1"><p>Si la expresión URL está vacía, el patrón URL solo detecta la página principal:</p><p>domain.com</p></td>
  </tr>
 </tbody>
</table>
