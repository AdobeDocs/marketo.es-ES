---
unique-page-id: 2949962
description: Alternar dinámicamente la visibilidad de un campo de formulario - Documentos de marketing - Documentación del producto
title: Alternar dinámicamente la visibilidad de un campo de formulario
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---


# Alternar dinámicamente la visibilidad de un campo de formulario {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Añadir una lista de selección de país en el formulario](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



Una característica realmente interesante de los formularios de Marketing es que puede ocultar o mostrar dinámicamente campos de formulario o [conjuntos de campos](add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Ejemplo**
>
>En este ejemplo, ocultemos el campo **Estado** a menos que **País** esté seleccionado como &quot;Estados Unidos&quot;.

1. Vaya a **Marketing** **Actividades**.

   ![](assets/login-marketing-activities-8.png)

1. Seleccione el formulario y haga clic en **Editar** **Formulario**.

   ![](assets/editform-1.png)

1. Seleccione el campo que desee ocultar/mostrar dinámicamente y haga clic en el vínculo para **Visibilidad** **Reglas**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Busque y seleccione el campo alrededor del cual desee generar una condición.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Seleccione el operador.

   >[!TIP]
   >
   >Esto es genial porque puedes elegir partidos borrosos como &quot;inicios con&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Seleccione los valores que desea buscar y haga clic fuera de la lista desplegable.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Puede seleccionar varios valores haciendo clic en ellos mientras está abierta la lista desplegable. Por ejemplo, puede seleccionar Estados Unidos y Canadá.

   >[!NOTE]
   >
   >Anteriormente convertimos País en un tipo de campo de lista de acopio y [agregamos todos los países como valores](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

¡Y eso es todo! Ahora, cuando las personas rellenan este formulario y seleccionan Estados Unidos para País, el campo Estado aparecerá dinámicamente con las opciones especificadas.

>[!NOTE]
>
>**Buceo profundo**
>
>¿Desea obtener más información sobre [formularios](http://docs.marketo.com/display/docs/forms)?

