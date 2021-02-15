---
unique-page-id: 2359807
description: Personalizar estilos de apuestas - Documentos de marketing - Documentación del producto
title: Personalizar estilos de apuestas
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Personalizar estilos de apuestas {#customize-sweepstakes-styles}

Cuando [crea una apuesta](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puede personalizar su aspecto en la página de aterrizaje.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

1. Vaya a **Actividades de marketing**.

![](assets/login-marketing-activities-1.png)

1. Seleccione las apuestas y haga clic en **Editar borrador**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. En el editor Apuestas, vaya a **Configuración de la aplicación** > **Aspecto**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Edite el texto del botón de registro y el vínculo de progreso.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Para cada elemento que desee personalizar, introduzca sus propiedades CSS personalizadas.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Ejemplo de CSS para **Botón Enter**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Imagen de ejemplo para **Botón Enter**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Si utiliza una imagen con texto, recuerde quitar el texto del campo **Botón de entrada** debajo de Texto arriba.

1. A medida que realiza cada cambio, el resultado se muestra en la previsualización Vista y edición.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Pruebe el botón en varios exploradores diferentes, incluidas versiones anteriores.

   >[!MORELIKETHIS]
   >
   >El siguiente paso es agregar [correos electrónicos de registro y cumplimiento a sus apuestas](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
