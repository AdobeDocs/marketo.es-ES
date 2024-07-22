---
unique-page-id: 12983101
description: 'Asignación de campos personalizados a Marketo: documentos de Marketo, documentación del producto'
title: Asignar campos personalizados a Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Asignar campos personalizados a Marketo {#map-custom-fields-to-marketo}

De forma predeterminada, es posible que desee recopilar más información que la información estándar que almacena Facebook, como la frecuencia con la que alguien utiliza su servicio de envío en línea. Puede lograr esto [creando preguntas personalizadas](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) en sus anuncios de posibles clientes de Facebook.

Sin embargo, **Marketo no comenzará a recopilar automáticamente estos datos**. Para que Marketo empiece a capturar valores de campos personalizados, **debe** asignar esos campos personalizados a un campo de Marketo.

A continuación, se indica cómo configurarlo en el área de LaunchPoint de Admin.

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de Administración y haga clic en **LaunchPoint**. En Servicios instalados, busque y edite **Anuncios de posibles clientes de Facebook**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Haga clic en **Siguiente**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Deje la cuenta autorizada tal cual: **no** realiza ningún cambio. Haga clic en **Siguiente**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Como antes, deje las páginas seleccionadas tal cual: **no** realiza ningún cambio. Haga clic en **Siguiente**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Aquí es donde se asigna el campo personalizado de Facebook al campo de Marketo. Haga clic en **Agregar.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. En la nueva fila, introduzca el nombre del campo personalizado de Facebook.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Solo los campos que se hayan guardado en plantillas de formulario de Facebook aparecerán como opciones aquí.

1. Haga clic en la columna **Campo de Marketo**. Escriba para buscar el campo al que desea asignar. Una vez que haya seleccionado un campo, haga clic en **Guardar**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Si todavía no tiene un campo en Marketo al que asignar el campo Facebook, aprenda a [crear campos personalizados](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Usted **debe** pasar por este proceso para cualquier nuevo campo de Facebook a fin de que Marketo recopile los datos.
