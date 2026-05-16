---
unique-page-id: 6848782
description: Utilice el contenido dinámico y la segmentación para mostrar el mensaje de cancelación de suscripción y el vínculo en diferentes idiomas.
title: Haga que el mensaje de cancelación de suscripción sea dinámico para idiomas
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
TQID: https://experienceleague.adobe.com/K4c0CGEKTpE-BbYd1i6f24B8L9oltiBYo3AhI6cHHPE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 472
ht-degree: 8%

---

# Haga que el mensaje de cancelación de suscripción sea dinámico para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

El mensaje y el vínculo predeterminados para cancelar la suscripción están en inglés. Puede utilizar contenido dinámico para mostrarlos en diferentes idiomas.

>[!NOTE]
>
>Este artículo representa una práctica recomendada, pero se puede realizar de otras maneras.

## Preparación de los datos {#prepare-your-data}

1. [Cree un campo personalizado](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) con el nombre &quot;Idioma preferido&quot;. (Configúrelo en su CRM si desea que este campo se sincronice).

   >[!TIP]
   >
   >En el futuro, utilice este campo cuando [cree un formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar las preferencias de idioma.

## Crear segmentación {#create-segmentation}

1. Ir a **[!UICONTROL Base de datos]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. En el menú desplegable **[!UICONTROL Nuevo]**, haga clic en **[!UICONTROL Nueva segmentación]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Asigne un nombre a la segmentación **[!UICONTROL Idioma preferido]**. Haga clic en **[!UICONTROL Agregar segmento]**. Escriba en un idioma.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >El segmento predeterminado será el inglés.

1. Continúe añadiendo segmentos hasta que se representen todos los idiomas. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Seleccione un segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Vaya a la pestaña **[!UICONTROL Lista inteligente]**. Escriba **[!UICONTROL Idioma preferido]** en el campo de búsqueda. Arrastre y suelte el filtro en el lienzo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Configure el idioma correspondiente adecuado.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Repita el proceso para todos los idiomas. A continuación, seleccione la lista desplegable **[!UICONTROL Acciones de segmentación]** y haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Crear un fragmento {#create-a-snippet}

1. Vaya a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. En la lista desplegable **[!UICONTROL Nuevo]**, haga clic en **[!UICONTROL Nuevo fragmento]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Asigne un nombre al fragmento **Mensaje de cancelación de suscripción**. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Escriba el mensaje de cancelación de suscripción predeterminado, resáltelo y haga clic en el icono de hipervínculo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copie y pegue este token: `{{system.unsubscribeLink}}` en el campo **[!UICONTROL URL]**. Haga clic en **[!UICONTROL Insertar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Seleccione **[!UICONTROL Segmentar por]** en la sección **[!UICONTROL Segmentación]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. En el menú desplegable **[!UICONTROL Segmentación]**, escriba **[!UICONTROL Preferido]** y seleccione **[!UICONTROL Idioma preferido]**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Seleccione un segmento del árbol. Haga clic en el texto &quot;Cancelar la suscripción&quot; y luego en el icono de vínculo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Asegúrese de que `{{system.unsubscribeLink}}` se encuentre todavía en el campo **[!UICONTROL URL]**. Edite **[!UICONTROL Mostrar texto]** para que coincida con el idioma seleccionado. Haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Repita el proceso para todos los segmentos. A continuación, vuelva a **[!UICONTROL Design Studio]**, haga clic en la lista desplegable **[!UICONTROL Acciones de fragmento]** y haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

## Uso de un fragmento en un correo electrónico {#use-a-snippet-in-an-email}

1. Dentro del editor de correo electrónico, haga clic en el elemento editable. A continuación, haga clic en el icono de engranaje y seleccione **[!UICONTROL Reemplazar con fragmento]**. Si selecciona un elemento de fragmento editable, haga clic en el icono de engranaje y seleccione **[!UICONTROL Editar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Busque y seleccione su fragmento de código en la lista desplegable y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Para probar, haga clic en **[!UICONTROL Atrás]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...y luego la ficha **[!UICONTROL Dinámico]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Haga clic en los diferentes idiomas para ver cómo cambia el fragmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >También puede editar el resto del correo electrónico para lenguaje dinámico. Utilice la misma técnica en la página de cancelación de suscripción.

## Personalización de la página de cancelación de suscripción con contenido dinámico {#customize-your-unsubscribe-page-with-dynamic-content}

Si desea que sus recursos accedan a una página de cancelación de suscripción en su idioma preferido, puede utilizar contenido dinámico en la página de aterrizaje y en la página de confirmación.

1. Vaya a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Escriba _Cancelar la suscripción_ en el campo de búsqueda y seleccione la página Cancelar la suscripción que desee.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Haga clic en **[!UICONTROL Editar borrador]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Seleccionar **[!UICONTROL Segmento Por]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Busque el segmento **[!UICONTROL Idioma preferido]**. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   >[!NOTE]
   >
   >Más información sobre [contenido dinámico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md).
