---
unique-page-id: 6848782
description: Dynamic el mensaje de cancelación de suscripción para idiomas - Documentos de Marketo - Documentación del producto
title: Dynamic el mensaje de cancelación de suscripción para idiomas
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Dynamic el mensaje de cancelación de suscripción para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

El mensaje y vínculo predeterminados para darse de baja están en inglés. Puede utilizar contenido dinámico para mostrarlo en distintos idiomas.

>[!NOTE]
>
>Este artículo representa una práctica recomendada, pero se puede realizar de otras maneras.

## Preparar los datos {#prepare-your-data}

1. [Creación de un campo personalizado](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) se denomina &quot;Idioma preferido&quot;. (Configúrelo en su CRM si desea que este campo se sincronice).

   >[!TIP]
   >
   >Más adelante, utilice este campo cuando [crear un formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar las preferencias de idioma.

## Crear segmentación {#create-segmentation}

1. Vaya a la **Base de datos**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. En el **Nuevo** desplegable, haga clic en **Nueva segmentación**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Asigne un nombre a la segmentación **Idioma preferido**. Haga clic en **Añadir segmento**. Escriba un idioma.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >El segmento predeterminado será inglés.

1. Siga agregando segmentos hasta que se representen todos sus idiomas. Haga clic en **Crear**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Seleccione un segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Vaya a la **Lista inteligente** pestaña . Entrar **Idioma preferido** en el campo de búsqueda. Arrastre y suelte el filtro en el lienzo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Defina el idioma correspondiente correspondiente.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Repita el proceso para todos sus idiomas. A continuación, seleccione la **Acciones de segmentación** y haga clic en **Aprobar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Crear un fragmento {#create-a-snippet}

1. Vaya a la **Design Studio**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. En el **Nuevo** menú desplegable, haga clic en **Nuevo fragmento**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Asigne un nombre al fragmento **Dar de baja un mensaje**. Haga clic en **Crear**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Escriba el mensaje predeterminado de cancelación de suscripción, resalte el mensaje y haga clic en el icono de hipervínculo.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copie y pegue este token: `{{system.unsubscribeLink}}` en el **URL** campo . Haga clic en **Insertar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Select **Segmentar por** en la sección Segmentación .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. En la lista desplegable Segmentación , escriba **Preferido** y seleccione **Idioma preferido**. Haga clic en **Guardar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Seleccione un segmento del árbol. Haga clic en su cancelación de suscripción y luego en el icono del vínculo .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Asegúrese de `{{system.unsubscribeLink}}` sigue en el campo URL . Edite Mostrar texto para que coincida con el idioma seleccionado. Haga clic en **Aplicar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Repita el proceso para todos los segmentos. A continuación, vuelva a Design Studio y haga clic en el **Acciones de fragmento** y haga clic en **Aprobar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Increíble. ¡Casi ahí!

## Utilizar fragmento de código en un correo electrónico {#use-snippet-in-an-email}

1. Dentro del editor de correo electrónico, haga clic en el elemento editable . A continuación, haga clic en el icono de engranaje y seleccione **Reemplazar con fragmento**. Si está seleccionando un elemento de fragmento editable, haga clic en el icono de engranaje y seleccione **Editar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Busque y seleccione el fragmento en la lista desplegable y haga clic en **Guardar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Para probarlo, haga clic en **Atrás**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...a continuación, la variable **Dinámica** pestaña .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Haga clic en los distintos idiomas para ver el cambio de fragmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Por supuesto, también puede editar el resto del correo electrónico para el lenguaje dinámico. Mientras esté en él, realice la misma técnica en la página de cancelación de suscripción.

## Personalización de la página de cancelación de suscripción con contenido dinámico {#customizing-your-unsubscribe-page-with-dynamic-content}

Si desea que sus usuarios vayan a una página de cancelación de suscripción en su idioma preferido, puede utilizar contenido dinámico en la página de aterrizaje y la página de confirmación.

1. Vaya a la **Design Studio**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Escriba en _Cancelar suscripción_ en el campo de búsqueda y seleccione la página de cancelación de suscripción que desee.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Haga clic en **Editar borrador**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Select **Segmentar por**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Busque el segmento Idioma preferido . Haga clic en **Guardar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Edite el contenido de cada página de aterrizaje, apruebe y ya estará listo.

   >[!NOTE]
   >
   >Más información sobre [contenido dinámico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) y todas las cosas geniales que puedes hacer.
