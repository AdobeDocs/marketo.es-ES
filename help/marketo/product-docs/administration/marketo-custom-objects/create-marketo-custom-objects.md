---
unique-page-id: 10093192
description: Creación de objetos personalizados de marketing - Documentos de marketing - Documentación del producto
title: Crear objetos personalizados de marketing
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# Crear objetos personalizados de marketing {#create-marketo-custom-objects}

Utilice objetos personalizados en Marketing para rastrear métricas específicas de su negocio. Esto puede ser cualquier cosa, desde autos, hasta cursos... todo lo que te gustaría modelar en Marketing para ejecutar tus campañas.

>[!NOTE]
>
>Puede configurar objetos personalizados para que funcionen de uno a varios o de varios a varios. El objeto inicial se crea del mismo modo, pero los pasos son diferentes cuando se inicio agregar campos al objeto. Consulte [Explicación de los objetos](understanding-marketo-custom-objects.md) personalizados de marketing para obtener más información.

>[!NOTE]
>
>Una vez aprobado el objeto personalizado, no se puede crear, editar ni eliminar un vínculo ni un campo de desduplicación.

## Creación de un objeto personalizado para una estructura de uno a varios {#create-a-custom-object-for-a-one-to-many-structure}

En este ejemplo se muestra un objeto personalizado Car, que se utiliza en una estructura de uno a varios. Posteriormente, creará un objeto personalizado de curso y un objeto intermedio para utilizarlo en una estructura de varios a varios.

1. Haga clic en **Administración** y, en Administración **de** bases de datos, seleccione **Comercializar objetos** personalizados.

   ** ![](assets/image2016-1-18-13-3a12-3a19.png)

   **

1. Haga clic en **Nuevo objeto** personalizado.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >La ficha Objetos personalizados de marketing muestra todos los objetos personalizados de la derecha y los detalles de los aprobados, incluido el número de registros y campos en la actualización más reciente.

1. Introduzca un nombre para mostrar. El nombre de la API y el nombre plural se rellenan automáticamente. Introduzca una descripción (opcional).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Puede editar estos campos cuando los esté creando, pero una vez guardados, sólo puede editar el campo Nombre plural y el control deslizante **Mostrar en detalle** de posible cliente.

1. Tire del control deslizante **Mostrar en detalle de posibles clientes **para mostrar **Mostrar** si desea realizar la vista de datos de objetos personalizados en la página Base de datos de posibles clientes. Haga clic en **Guardar**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. La información del objeto personalizado muestra el contenido introducido. Observe que está en estado Borrador.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   El siguiente paso es agregar campos para [crear el objeto](add-marketo-custom-object-fields.md)personalizado.

   >[!NOTE]
   >
   >Solo puede rellenar Objetos personalizados de marketing mediante una importación de listas o la [API](http://developers.marketo.com/documentation/rest/).

## Creación de un objeto personalizado para una estructura de varios a varios {#create-a-custom-object-for-a-many-to-many-structure}

En este ejemplo se muestra un objeto personalizado de curso que se utilizará para crear una relación de varios a varios entre personas/compañías y cursos. Cuando haya terminado, creará un objeto intermediario para conectarlo a personas o compañías de la base de datos.

>[!NOTE]
>
>Para una relación de varios a varios, no es necesario crear un vínculo en el objeto personalizado. En su lugar, agregará dos vínculos al objeto intermediario (véase más abajo).

1. Haga clic en **Administración** y, en Administración **de** bases de datos, seleccione **Comercializar objetos** personalizados.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Haga clic en **Nuevo objeto** personalizado.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Introduzca un nombre para mostrar. El nombre de la API y el nombre plural se rellenan automáticamente. Introduzca una descripción (opcional).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Puede editar estos campos cuando los esté creando, pero una vez guardados, sólo puede editar el campo Nombre plural y el control deslizante **Mostrar en detalle** de posible cliente.

1. Tire del control deslizante **Mostrar en detalle de posibles clientes **para mostrar Mostrar si desea realizar la vista de datos de objetos personalizados en la página Base de datos de posibles clientes. Haga clic en **Guardar**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. La información del objeto personalizado muestra el contenido introducido. Observe que está en estado Borrador.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Solo puede rellenar Objetos personalizados de marketing mediante una importación de listas o la [API](http://developers.marketo.com/documentation/rest/).

El siguiente paso es crear el objeto intermediario (ver más abajo). Pero antes de eso, se necesita crear un campo para vincularlo con él.

## Creación de un objeto intermedio {#create-an-intermediary-object}

Utilice un objeto intermedio para conectar un objeto personalizado a personas o compañías. En este ejemplo, se utiliza para conectar cursos del objeto personalizado del curso a personas o compañías de la base de datos.

>[!NOTE]
>
>No es necesario crear un objeto intermedio para una estructura de objetos personalizada de uno a varios.

1. Haga clic en **Administración** y, en Administración **de** bases de datos, seleccione **Comercializar objetos** personalizados.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Haga clic en **Nuevo objeto** personalizado.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Introduzca un nombre para mostrar. El nombre de la API y el nombre plural se rellenan automáticamente. Introduzca una descripción (opcional).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Puede editar estos campos cuando los esté creando, pero una vez guardados, solo podrá editar el campo Nombre plural y el control deslizante Mostrar en detalle de posible cliente.

1. Desplace el control deslizante **Mostrar en detalle** de posible cliente para mostrar Mostrar si desea vista los datos de objeto personalizados en la página Base de datos de posibles clientes. Haga clic en **Guardar**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. La información del objeto personalizado muestra el contenido introducido. Observe que está en estado Borrador.

   El siguiente paso es [agregar campos](add-marketo-custom-object-link-fields.md) de vínculo para conectar el objeto intermediario con una persona o compañía y un objeto personalizado.

>[!MORELIKETHIS]
>
>* [Añadir campos de objeto personalizados de marketing](add-marketo-custom-object-fields.md)
>* [Añadir campos de vínculo de objeto personalizado de marketing a](add-marketo-custom-object-link-fields.md)
>* [Explicación de los objetos personalizados de marketing](understanding-marketo-custom-objects.md)

>



