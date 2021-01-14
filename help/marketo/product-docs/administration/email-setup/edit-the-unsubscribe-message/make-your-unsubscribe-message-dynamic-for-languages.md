---
unique-page-id: 6848782
description: Hacer que el mensaje de cancelación de suscripciones sea dinámico para los idiomas - Documentos de marketing - Documentación del producto
title: Dinamizar el mensaje de cancelación de suscripción para los idiomas
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---


# Conversión de su mensaje de cancelación de suscripción en dinámico para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

El mensaje y el vínculo predeterminados de cancelación de suscripción están en inglés. Puede utilizar contenido dinámico para mostrarlo en distintos idiomas.

>[!NOTE]
>
>Hemos preparado este pequeño tutorial para usted. Representa una práctica recomendada, pero esto puede lograrse de otras maneras.

## Preparar los datos {#prepare-your-data}

1. [Cree un ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) campo personalizado denominado &quot;Idioma preferido&quot;. (Configúrelo en su CRM si desea sincronizar este campo).

   >[!TIP]
   >
   >En el futuro, utilice este campo cuando [cree un formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar las preferencias de idioma.

## Crear segmentación {#create-segmentation}

1. Vaya a la **Base de datos**.

   ![](assets/db.png)

1. En la lista desplegable **Nuevo**, haga clic en **Nueva segmentación**.

   ![](assets/two.png)

1. Asigne un nombre al **Idioma preferido** de la segmentación. Haga clic en **Añadir segmento**. Escriba un idioma.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >El segmento predeterminado será inglés.

1. Continúe agregando segmentos hasta que se representen todos los idiomas. Haga clic en **Crear**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Seleccione un segmento.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Vaya a la ficha **Lista inteligente**. Escriba **Idioma preferido** en el campo de búsqueda. Arrastre y suelte el filtro en el lienzo.

   ![](assets/six.png)

1. Configure el idioma correspondiente correspondiente.

   ![](assets/seven.png)

1. Repita el proceso para todos los idiomas diferentes. A continuación, seleccione la lista desplegable **Acciones de segmentación** y haga clic en **Aprobar**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

## Crear un fragmento de código {#create-a-snippet}

1. Vaya a **Design Studio**.

   ![](assets/ds.png)

1. En la lista desplegable **Nuevo**, haga clic en **Nuevo fragmento**.

   ![](assets/ten.png)

1. Asigne un nombre al fragmento de código **Mensaje de cancelación de suscripción**. Haga clic en **Crear**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Escriba el mensaje predeterminado de cancelación de suscripción, resalte el mensaje y haga clic en el icono de hipervínculo.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copie y pegue este token: `{{system.unsubscribeLink}}` en el campo **URL del vínculo**. Haga clic en **Insertar**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Seleccione **Segmentar por** en la sección Segmentación.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. En la lista desplegable Segmentación, escriba **Preferred** y seleccione **Preferred Language**. Haga clic en **Guardar**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Seleccione un segmento del árbol. Escriba su mensaje de cancelación de suscripción en ese idioma.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copie y pegue el mismo token: `{{system.unsubscribeLink}}` en el campo **URL del vínculo**. Haga clic en **Insertar**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Repita el proceso para todos los segmentos. A continuación, vuelva a Design Studio, haga clic en la lista desplegable **Acciones de fragmento** y haga clic en **Aprobar**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Increíble. Casi ahí.

## Usar fragmento de código en un mensaje de correo electrónico {#use-snippet-in-an-email}

1. Dentro del editor de correo electrónico, haga clic en el elemento editable. A continuación, haga clic en el icono de engranaje y seleccione **Reemplazar con fragmento**. Si está seleccionando un elemento de fragmento editable, haga clic en el icono de engranaje y seleccione **Editar**.

   ![](assets/4.1.png)

1. Busque y seleccione el fragmento en la lista desplegable y haga clic en **Guardar**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Para probarlo, haga clic en **Atrás**...

   ![](assets/4.3.png)

1. ...a continuación, la ficha **Dynamic**.

   ![](assets/4.4.png)

1. Haga clic en los distintos idiomas para ver el cambio de fragmento.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Por supuesto, también puede editar el resto del correo electrónico para el lenguaje dinámico. Mientras esté en él, realice la misma técnica en la página de cancelación de suscripción.

## Personalización de la página de cancelación de suscripciones con contenido dinámico {#customizing-your-unsubscribe-page-with-dynamic-content}

Si desea que su gente venga a una página de cancelación de suscripción en su idioma preferido, puede utilizar contenido dinámico en la página de aterrizaje y en la página de confirmación.

1. Vaya a Design Studio.

   ![](assets/ds.png)

1. Escriba _Cancelar suscripción_ en el campo de búsqueda. Debería encontrar sus páginas de cancelación de suscripción.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

1. Haga clic en **Editar borrador**.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

1. Seleccione **Segmento por**.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

1. Busque el segmento Idioma preferido. Haga clic en **Guardar**.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Edite su contenido para cada página de aterrizaje, apruebe, ¡y ya está listo!

   >[!NOTE]
   >
   >Obtenga más información sobre [contenido dinámico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) y todo lo interesante que puede hacer.
