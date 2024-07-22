---
unique-page-id: 10093688
description: 'Agregar campos de objeto personalizados de Marketo: documentos de Marketo, documentación del producto'
title: Agregar campos de objeto personalizados de Marketo
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 99c38fd24631e94a9554bf09de11e8eb607150d6
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Agregar campos de objeto personalizados de Marketo {#add-marketo-custom-object-fields}

Después de crear un objeto personalizado, debe agregarle campos para satisfacer sus necesidades comerciales.

Los campos definen la información específica que utiliza un objeto personalizado. Los campos de vínculo tienen un trabajo especial, para conectar objetos personalizados, y se tratan en [artículo independiente](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Haga clic en **[!UICONTROL Objetos personalizados de Marketo]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Seleccione el objeto al que desee añadir el campo a la derecha.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Haga clic en la ficha **[!UICONTROL Campos]** y luego en **[!UICONTROL Nuevo campo]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Marketo crea automáticamente los tres campos mostrados arriba cuando crea un objeto personalizado. Marketo administra estos campos automáticamente y no se pueden editar ni eliminar.

1. Escriba un [!UICONTROL Nombre para mostrar] y (opcional) [!UICONTROL Descripción].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >El nombre de la API solo se puede editar hasta que se apruebe.

1. Ahora, elija un [!UICONTROL Tipo de datos] apropiado en la lista.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Pase el control deslizante [!UICONTROL Desduplicar] si quiere usar el nuevo campo como identificador único. Haga clic en **[!UICONTROL Guardar]** para finalizar.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Los campos desduplicados se pueden utilizar para recuperar, actualizar o eliminar objetos personalizados. Cada definición de objeto personalizada debe contener al menos un campo de desduplicación (y no más de tres).

1. Añada cualquier otro campo que necesite.

   >[!NOTE]
   >
   >Si está creando una estructura &quot;uno a varios&quot;, debe añadir un campo Vínculo al objeto personalizado. Para una estructura &quot;varios a varios&quot;, no se necesita un campo de vínculo en el objeto personalizado, pero se deben añadir dos campos de vínculo en el objeto intermedio. Consulte [Agregar campos de vínculo de objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) para crear los campos de vínculo y [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obtener más información sobre los tipos de objetos personalizados.

>[!MORELIKETHIS]
>
>* [Agregar campos de vínculo de objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Editar y eliminar un objeto personalizado de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Editar y eliminar campos de objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
