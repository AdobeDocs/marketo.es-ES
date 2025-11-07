---
solution: Marketo Engage
product: marketo
title: Contenido condicional
description: Utilice contenido condicional en los correos electrónicos para mostrar de forma dinámica el contenido en función del destinatario.
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: fdd1cc80d215fc7dee484a9e7b9fa640a47c4519
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Contenido condicional {#conditional-content}

El contenido condicional permite controlar de forma dinámica qué contenido se ve en función de la audiencia. Utilice las segmentaciones existentes para determinar lo que ve un destinatario en función de criterios predefinidos.

>[!PREREQUISITES]
>
>Tener al menos una segmentación [creada](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) y [aprobada](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md).

## Añadir contenido condicional {#add-conditional-content}

1. Abra el correo electrónico que desee y haga clic en **Editar contenido de correo electrónico**.

   ![](assets/conditional-content-1.png)

1. Seleccione el contenido que desea que sea condicional (en este ejemplo, se elige la imagen del encabezado). Haga clic en el icono _Habilitar contenido condicional_.

   ![](assets/conditional-content-2.png)

1. La caja se vuelve naranja. A la izquierda, haga clic en el icono _Seleccionar condición_ para definir la variante.

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. Elija el segmento que desee y haga clic en **Seleccionar**.

   ![](assets/conditional-content-4.png)

1. Haga clic en el icono _Editar imagen_ para reemplazar la imagen existente de la variante. Elija el origen de la nueva imagen. En este ejemplo, elegimos la biblioteca _Imágenes y archivos_ en nuestra suscripción a Marketo Engage.

   ![](assets/conditional-content-5.png)

1. Elija la imagen aplicable y haga clic en **Seleccionar**.

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. Aparecerá la nueva imagen. Es aconsejable cambiar el nombre de la variante para que sea más fácil de identificar.

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. Para agregar variantes adicionales (opcional), haga clic en **Agregar variante** y siga los mismos pasos.

   ![](assets/conditional-content-8.png)

1. Cuando haya terminado, cada variante mostrará el contenido seleccionado.

   ![](assets/conditional-content-9.gif)

1. Los destinatarios ven el contenido en función de las reglas definidas en cada segmento. En el ejemplo anterior, todos los que tengan &quot;football&quot; en tu campo de Marketo Engage _Favorite Sport_ verán la imagen del football.

>[!MORELIKETHIS]
>
>* [Definir reglas de segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Crear un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
