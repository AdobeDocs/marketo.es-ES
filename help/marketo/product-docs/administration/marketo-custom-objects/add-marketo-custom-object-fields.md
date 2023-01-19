---
unique-page-id: 10093688
description: 'Agregar campos de objeto personalizados de Marketo: Documentos de Marketo: Documentación del producto'
title: Agregar campos de objeto personalizados de Marketo
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Agregar campos de objeto personalizados de Marketo {#add-marketo-custom-object-fields}

Después de crear un objeto personalizado, debe agregar campos para satisfacer las necesidades empresariales.

Los campos definen la información específica que utiliza un objeto personalizado. Los campos de vínculo tienen un trabajo especial, para conectar objetos personalizados y están cubiertos en un [artículo independiente](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Vaya a la **Administrador** .

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Haga clic en **Objetos personalizados de Marketo**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Seleccione el objeto al que desee añadir el campo a la derecha.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. En el **Campos** , haga clic en **Campo nuevo**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Marketo crea automáticamente los tres campos que se muestran arriba al crear un objeto personalizado. Marketo administra estos campos automáticamente y no puede editarlos ni eliminarlos.

1. Introduzca un nombre para mostrar y una descripción.

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >El nombre de la API solo se puede editar hasta que se apruebe.

1. Ahora, elija un tipo de datos adecuado en la lista.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Despliegue el control deslizante Desduplicación si desea utilizar el nuevo campo como identificador único. Haga clic en **Guardar** para terminar.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Los campos de desduplicación se pueden utilizar para recuperar, actualizar o eliminar objetos personalizados. Cada definición de objeto personalizada debe contener al menos un campo de desduplicación (y no más de tres).

1. Añada los demás campos que necesite.

   >[!NOTE]
   >
   >Si está creando una estructura de uno a varios, debe agregar un campo Vínculo al objeto personalizado. Para una estructura de varios a varios, no necesita un campo de vínculo en el objeto personalizado, pero debe agregar dos campos de vínculo en el objeto intermedio. Consulte [Agregar campos de vínculo de objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) para crear los campos de vínculo, y [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obtener más información sobre tipos de objetos personalizados.

>[!MORELIKETHIS]
>
>* [Agregar campos de vínculo de objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Editar y eliminar un objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Editar y eliminar campos de objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

