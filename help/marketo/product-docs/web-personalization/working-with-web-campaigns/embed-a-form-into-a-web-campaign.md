---
unique-page-id: 10095554
description: Incrustar un formulario en una campaña web - Documentos de Marketo - Documentación del producto
title: Incrustar un formulario en una campaña web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Incrustar un formulario en una campaña web {#embed-a-form-into-a-web-campaign}

Vea cómo incrustar un formulario de Marketo en una campaña web (Dialog, In Zone o Widget).

1. Haga clic con el botón derecho en un formulario aprobado. Select **Código incrustado**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copie el código.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. En Personalización web, vaya a **Campañas web**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Haga clic en **Crear nueva campaña**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. En el Editor de texto enriquecido, haga clic en el icono del HTML.

   ![](assets/five-1.png)

1. Pegue el código incrustado del formulario en el Editor de origen de HTML. Haga clic en **Actualizar**.

   ![](assets/six-1.png)

1. El formulario no se muestra en la vista del editor, pero puede obtener una vista previa para ver cómo se renderizará en una campaña.

1. Haga clic en **Launch** para iniciar la campaña.

   >[!NOTE]
   >
   >Cualquier cambio en los campos del formulario debe realizarse dentro de las actividades de marketing de Marketo en Editar borrador del formulario.

## Tres formas de agregar una imagen de fondo a un formulario {#three-ways-to-add-a-background-image-to-a-form}

Para agregar una imagen de fondo al formulario, puede:

* Editar la CSS de un tema del formulario
* Cambiar los colores del cuadro de diálogo o la utilidad en Establecer campaña
* Agregar código CSS al script

Para editar la CSS de un tema del formulario, consulte [este artículo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Para cambiar los colores del cuadro de diálogo o la utilidad en Set Campaign:

1. En el Editor de texto enriquecido, seleccione un tipo de campaña Cuadro de diálogo y un estilo de cuadro de diálogo, color de encabezado y color de fondo para personalizar los colores de fondo del formulario. Haga clic en **Guardar**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Aquí hay un ejemplo de cómo se ve un estilo de cuadro de diálogo de recorte moderno con un encabezado liviano morado y un color de fondo.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Para agregar código CSS al script:

1. En el Editor de texto enriquecido, haga clic en el icono del HTML.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Pegue el código incrustado del formulario con el código de estilo de fondo en el Editor de origen de HTML. Haga clic en **Actualizar**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Haga clic en **Vista previa** para ver cómo se renderizará en una campaña (el formulario no se muestra en la vista del editor). A continuación se muestra un ejemplo de cómo se procesa el código de formulario anterior en una campaña con una imagen de fondo.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Editar la CSS de un tema del formulario](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Mostrar mensaje de agradecimiento sin una página de aterrizaje de seguimiento](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://developers.marketo.com/documentation/websites/forms-2-0/)

