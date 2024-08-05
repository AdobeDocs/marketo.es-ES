---
unique-page-id: 2950561
description: Script de conversión para eventos personalizados - Documentos de Marketo - Documentación del producto
title: Script de conversión para eventos personalizados
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# Script de conversión para eventos personalizados {#conversion-script-for-custom-events}

El objetivo de cumplimiento se define al crear una oferta de referencia. Si la acción que cuenta para el objetivo es un evento específico en su propia página web, puede utilizar un script de conversión para llamar a nuestra API de JavaScript.

>[!IMPORTANT]
>
>El 31 de julio de 2024, empezamos el proceso de dejar de utilizar esta función. Ya no se pueden crear nuevos recursos. Los recursos existentes seguirán funcionando hasta el 31 de enero de 2025. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Recuperación del script de conversión {#retrieve-the-conversion-script}

1. En el editor de ofertas de reenvío, haga clic en **Detalles de la oferta** y, a continuación, seleccione **Evento de JavaScript del cliente** en la lista desplegable de objetivo de cumplimiento.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie el script superior en el cuadro gris y colóquelo en la página web dentro de las etiquetas `<body>`. El script inferior se coloca dentro de las etiquetas `<header>`.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Recuerde copiar y pegar ambos scripts si van a un sitio web que no sea de Marketo.

## Recuperación del script del cargador {#retrieve-the-loader-script}

1. Seleccione la oferta de referencia del árbol y, a continuación, haga clic en **Acciones de oferta de referencia** y en **Código incrustado**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Haga clic con el botón derecho en **Código de encabezado** e insértelo en el encabezado de la página web. Entonces haga lo mismo para el **Código de cuerpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Pegar los scripts en la página web {#pasting-the-scripts-onto-your-webpage}

Pegue los scripts de conversión en el HTML para el cuerpo y el encabezado. A continuación, coloque los scripts del cargador en el HTML para el cuerpo y el encabezado.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conexión del script de conversión {#connecting-the-conversion-script}

Aquí es donde escribirá una función de JavaScript que utiliza el ID de HTML específico del elemento de página en el que desee almacenar en déclencheur la finalización del objetivo. Por ejemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

En este ejemplo hay un botón en la página web con el ID &quot;#myButtonId&quot;. Cuando se hace clic en ese botón, la persona se registra como si hubiera completado el objetivo.

¡Fantástico! El sitio web ahora captura los objetivos de promoción social personalizados con Marketo.

>[!MORELIKETHIS]
>
>* [Especificar meta para oferta de reenvío](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Crear una oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implementar Social en su sitio web](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
