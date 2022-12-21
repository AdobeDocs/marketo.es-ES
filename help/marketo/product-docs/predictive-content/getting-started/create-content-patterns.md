---
unique-page-id: 11385579
description: 'Creación de patrones de contenido: documentos de Marketo: documentación del producto'
title: Crear patrones de contenido
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Crear patrones de contenido {#create-content-patterns}

Cuando establece patrones de contenido, el contenido se descubre automáticamente cuando un visitante web hace clic en la página web del HTML relevante para el patrón de contenido. Se utiliza para agregar páginas HTML (anuncios de blogs, comunicados de prensa, artículos de noticias) como artículos de contenido a la página Todo el contenido. Cuando el descubrimiento automático se basa en patrones de contenido, detecta y rastrea páginas HTML que están relacionadas con el patrón de URL definido cuando un visitante web hace clic o visualiza un vínculo a la página. Esta parte de contenido (la URL, el nombre de página y los metadatos, incluyendo la dirección URL y la descripción de la imagen) se agrega a la página Todo contenido para preparar contenido predictivo. Para detectar automáticamente otro contenido, como PDF y vídeo incrustado, debe [habilitar la detección de contenido](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vaya a **Configuración de contenido**.

   ![](assets/settings-dropdown-hand-2.png)

1. Haga clic en **Patrones de URL**.

   ![](assets/click-url-patterns-hand.png)

1. Haga clic en el **+** para abrir una fila donde puede introducir su información.

   ![](assets/content-settings-create-patterns-hand.png)

1. Añada la extensión URL del dominio donde existe la página web. Seleccione la categoría (por ejemplo, Blog, Artículo, Hoja de datos, Comunicado de prensa).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Los elementos de la lista desplegable de la derecha reflejan las categorías que configuró al [categorías creadas](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Haga clic en **+** para agregar otra ruta.

   ![](assets/url-patterns-add2.png)

1. Añada la extensión y la categoría para la ruta adicional y haga clic en **Guardar**.

   ![](assets/url-patterns-save.png)

## Reglas del patrón de contenido {#content-pattern-rules}

* Puede utilizar un comodín en cualquier lugar de una expresión (ejemplo: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Se recomienda usar /&#42; al final de una expresión para continuar con la detección de patrones (Ejemplo: _domain.com/blog/&#42;_ detecta todas las publicaciones de la carpeta Blog)
* Los patrones de contenido no distinguen entre mayúsculas y minúsculas (ejemplo: _domain.com/Blog/&#42;_ detecta todas las páginas html en _domain.com/Blog_ y _domain.com/blog_)

* Los parámetros de URL no se descubren (esto evita descubrir varios elementos con la misma dirección URL de contenido pero parámetros diferentes)

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
   <td><p>Descubre todo el contenido que coincide con el patrón domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>article/2017/*</td> 
   <td><p>Descubre todo el contenido que coincide con el patrón domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>Descubre cualquier dirección URL que contenga la palabra "hojas de datos:"</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>comunicado de prensa</td> 
   <td><p>Solo se detecta una página del HTML de coincidencia exacta:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Si la expresión URL está vacía, el patrón de URL detecta solo la página principal:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
