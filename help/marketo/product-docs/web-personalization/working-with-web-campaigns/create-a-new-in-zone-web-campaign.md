---
unique-page-id: 4719400
description: Creación de una nueva campaña web en la zona - Documentos de Marketo - Documentación del producto
title: Creación de una nueva campaña web en la zona
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Creación de una nueva campaña web en la zona {#create-a-new-in-zone-web-campaign}

Una campaña web es una reacción personalizada asociada a un segmento específico y puede ser un [cuadro de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) en tu sitio web, un reemplazo de zona, una [característica de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) o una alerta por correo electrónico. Una campaña web In Zone reemplaza un elemento del sitio web basado en el ID de zona con contenido o titulares gráficos.

## Creación de una campaña web en la zona {#create-an-in-zone-web-campaign}

1. Vaya a **[!UICONTROL Campañas web]**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Seleccione **[!UICONTROL Crear nueva campaña web].**

   ![](assets/create-new-web-campaign-hand.png)

1. Seleccione el tipo de campaña **[!UICONTROL En la zona]**. Personalice y agregue un **[!UICONTROL ID de zona].** Establece la campaña en **[!UICONTROL Adhesiva]** y agrega tu elemento creativo en el editor. Agregue la dirección URL de la página para obtener una vista previa y haga clic en **[!UICONTROL Vista previa]** para ver cómo reaccionará la campaña en el sitio.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**¿Qué es un ID de zona?**
   >
   >Un ID de zona es donde desea que se encuentre la campaña web &quot;[!UICONTROL En la zona]&quot;. Para encontrar un &quot;[!UICONTROL ID de zona]&quot;, simplemente vaya a su sitio web, seleccione el área que desee reemplazar con una campaña web y haga clic con el botón derecho. En Chrome, la opción es &quot;Inspeccionar elemento&quot;, pero en otros navegadores puede variar.
   >
   >A continuación, desea encontrar el &quot;id&quot; asociado con esta sección del sitio web, que se resalta porque está inspeccionando ese elemento. Por ejemplo, si una vez que hace clic con el botón secundario en Chrome, el texto resaltado indica `<div id="featured-slider">`, entonces &quot;deslizador destacado&quot; es lo que debe escribir en la sección &quot;id de zona&quot;. Normalmente se utiliza &quot;div id&quot;, pero también se puede utilizar cualquier ID, como h1 id, p id, etc.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nombre</th> 
   <th colspan="1" rowspan="1">Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> ID de zona </strong></td> 
   <td colspan="1" rowspan="1"><p>Introduzca el nombre del ID que se encuentra en el código HTML del elemento del sitio web al que sustituye la campaña.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Adhesivo </strong></p></td> 
   <td colspan="1" rowspan="1">La casilla de verificación "Adhesivo" está seleccionada de forma predeterminada para la campaña "En zona" y mantiene la campaña "En zona" en su posición de ID de zona durante toda la sesión del visitante en el sitio web. Se recomienda tener siempre una zona de entrada configurada como fija.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> se desvanece</strong> </p></td> 
   <td colspan="1" rowspan="1">Al seleccionar la casilla de verificación Usar efecto y Atenuación, se produce un efecto de atenuación en el área ID de zona del sitio web. Si la zona de entrada es un banner gráfico, la página primero se carga y luego la campaña se activa con un efecto de atenuación.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Deslizante</strong></td> 
   <td colspan="1">Al seleccionar la casilla de verificación Usar efecto y la opción Deslizamiento, se produce un deslizamiento en el área ID de zona del sitio web. Si la zona de entrada es un banner gráfico, la página primero se carga y luego la campaña se activa con un efecto deslizante de izquierda a derecha.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editor de texto enriquecido  </strong></td> 
   <td colspan="1">El editor de texto enriquecido permite dar formato al texto, vincular e insertar imágenes. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Más información aquí</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Vista previa en el sitio   </strong></td> 
   <td colspan="1">Previsualice las campañas antes de iniciarlas. <br> 
    <ul> 
     <li> URL: introduzca una URL de ejemplo en la que se ejecutaría la campaña para ver un ejemplo de vista previa del aspecto que tendría la campaña en directo.</li> 
     <li>Dispositivo: obtenga una vista previa del aspecto de la campaña por dispositivo: Escritorio, Móvil vertical, Móvil horizontal, Tablet vertical, Vertical horizontal.</li> 
     <li> Vista previa: haga clic en <strong>Vista previa</strong> para abrir una nueva ventana de la URL de ejemplo y ver cómo reacciona la campaña.</li> 
     <li> Compartir: utilice el botón Compartir para enviar un correo electrónico a un compañero con un vínculo para ver la campaña de proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Acelere y simplifique su proceso de creación de campañas utilizando nuestras [plantillas integradas](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) o [guardando su campaña existente](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) como plantilla para reutilizarla.

>[!NOTE]
>
>**¿Desea probar sus campañas web?** Una o más campañas web se pueden [probar A/B para obtener resultados óptimos](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Con la función Ajuste automático, la plataforma reconoce automáticamente las campañas con mejor rendimiento, continúa con las campañas de conversión más altas y pausa las demás.

## Edición de una campaña web {#edit-a-web-campaign}

En la página **Campañas web**, haga clic en **Editar** en la campaña.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Para facilitar la búsqueda de la campaña que desea, use la [característica de filtro](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Previsualización de una campaña web {#preview-a-web-campaign}

1. En la página [!UICONTROL Campañas web], haga clic en **[!UICONTROL Vista previa]** en la campaña web que desee ver.

   ![](assets/in-zone-web-campaign-preview.png)

## Clonar una campaña web {#clone-a-web-campaign}

Ver [Clonar una campaña web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Eliminación de una campaña web {#delete-a-web-campaign}

1. En la página Campañas web, haga clic en **[!UICONTROL Eliminar]** en la campaña que desee eliminar.

   ![](assets/in-zone-web-campaign-delete.png)

1. Aparecerá un mensaje de confirmación para confirmar si desea eliminar la campaña.

>[!MORELIKETHIS]
>
>* [Crear una nueva campaña web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Crear una nueva campaña web de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
