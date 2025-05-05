---
unique-page-id: 10095554
description: 'Incrustar un formulario en una campaña web: documentos de Marketo, documentación del producto'
title: Incrustar un formulario en una campaña web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Incrustar un formulario en una campaña web {#embed-a-form-into-a-web-campaign}

Consulte cómo incrustar un formulario de Marketo en una campaña web (cuadro de diálogo, zona interna o widget).

1. Haga clic con el botón derecho en un formulario aprobado. Seleccionar **código incrustado**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copie el código.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. En Web Personalization, vaya a **Campañas web**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Haga clic en **Crear nueva campaña**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. En el Editor de texto enriquecido, haga clic en el icono HTML.

   ![](assets/five-1.png)

1. Pegue el código incrustado del formulario en el Editor de Source de HTML. Haga clic en **Actualizar**.

   ![](assets/six-1.png)

1. El formulario no se mostrará en la vista del editor, pero puede previsualizarlo para ver cómo se procesará en una campaña.

1. Haga clic en **Iniciar** para iniciar la campaña.

   >[!NOTE]
   >
   >Cualquier cambio en los campos del formulario debe realizarse dentro de las actividades de marketing de Marketo en Editar borrador del formulario.

## Tres formas de agregar una imagen de fondo a un formulario {#three-ways-to-add-a-background-image-to-a-form}

Para agregar una imagen de fondo al formulario, puede:

* Editar el CSS de una temática de formulario
* Cambio de los colores de los cuadros de diálogo o los widgets en Definir campaña
* Añadir código CSS al script

Para editar el CSS de una temática de formulario, consulte [este artículo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Para cambiar los colores de los cuadros de diálogo o los widgets en Definir campaña:

1. En el Editor de texto enriquecido, seleccione un tipo de campaña de cuadro de diálogo y un estilo de cuadro de diálogo, color de encabezado y color de fondo para personalizar los colores de fondo del formulario. Haga clic en **Guardar**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. A continuación se muestra un ejemplo del aspecto de un estilo de cuadro de diálogo de recorte moderno con un encabezado y un color de fondo morados claros.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Para agregar código CSS al script:

1. En el Editor de texto enriquecido, haga clic en el icono HTML.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Pegue el código incrustado del formulario con el código de estilo de fondo en el Editor de Source de HTML. Haga clic en **Actualizar**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Haga clic en **Vista previa** para ver cómo se procesará en una campaña (el formulario no se mostrará en la vista del editor). Este es un ejemplo de cómo se procesa el código de formulario anterior en una campaña con una imagen de fondo.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Editar el CSS de un tema de formulario](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Mostrar mensaje de agradecimiento sin una página de aterrizaje de seguimiento](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
