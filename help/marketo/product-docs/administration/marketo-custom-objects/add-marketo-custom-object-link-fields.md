---
unique-page-id: 10097613
description: 'Agregar campos de vínculo de objeto personalizado de Marketo: documentos de Marketo, documentación del producto'
title: Añadir campos de vínculo de objetos personalizables de Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 2%

---

# Añadir campos de vínculo de objetos personalizables de Marketo {#add-marketo-custom-object-link-fields}

Al crear objetos personalizados, debe proporcionar campos de vínculo para conectar el registro de objeto personalizado al registro principal correcto.

* Para una estructura personalizada de uno a varios, utilice el campo de vínculo del objeto personalizado para conectarlo a una persona o compañía.
* Para una estructura de varios a varios, se utilizan dos campos de vínculo, conectados desde un objeto intermedio creado por separado (que también es un tipo de objeto personalizado). Un vínculo se conecta a personas o empresas de la base de datos y el otro al objeto personalizado. En este caso, el campo de vínculo no se encuentra en el propio objeto personalizado.

>[!IMPORTANT]
>
>Marketo Engage solo admite un objeto Edge único para cada objeto Bridge en la relación de varios a varios. En el ejemplo que se muestra a continuación, cada inscripción solo puede vincularse a un único curso. Sin embargo, puede haber muchos objetos puente para cada objeto edge, al igual que hay muchas inscripciones de alumnos en cada curso (relación Varios a uno). Si los datos de objeto personalizados están estructurados de modo que haya más de un registro de objeto de Edge para cada registro de objeto de Bridge (uno a varios o varios a varios), puede crear varios registros de objeto de Bridge, cada uno de los cuales hace referencia a un único registro de objeto de Edge para representar esos datos en Marketo.

## Creación de un campo de vínculo para una estructura &quot;uno a varios&quot; {#create-a-link-field-for-a-one-to-many-structure}

A continuación, se muestra cómo crear un campo de vínculo en un objeto personalizado para una estructura &quot;uno a varios&quot;.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Haga clic en **[!UICONTROL Objetos personalizados de Marketo]**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Seleccione el objeto personalizado en la lista.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. En la ficha **[!UICONTROL Campos]**, haga clic en **[!UICONTROL Nuevo campo]**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Asigne un nombre al campo de vínculo y agregue una [!UICONTROL descripción] opcional. Asegúrese de seleccionar el tipo de datos [!UICONTROL Link].

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Una vez que se apruebe el objeto personalizado, no podrás volver atrás y crear, editar ni eliminar un [!UICONTROL vínculo] o [!UICONTROL campo desduplicado].

1. Seleccione si el [!UICONTROL objeto de vínculo] es para un [!UICONTROL posible cliente] (persona) o una [!UICONTROL empresa].

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Si eliges [!UICONTROL posible cliente], verás el identificador, la dirección de correo electrónico y cualquier campo personalizado en la lista.
   >
   >Si elige [!UICONTROL empresa], verá el identificador y cualquier campo personalizado en la lista.

1. Seleccione el [!UICONTROL campo de vínculo] al que desee conectarse como elemento principal del nuevo campo.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >Solo se admiten tipos de campos de cadena en [!UICONTROL Campo de vínculo].

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Creación de un campo de vínculo para una estructura &quot;varios a varios&quot; {#create-a-link-field-for-a-many-to-many-structure}

A continuación, se muestra cómo crear un campo de vínculo en un objeto intermedio para utilizarlo en una estructura de varios a varios.

>[!PREREQUISITES]
>
>Ya debe haber creado el objeto intermedio y los objetos personalizados con los que desea vincularlo.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Haga clic en **[!UICONTROL Objetos personalizados de Marketo]**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Seleccione el objeto intermedio al que desee agregar el campo.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. En la ficha **[!UICONTROL Campos]**, haga clic en **[!UICONTROL Nuevo campo]**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Debe crear dos campos de vínculo. Créelos de uno en uno. En primer lugar, asigne un nombre al campo de los miembros de la lista de la base de datos (por ejemplo, leadID). Agregue una [!UICONTROL descripción] opcional. Asegúrese de seleccionar el [!UICONTROL vínculo] [!UICONTROL tipo de datos].

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Una vez que se apruebe el objeto personalizado, no podrás volver atrás y crear, editar ni eliminar un [!UICONTROL vínculo] o [!UICONTROL campo desduplicado].

1. Seleccione [!UICONTROL Link Object] de la base de datos; en este caso, [!UICONTROL Lead].

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Seleccione el [!UICONTROL campo de vínculo] al que desee conectarse, en este caso, [!UICONTROL Id].

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >Solo se admiten tipos de campos de cadena en [!UICONTROL Campo de vínculo].

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Repita este proceso para el segundo vínculo a su objeto personalizado, en este ejemplo, courseID. El nombre de [!UICONTROL objeto de vínculo] será courseID y el [!UICONTROL campo de vínculo] será courseID. Dado que ya ha creado y aprobado el objeto personalizado del curso, estas selecciones están disponibles en los menús desplegables.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Cree cualquier otro campo que desee utilizar en el objeto intermedio, como enrollmentID o grade.

## Uso de objetos personalizados {#using-custom-objects}

El siguiente paso es utilizar estos objetos personalizados en filtros en sus campañas inteligentes. Con una relación &quot;varios a varios&quot;, puede seleccionar varias personas o empresas y varios objetos personalizados. En el ejemplo siguiente, se muestra cualquier persona de la base de datos que coincida con estos criterios. El campo Nombre de curso procede del objeto personalizado del curso y la nota de inscripción procede del objeto intermedio.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Agregar campos de objeto personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar y eliminar un objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Editar y eliminar campos de objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
