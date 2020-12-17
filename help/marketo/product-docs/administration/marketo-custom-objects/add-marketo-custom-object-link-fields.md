---
unique-page-id: 10097613
description: Añadir campos de vínculo de objeto personalizado de marketing - Documentos de marketing - Documentación de producto
title: Añadir campos de vínculo de objeto personalizado de marketing a
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Añadir campos de vínculo de objeto personalizado de marketing {#add-marketo-custom-object-link-fields}

Al crear objetos personalizados, debe proporcionar campos de vínculo para conectar el registro de objetos personalizado con el registro principal correcto.

* Para una estructura personalizada de uno a varios, utilice el campo de vínculo del objeto personalizado para conectarlo a una persona o una compañía.
* Para una estructura de varios a varios, se utilizan dos campos de vínculo, conectados desde un objeto intermedio creado por separado (que también es un tipo de objeto personalizado). Un vínculo se conecta a personas o compañías de la base de datos y el otro se conecta al objeto personalizado. En este caso, el campo de vínculo no se encuentra en el propio objeto personalizado.

## Crear un campo de vínculo para una estructura de uno a varios {#create-a-link-field-for-a-one-to-many-structure}

A continuación se muestra cómo crear un campo de vínculo en un objeto personalizado para una estructura de uno a varios.

1. Haga clic en **Administración** y, en **Administración de bases de datos**, seleccione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Seleccione el objeto personalizado en la lista.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. En la ficha **Campos**, haga clic en **Nuevo campo**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Asigne un nombre al campo del vínculo y agregue una descripción opcional. Asegúrese de seleccionar el tipo de datos Vínculo.

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Una vez aprobado el objeto personalizado, no podrá volver atrás y crear, editar o eliminar un vínculo o campo de desduplicación.

1. Seleccione si el objeto de vínculo es para un posible cliente o una compañía.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Si elige un lead, verá Id, Dirección de correo electrónico y cualquier campo personalizado en la lista.
   >
   >
   >Si elige la compañía, verá Id y los campos personalizados en la lista.

1. Seleccione el campo de vínculo al que desea conectarse como principal del nuevo campo.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >En el campo de vínculo solo se admiten los tipos de campo de cadena.

1. Haga clic en **Guardar.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Crear un campo de vínculo para una estructura de varios a varios {#create-a-link-field-for-a-many-to-many-structure}

A continuación se muestra cómo crear un campo de vínculo en un objeto intermedio para utilizarlo en una estructura de varios a varios.

>[!PREREQUISITES]
>
>Debe haber creado ya el objeto intermediario y los objetos personalizados con los que desea vincularlo.

1. Haga clic en **Administración** y, en **Administración de bases de datos**, seleccione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Seleccione el objeto intermediario al que desea agregar el campo.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. En la ficha **Campos **, haga clic en **Nuevo campo**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. Debe crear dos campos de vínculo. Crearlos de uno en uno. En primer lugar, asigne un nombre al campo de los miembros de la lista de base de datos (leadID, por ejemplo). Añada una descripción opcional. Asegúrese de seleccionar el tipo de datos del vínculo.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Una vez aprobado el objeto personalizado, no podrá volver atrás y crear, editar o eliminar un vínculo o campo de desduplicación.

1. Seleccione el objeto link de la base de datos, en este caso Lead.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Seleccione el campo de vínculo al que desea conectarse, en este caso, Id.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >En el campo de vínculo solo se admiten los tipos de campo de cadena.

1. Haga clic en **Guardar.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Repita este proceso para el segundo vínculo al objeto personalizado, en este ejemplo, CourseID. El nombre del objeto de vínculo será un curso y el campo de vínculo será un campoID. Como ya ha creado y aprobado el objeto personalizado del curso, estas selecciones están disponibles en los menús desplegables.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Cree cualquier otro campo que desee utilizar en el objeto intermediario, como enregistrationID o grade.

## Uso de objetos personalizados {#using-custom-objects}

El siguiente paso es utilizar estos objetos personalizados en filtros de sus campañas inteligentes. Con una relación de varios a varios, puede seleccionar varias personas/compañías y varios objetos personalizados. En el ejemplo siguiente, se enumerarán todos los usuarios de la base de datos que coincidan con estos criterios. El campo coursename procede del objeto personalizado del curso y el grado de matriculación procede del objeto intermedio.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Añadir campos de objeto personalizados de marketing](add-marketo-custom-object-fields.md)
>* [Editar y eliminar un objeto personalizado de marketing](edit-and-delete-a-marketo-custom-object.md)
>* [Explicación de los objetos personalizados de marketing](understanding-marketo-custom-objects.md)
>* [Editar y eliminar campos de objetos personalizados de marketing](edit-and-delete-marketo-custom-object-fields.md)

>



