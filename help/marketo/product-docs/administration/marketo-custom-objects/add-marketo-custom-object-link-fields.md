---
unique-page-id: 10097613
description: 'Agregar Campos De Vínculo De Objeto Personalizado De Marketo: Documentos De Marketo: Documentación Del Producto'
title: Agregar campos de vínculo de objeto personalizado de Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Agregar campos de vínculo de objeto personalizado de Marketo {#add-marketo-custom-object-link-fields}

Al crear objetos personalizados, debe proporcionar campos de vínculo para conectar el registro de objeto personalizado al registro principal correcto.

* Para una estructura personalizada de uno a varios, utilice el campo de vínculo del objeto personalizado para conectarlo a una persona o empresa.
* Para una estructura de varios a varios, se utilizan dos campos de vínculo conectados desde un objeto intermedio creado separadamente (que también es un tipo de objeto personalizado). Un vínculo se conecta a personas o empresas de la base de datos y el otro se conecta al objeto personalizado. En este caso, el campo del vínculo no se encuentra en el propio objeto personalizado.

## Crear un campo de vínculo para una estructura de uno a varios {#create-a-link-field-for-a-one-to-many-structure}

A continuación, se explica cómo crear un campo de vínculo en un objeto personalizado para una estructura de uno a varios.

1. Vaya a la **Administrador** .

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Haga clic en **Objetos personalizados de Marketo**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Seleccione el objeto personalizado de la lista.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. En el **Campos** , haga clic en **Campo nuevo**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Asigne un nombre al campo del vínculo y añada una descripción opcional. Asegúrese de seleccionar el tipo de datos Vínculo .

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Una vez aprobado el objeto personalizado, no se puede volver atrás para crear, editar o eliminar un campo de vínculo o desduplicación.

1. Seleccione si el objeto de vínculo es para un posible cliente (persona) o una empresa.

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Si elige un posible cliente, verá Id, dirección de correo electrónico y los campos personalizados de la lista.
   >
   >Si elige una empresa, verá Id y los campos personalizados en la lista.

1. Seleccione el campo de vínculo al que desea conectarse como principal del nuevo campo.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >En el campo de vínculo solo se admiten tipos de campos de cadena.

1. Haga clic en **Guardar.**

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Crear un campo de vínculo para una estructura de varios a varios {#create-a-link-field-for-a-many-to-many-structure}

A continuación, se explica cómo crear un campo de vínculo en un objeto intermedio para utilizarlo en una estructura de varios a varios.

>[!PREREQUISITES]
>
>Ya debe haber creado el objeto intermedio y los objetos personalizados a los que desea vincularlo.

1. Vaya a la **Administrador** .

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Haga clic en **Objetos personalizados de Marketo**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Seleccione el objeto intermedio al que desee añadir el campo.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. En el **Campos** , haga clic en **Campo nuevo**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Debe crear dos campos de vínculo. Crearlos de a uno. En primer lugar, asigne un nombre al campo de los miembros de la lista de la base de datos (leadID, por ejemplo). Añada una descripción opcional. Asegúrese de seleccionar el tipo de datos del vínculo.

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Una vez aprobado el objeto personalizado, no se puede volver atrás para crear, editar o eliminar un campo de vínculo o desduplicación.

1. Seleccione el objeto link de la base de datos, en este caso Lead.

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Seleccione el campo de vínculo al que desea conectarse, en este caso, Id.

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >En el campo de vínculo solo se admiten tipos de campos de cadena.

1. Haga clic en **Guardar.**

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Repita este proceso para el segundo vínculo al objeto personalizado, en este ejemplo, CourseID. El nombre del objeto del vínculo será un curso y el campo del vínculo será un ID de curso. Dado que ya ha creado y aprobado el objeto personalizado del curso, estas selecciones están disponibles en los menús desplegables.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Cree cualquier otro campo que desee utilizar en el objeto intermedio, como ensubscriptionID o grade.

## Uso de objetos personalizados {#using-custom-objects}

El siguiente paso es utilizar estos objetos personalizados en filtros en las campañas inteligentes. Con una relación de varios a varios, puede seleccionar varias personas/empresas y varios objetos personalizados. En el siguiente ejemplo, se enumerarán todos los miembros de la base de datos que coincidan con estos criterios. El campo coursename proviene del objeto personalizado del curso y el grado de inscripción procede del objeto intermedio.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Agregar campos de objeto personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar y eliminar un objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Editar y eliminar campos de objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)

