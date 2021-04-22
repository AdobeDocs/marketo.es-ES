---
unique-page-id: 10097613
description: 'Agregar Campos De Vínculo De Objeto Personalizado De Marketo: Documentos De Marketo: Documentación Del Producto'
title: Agregar campos de vínculo de objeto personalizado de Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Agregar campos de vínculo de objeto personalizado de Marketo {#add-marketo-custom-object-link-fields}

Al crear objetos personalizados, debe proporcionar campos de vínculo para conectar el registro de objeto personalizado al registro principal correcto.

* Para una estructura personalizada de uno a varios, utilice el campo de vínculo del objeto personalizado para conectarlo a una persona o empresa.
* Para una estructura de varios a varios, se utilizan dos campos de vínculo conectados desde un objeto intermedio creado separadamente (que también es un tipo de objeto personalizado). Un vínculo se conecta a personas o empresas de la base de datos y el otro se conecta al objeto personalizado. En este caso, el campo del vínculo no se encuentra en el propio objeto personalizado.

## Crear un campo de vínculo para una estructura de uno a varios {#create-a-link-field-for-a-one-to-many-structure}

Así se crea un campo de vínculo en un objeto personalizado para una estructura de uno a varios.

1. Haga clic en **Administración** y, en **Administración de bases de datos**, seleccione **Objetos personalizados de Marketo**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Seleccione el objeto personalizado de la lista.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. En la pestaña **Fields**, haga clic en **Nuevo campo**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Asigne un nombre al campo del vínculo y añada una descripción opcional. Asegúrese de seleccionar el tipo de datos Vínculo .

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Una vez aprobado el objeto personalizado, no se puede volver atrás para crear, editar o eliminar un campo de vínculo o desduplicación.

1. Seleccione si el objeto de vínculo es para un posible cliente (persona) o una empresa.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Si elige un posible cliente, verá Id, dirección de correo electrónico y los campos personalizados de la lista.
   >
   >Si elige una empresa, verá Id y los campos personalizados en la lista.

1. Seleccione el campo de vínculo al que desea conectarse como principal del nuevo campo.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >En el campo de vínculo solo se admiten tipos de campos de cadena.

1. Haga clic en **Guardar.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Crear un campo de vínculo para una estructura de varios a varios {#create-a-link-field-for-a-many-to-many-structure}

A continuación, se explica cómo crear un campo de vínculo en un objeto intermedio para utilizarlo en una estructura de varios a varios.

>[!PREREQUISITES]
>
>Ya debe haber creado el objeto intermedio y los objetos personalizados a los que desea vincularlo.

1. Haga clic en **Administración** y, en **Administración de bases de datos**, seleccione **Objetos personalizados de Marketo**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Seleccione el objeto intermedio al que desee añadir el campo.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. En la pestaña **Fields**, haga clic en **Nuevo campo**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. Debe crear dos campos de vínculo. Crearlos de a uno. En primer lugar, asigne un nombre al campo de los miembros de la lista de la base de datos (leadID, por ejemplo). Añada una descripción opcional. Asegúrese de seleccionar el tipo de datos del vínculo.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Una vez aprobado el objeto personalizado, no se puede volver atrás para crear, editar o eliminar un campo de vínculo o desduplicación.

1. Seleccione el objeto link de la base de datos, en este caso Lead.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Seleccione el campo de vínculo al que desea conectarse, en este caso, Id.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >En el campo de vínculo solo se admiten tipos de campos de cadena.

1. Haga clic en **Guardar.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Repita este proceso para el segundo vínculo al objeto personalizado, en este ejemplo, CourseID. El nombre del objeto del vínculo será un curso y el campo del vínculo será un ID de curso. Dado que ya ha creado y aprobado el objeto personalizado del curso, estas selecciones están disponibles en los menús desplegables.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Cree cualquier otro campo que desee utilizar en el objeto intermedio, como ensubscriptionID o grade.

## Uso de objetos personalizados {#using-custom-objects}

El siguiente paso es utilizar estos objetos personalizados en filtros en las campañas inteligentes. Con una relación de varios a varios, puede seleccionar varias personas/empresas y varios objetos personalizados. En el siguiente ejemplo, se enumerarán todos los miembros de la base de datos que coincidan con estos criterios. El campo coursename proviene del objeto personalizado del curso y el grado de inscripción procede del objeto intermedio.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!MORELIKETHIS]
>
>* [Agregar campos de objeto personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar y eliminar un objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Editar y eliminar campos de objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)

