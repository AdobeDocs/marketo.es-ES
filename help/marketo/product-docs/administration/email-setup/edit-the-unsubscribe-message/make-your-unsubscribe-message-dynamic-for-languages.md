---
unique-page-id: 6848782
description: Haga que el mensaje de cancelación de suscripción sea dinámico para idiomas - Documentos de Marketo - Documentación del producto
title: Haga que el mensaje de cancelación de suscripción sea dinámico para idiomas
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# Haga que el mensaje de cancelación de suscripción sea dinámico para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

El mensaje y el vínculo predeterminados para cancelar la suscripción están en inglés. Puede utilizar el contenido dinámico para mostrarlo en diferentes idiomas.

>[!NOTE]
>
>Este artículo representa una práctica recomendada, pero se puede realizar de otras maneras.

## Preparación de los datos {#prepare-your-data}

1. [Crear un campo personalizado](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) se denomina &quot;Idioma preferido&quot;. (Configúrelo en su CRM si desea que este campo se sincronice).

   >[!TIP]
   >
   >En el futuro, utilice este campo cuando [creación de un formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para recopilar las preferencias de idioma.

## Crear segmentación {#create-segmentation}

1. Vaya a la **[!UICONTROL Base de datos]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. En el **[!UICONTROL Nuevo]** , haga clic en **[!UICONTROL Nueva segmentación]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Nombrar la segmentación **[!UICONTROL Idioma preferido]**. Clic **[!UICONTROL Añadir segmento]**. Escriba en un idioma.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >El segmento predeterminado será el inglés.

1. Continúe añadiendo segmentos hasta que se representen todos los idiomas. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Seleccione un segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Vaya a la **[!UICONTROL Lista inteligente]** pestaña. Entrar **[!UICONTROL Idioma preferido]** en el campo de búsqueda. Arrastre y suelte el filtro en el lienzo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Configure el idioma correspondiente adecuado.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Repita el proceso para todos los idiomas. A continuación, seleccione la **[!UICONTROL Acciones de segmentación]** y haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Crear un fragmento {#create-a-snippet}

1. Vaya a la **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. En el **[!UICONTROL Nuevo]** , haga clic en **[!UICONTROL Nuevo fragmento]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Asignar un nombre al fragmento **Mensaje de cancelación de suscripción**. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Escriba el mensaje de cancelación de suscripción predeterminado, resáltelo y haga clic en el icono de hipervínculo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copie y pegue este token: `{{system.unsubscribeLink}}` en el **[!UICONTROL URL]** field. Clic **[!UICONTROL Insertar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Seleccionar **[!UICONTROL Segmentar por]** en el **[!UICONTROL Segmentación]** sección.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. Desde el **[!UICONTROL Segmentación]** menú desplegable, escriba **[!UICONTROL Preferida]** y seleccione **[!UICONTROL Idioma preferido]**. Clic **[!UICONTROL Guardar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Seleccione un segmento del árbol. Haga clic en su cancelación de suscripción y luego en el icono de enlace.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Asegúrese de `{{system.unsubscribeLink}}` sigue en el **[!UICONTROL URL]** field. Edite el **[!UICONTROL Mostrar texto]** para que coincida con el idioma seleccionado. Clic **[!UICONTROL Aplicar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Repita el proceso para todos los segmentos. A continuación, vuelva a la **[!UICONTROL Design Studio]**, haga clic en **[!UICONTROL Acciones de fragmento]** y haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Fantástico. ¡Ya casi está!

## Usar fragmento de código en un correo electrónico {#use-snippet-in-an-email}

1. Dentro del editor de correo electrónico, haga clic en el elemento editable. A continuación, haga clic en el icono de engranaje y seleccione **[!UICONTROL Reemplazar por fragmento]**. Si está seleccionando un elemento de fragmento editable, haga clic en el icono de engranaje y seleccione **[!UICONTROL Editar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Busque y seleccione el fragmento de código de la lista desplegable y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Para probarlo, haga clic en **[!UICONTROL Atrás]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...y luego el **[!UICONTROL Dinámico]** pestaña.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Haga clic en los diferentes idiomas para ver cómo cambia el fragmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Por supuesto, también puede editar el resto del correo electrónico para lenguaje dinámico. Mientras está en ello, realice la misma técnica en la página de cancelación de suscripción.

## Personalización de la página de cancelación de suscripción con contenido dinámico {#customizing-your-unsubscribe-page-with-dynamic-content}

Si desea que sus recursos accedan a una página de cancelación de suscripción en su idioma preferido, puede utilizar contenido dinámico en la página de aterrizaje y en la página de confirmación.

1. Vaya a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Escribir en _Cancelar suscripción_ en el campo de búsqueda y seleccione la página de cancelación de suscripción deseada.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Clic **[!UICONTROL Editar borrador]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Seleccionar **[!UICONTROL Segmentar por]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Busque el **[!UICONTROL Idioma preferido]** segmento. Clic **[!UICONTROL Guardar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Edite el contenido de cada página de aterrizaje, apruébelo y ya está listo.

   >[!NOTE]
   >
   >Más información sobre [contenido dinámico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) y todas las cosas geniales que puedes hacer.
