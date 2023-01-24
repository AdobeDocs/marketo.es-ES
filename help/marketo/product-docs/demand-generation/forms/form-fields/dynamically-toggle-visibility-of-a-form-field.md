---
unique-page-id: 2949962
description: 'Alternar dinámicamente la visibilidad de un campo de formulario: Documentos de Marketo: Documentación del producto'
title: Alternar dinámicamente la visibilidad de un campo de formulario
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
source-git-commit: 0aa754bb3fb9057aaec87dc41743711fb15f8d62
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Alternar dinámicamente la visibilidad de un campo de formulario {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Agregar una lista de selección de países al formulario](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Una característica realmente interesante de los formularios de Marketo es que puede ocultar o mostrar dinámicamente campos de formulario o [campos](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Ejemplo**
>
>En este ejemplo, ocultemos la variable **Estado** field **País** se selecciona como &quot;Estados Unidos&quot;.

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Seleccione el formulario y haga clic en **Editar formulario**.

   ![](assets/editform-1.png)

1. Seleccione el campo que desee ocultar o mostrar dinámicamente y haga clic en el vínculo para **Reglas de visibilidad**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Busque y seleccione el campo en el que desea crear una condición.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Seleccione el operador .

   >[!TIP]
   >
   >Esto es genial porque puedes elegir partidos difusos como &quot;comienza con&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Seleccione los valores que desea buscar y haga clic fuera de la lista desplegable.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Puede seleccionar varios valores haciendo clic en ellos mientras la lista desplegable está abierta. Por ejemplo, puede seleccionar Estados Unidos y Canadá.

   >[!NOTE]
   >
   >Anteriormente convertimos País en un tipo de campo de lista de selección y [se han agregado todos los países como valores](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Haga clic en **Guardar**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

¡Y eso es todo! Ahora, cuando las personas rellenen este formulario y seleccionen Estados Unidos para País, el campo Estado aparecerá dinámicamente con las opciones especificadas.

>[!IMPORTANT]
>
>El comportamiento de los campos de formulario funcionará perfectamente cuando los valores de los campos se definan o actualicen mediante una secuencia de comandos personalizada mediante [Funciones de API](https://developers.marketo.com/javascript-api/forms/){target="_blank"} en Forms 2.0.
>
>Los campos condicionales pueden no funcionar como se espera si los valores de los campos se modifican mediante secuencias de comandos externas que no sean la API de JavaScript de Forms 2.0.
