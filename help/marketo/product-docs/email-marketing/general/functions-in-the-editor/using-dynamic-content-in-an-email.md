---
unique-page-id: 2950617
description: 'Uso de contenido dinámico en un correo electrónico: documentos de Marketo, documentación del producto'
title: Uso de contenido dinámico en un correo electrónico
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Uso de contenido dinámico en un correo electrónico {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Crear una segmentación](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Utilice contenido dinámico en los correos electrónicos para enviar la información de destino de los posibles clientes.

>[!NOTE]
>
>El uso de variables dentro del contenido dinámico en un correo electrónico solo se admite cuando se utilizan campañas de Déclencheur. Se admite **no** al usar campañas por lotes.

## Añadir segmentación {#add-segmentation}

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities.png)

1. Seleccione su correo electrónico y haga clic en **Editar borrador**.

   ![](assets/1.2.png)

1. En este ejemplo estamos haciendo que la Línea de asunto sea dinámica. Haga clic en el campo Asunto y, a continuación, haga clic en el botón **Convertir en dinámico**.

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >También puede hacer que un elemento dentro del correo electrónico sea dinámico. Para ello, seleccione el área, haga clic en el icono de engranaje y seleccione **Hacer dinámico** (o [Reemplazar con fragmento](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), según lo que esté haciendo).

1. Introduzca el nombre de la segmentación, selecciónela y haga clic en **Guardar**.

   ![](assets/1.4.png)

   La segmentación y sus segmentos aparecen en la pestaña Dynamic de la derecha.

   ![](assets/1.5.png)

## Aplicar contenido dinámico {#apply-dynamic-content}

>[!CAUTION]
>
>El número de elementos de contenido dinámico permitidos no es ilimitado. Aunque no hay un límite numérico específico (puede variar en función de la combinación de contenido), el uso excesivo del contenido dinámico puede afectar negativamente al rendimiento del correo electrónico. Se recomienda mantener la cantidad de elementos de contenido dinámico utilizados por debajo de 20 por correo electrónico.

1. Haga clic en los segmentos y añada la línea de asunto.

![](assets/2.1.png)

1. Repita el proceso para cada segmento.

   ![](assets/2.2.png)

>[!TIP]
>
>Cree un correo electrónico predeterminado antes de aplicar contenido a los distintos segmentos.

>[!CAUTION]
>
>Cambios en el bloque de contenido de segmento predeterminado: se aplica a todos los segmentos.

¡Dulce! Ahora puede enviar correos electrónicos flexibles a su audiencia objetivo.

>[!MORELIKETHIS]
>
>* [Vista previa de un correo electrónico con contenido dinámico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Usar contenido dinámico en una página de aterrizaje](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
