---
unique-page-id: 10093188
description: Explicación de los objetos personalizados de marketing - Documentos de marketing - Documentación del producto
title: Explicación de los objetos personalizados de marketing
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---


# Explicación de los objetos personalizados de marketing {#understanding-marketo-custom-objects}

Utilice objetos personalizados para rastrear métricas específicas de su negocio.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

Utilice objetos personalizados como filtros y déclencheur en sus campañas inteligentes. Por ejemplo:

* **Filtro**: Enviar correos electrónicos sólo a los propietarios de una marca de vehículo específica
* **Déclencheur**: Enviar un correo electrónico cuando se añada un objeto personalizado a una persona o compañía.

Puede configurar objetos personalizados en una relación de uno a varios o de varios a varios. Por ejemplo:

* **Uno a varios**: Una persona posee varios coches
* **Varios a muchos**: Varios estudiantes están matriculados en varios cursos desde un catálogo de cursos

Una estructura de uno a varios utiliza un solo campo de vínculo para conectar el objeto personalizado a una persona o una compañía.

Muchos objetos personalizados utilizan dos campos de vínculo, que forman parte de un objeto intermedio. Un campo Vínculo está conectado a la persona o compañía y otro está conectado al objeto personalizado, como el catálogo del curso. Este objeto intermediario puede contener campos personalizados adicionales, como un grado de curso o una fecha de asistencia, que definen mejor la naturaleza de la conexión.

>[!TIP]
>
>Importe objetos personalizados mediante valores separados por comas (CSV) en la interfaz de usuario para probar y validar una muestra de datos. A continuación, cargue todos los archivos con una API.

>[!CAUTION]
>
>No puede restaurar objetos personalizados, por lo que asegúrese de que ya no los necesita antes de eliminarlos.

## Acceso a objetos personalizados de marketing {#accessing-marketo-custom-objects}

1. Para crear o editar objetos personalizados de Marketing to, haga clic en **Administración** y luego en el vínculo **Objetos personalizados de Marketing to**.

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. Los objetos personalizados de marketing muestran listas de todos los objetos personalizados de la derecha, pero solo los aprobados de la cuadrícula principal.

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. La cuadrícula muestra el nombre del objeto, el número de registros, el número de campos y la fecha de la actualización más reciente.

   >[!TIP]
   >
   >Marketo actualiza estos campos automáticamente, pero puede actualizar la visualización haciendo clic en el icono de la columna Registros.

1. Haga clic en el nombre del objeto a la derecha para abrir la página de detalles.

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## Objetos personalizados de vista asociados a una persona {#view-custom-objects-associated-to-a-person}

Después de crear la estructura de objetos personalizada, al cargar los datos de objetos personalizados específicos, los objetos personalizados se asocian automáticamente a las personas de la base de datos mediante el campo de vínculo del objeto personalizado. Puede realizar la vista de información desde la ficha Objetos personalizados de la página de detalles de la persona.

1. Vaya a **Base de datos**.

   ![](assets/db.png)

1. Abra la base de datos y haga clic en la ficha **Personas**. Haga clic con el doble en el registro de una persona asociada a un objeto personalizado.

   ![](assets/five.png)

1. En la página de detalles de la persona, haga clic en la ficha **Objetos personalizados**. Seleccione el objeto en la lista desplegable.

   ![](assets/six.png)

1. Ahora puede vista una lista de todos los objetos personalizados de ese tipo asociados a esa persona.

   ![](assets/seven.png)

## Uso de objetos personalizados con Compañías {#using-custom-objects-with-companies}

Un objeto personalizado vinculado a la compañía funciona mejor si sincroniza compañías desde CRM o si crea compañías explícitamente mediante la API. También se recomienda utilizar el ID de Compañía como campo de vínculo.

Si hay varias personas en Marketing que son registros en los registros de CRM o solo de marketing, un objeto personalizado vinculado a una compañía no se asociará a más de un registro individual. Esto se debe a que una compañía con varias personas debajo de ella solo se admite cuando las compañías se sincronizan desde CRM o si se utiliza una API para crear compañías explícitamente.

Los objetos personalizados solo pueden vincularse directamente a un único registro. Esto significa que cuando el tipo de objeto personalizado está vinculado por el campo de compañía, debe asegurarse de que los registros de personas están asociados a una compañía mediante la conversión de contactos en su CRM o mediante el campo externoCompanyId, si administra compañías mediante las API REST de Marketing. Para los registros de personas que no están vinculados explícitamente a registros de compañía, los objetos personalizados vinculados mediante compañía se vincularán aleatoriamente a un único registro, aunque el valor del campo de compañía se comparta entre muchas personas.

Consulte [Importar datos de objeto personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) para obtener más información.

>[!MORELIKETHIS]
>
>* [Crear objetos personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Aprobar un objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Editar y eliminar un objeto personalizado de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Añadir campos de objeto personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar y eliminar campos de objetos personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Importar datos de objeto personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

