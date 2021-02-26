---
unique-page-id: 4719400
description: Crear una nueva Campaña web en la zona - Documentos de marketing - Documentación del producto
title: Crear una nueva Campaña web en la zona
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---


# Crear una nueva Campaña Web en la zona {#create-a-new-in-zone-web-campaign}

Una campaña Web es una reacción personalizada asociada a un segmento específico y puede ser un [cuadro de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) en su sitio Web, un reemplazo de zona, una [función de utilidad](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) o una alerta por correo electrónico. Una campaña web en la zona sustituye un elemento del sitio web basado en la identificación de la zona por contenido o pancartas gráficas.

## Crear una Campaña Web en la zona {#create-an-in-zone-web-campaign}

1. Vaya a **Campañas Web**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Seleccione **Crear nueva Campaña Web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Seleccione el tipo de campaña **En zona**. Personalice y agregue un **Id. de zona.** Configure la campaña en  **** Pegatina y agregue el elemento creativo al editor. Añada la dirección URL de la página en previsualización y haga clic en **Previsualización** para ver cómo reaccionará la campaña en el sitio.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**¿Qué es un Id. de zona?**
   >
   >Un Id. de zona es donde desea que la campaña web &quot;En la zona&quot; esté ubicada en el sitio. Para encontrar un &quot;Id. de zona&quot;, simplemente ingrese a su sitio web y seleccione el área que desee reemplazar con una campaña web y haga clic con el botón derecho. En Chrome, la opción es &quot;Elemento Inspect&quot;, y en otros exploradores puede variar.
   >
   >Luego, desea encontrar la &quot;identificación&quot; asociada con esta sección del sitio web, que se resalta porque está inspeccionando ese elemento. Por ejemplo, si una vez que hace clic con el botón derecho en Chrome, el texto resaltado indica `<div id="featured-slider">`, entonces &quot;deslizador de funciones&quot; es lo que debe escribir en la sección &quot;id de zona&quot;. Generalmente se utiliza &quot;div id&quot;, pero también se puede usar cualquier ID, como h1 id, p id, etc.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nombre</th> 
   <th colspan="1" rowspan="1">Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> Id. de zona </strong></td> 
   <td colspan="1" rowspan="1"><p>Escriba el nombre del identificador que se encuentra en el código HTML del elemento de sitio web que reemplaza la campaña.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Fijo </strong></p></td> 
   <td colspan="1" rowspan="1">La casilla Fijo está seleccionada de forma predeterminada para la campaña En zona y mantiene la campaña En zona en su posición de identificación de zona durante toda la sesión del visitante en el sitio web. Se recomienda tener siempre una Zona de entrada definida como Fijo.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Desvanecimiento</strong> </p></td> 
   <td colspan="1" rowspan="1">Al seleccionar la casilla de verificación Utilizar efecto y Desvanecer se produce un efecto de atenuación en el área de identificación de zona del sitio web. Si la zona de entrada es una pancarta gráfica, la página primero se carga y, a continuación, la campaña se activa con un efecto de atenuación.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Deslizamiento</strong></td> 
   <td colspan="1">Al seleccionar la casilla de verificación Usar efecto y la opción Diapositiva, se proporciona un deslizamiento en el área de identificación de zona del sitio web. Si la zona de entrada es una pancarta gráfica, la página primero se carga y, a continuación, la campaña se activa con un efecto deslizante de izquierda a derecha.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editor de texto enriquecido  </strong></td> 
   <td colspan="1">El editor de texto enriquecido permite dar formato al texto, vincular e insertar imágenes. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Lea más aquí</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Previsualización en el sitio   </strong></td> 
   <td colspan="1">Campañas de previsualización antes de que se inicien. <br> 
    <ul> 
     <li> URL: introduzca una URL de ejemplo en la que se ejecutaría la campaña para ver un ejemplo de previsualización de cómo se vería la campaña en directo.</li> 
     <li>Dispositivo: Previsualización cómo aparecerá su campaña por dispositivo: Ordenador, Vertical Móvil, Horizontal Móvil, Vertical Tablet, Horizontal Vertical Vertical.</li> 
     <li> Previsualización: haga clic en <strong>Previsualización</strong> para abrir una nueva ventana de la URL de ejemplo para ver cómo reacciona la campaña.</li> 
     <li> Compartir: utilice el botón Compartir para enviar un correo electrónico a un colega con un vínculo para ver la campaña proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Acelere y simplifique el proceso de creación de campañas mediante el uso de [plantillas integradas](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) o [guardando la campaña existente](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) como una plantilla para reutilizarla.

>[!NOTE]
>
>**¿Desea realizar una prueba A/B de sus campañas web?** Se puede probar una o varias campañas web  [A/B para obtener resultados](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md) óptimos. Con la función de ajuste automático, la plataforma reconoce automáticamente las campañas de mejor rendimiento, continúa con las campañas de conversión más elevadas y pone en pausa las demás.

## Editar una Campaña Web {#edit-a-web-campaign}

En la página **Campañas Web**, haga clic en **Editar** en la Campaña.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Para facilitar la búsqueda de la campaña deseada, utilice la función [filter](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Previsualización de una Campaña Web {#preview-a-web-campaign}

1. En la página Campañas Web, haga clic en **Previsualización** en la campaña Web que desee vista.

   ![](assets/in-zone-web-campaign-preview.png)

## Clonar una Campaña Web {#clone-a-web-campaign}

Consulte [Clonar una Campaña Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Eliminar una Campaña Web {#delete-a-web-campaign}

1. En la página Campañas Web, haga clic en **Eliminar** en la Campaña que desee eliminar.

   ![](assets/in-zone-web-campaign-delete.png)

1. Aparecerá un mensaje de confirmación para confirmar si desea eliminar la Campaña.

>[!MORELIKETHIS]
>
>* [Crear una nueva Campaña Web de utilidades](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Crear una nueva Campaña web de cuadro de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)

