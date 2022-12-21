---
unique-page-id: 12983101
description: Asignación de campos personalizados a Marketo - Documentos de Marketo - Documentación del producto
title: Asignación de campos personalizados a Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Asignación de campos personalizados a Marketo {#map-custom-fields-to-marketo}

Es posible que desee recopilar más información de la que Facebook almacena de forma predeterminada, como la frecuencia con la que alguien utiliza su servicio de envío en línea. Puede hacerlo de [creación de preguntas personalizadas](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) en sus anuncios principales de Facebook.

Sin embargo, **Marketo no empezará a recopilar automáticamente estos datos**. Para que Marketo empiece a capturar valores de campo personalizados, debe **must** asigne esos campos personalizados a un campo de Marketo.

A continuación se indica cómo configurarlo en el área LaunchPoint de Administración.

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Vaya al área Administración y haga clic en **LaunchPoint**. En Servicios instalados, busque y edite **Anuncios de posible cliente de facebook**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Deje la cuenta autorizada tal cual—do **not** realice cualquier cambio. Haga clic en **Siguiente**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Como antes, deje las páginas seleccionadas tal cual, haga clic en **not** realice cualquier cambio. Haga clic en **Siguiente**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Aquí es donde asigna el campo personalizado de Facebook al campo de Marketo. Haga clic en **Agregar.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. En la nueva fila, introduzca el nombre del campo personalizado de Facebook.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Solo los campos que se hayan guardado en plantillas de formulario de Facebook aparecerán como opciones aquí.

1. Haga clic en el **Campo Marketo** para abrir el Navegador. Escriba para buscar el campo al que desea asignar. Una vez seleccionado un campo, haga clic en **Guardar**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Si aún no tiene un campo en Marketo para asignar el campo Facebook a, aprenda a [crear campos personalizados](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>You **must** siga este proceso para cualquier nuevo campo de Facebook para que Marketo recopile los datos.
