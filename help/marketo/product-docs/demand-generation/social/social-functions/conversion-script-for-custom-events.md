---
unique-page-id: 2950561
description: Script de conversión para eventos personalizados - Documentos de Marketo - Documentación del producto
title: Script de conversión para eventos personalizados
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Script de conversión para eventos personalizados {#conversion-script-for-custom-events}

El objetivo de cumplimiento se define al crear una oferta de referencia. Si la acción que cuenta para el objetivo es un evento específico en su propia página web, puede utilizar un script de conversión para llamar a nuestra API de JavaScript.

## Recuperación del script de conversión {#retrieve-the-conversion-script}

1. En el editor de ofertas de referencia, haga clic en **Detalles de oferta** y luego seleccione **Evento de JavaScript del cliente** en la lista desplegable objetivo de cumplimiento.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie el script superior en el cuadro gris y colóquelo en la página web dentro de `<body>` etiquetas. La secuencia de comandos inferior se coloca dentro de `<header>` etiquetas.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Recuerde copiar y pegar ambos scripts si van a un sitio web que no sea de Marketo.

## Recuperación del script del cargador {#retrieve-the-loader-script}

1. Seleccione la oferta de referencia del árbol y haga clic en **Acciones de oferta de referencia** y **Código incrustado**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Haga clic con el botón derecho en **Código de encabezado** e insértelo en el encabezado de la página web. A continuación, haga lo mismo para el **Código de cuerpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Pegar los scripts en la página web {#pasting-the-scripts-onto-your-webpage}

Pegue los scripts de conversión en el HTML para el cuerpo y el encabezado. A continuación, coloque los scripts del cargador en el HTML para el cuerpo y el encabezado.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conexión del script de conversión {#connecting-the-conversion-script}

Aquí es donde escribirá una función de JavaScript que utilice el ID de HTML específico del elemento de página en el que desee almacenar en déclencheur la finalización del objetivo. Por ejemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

En este ejemplo hay un botón en la página web con el ID &quot;#myButtonId&quot;. Cuando se hace clic en ese botón, la persona se registra como si hubiera completado el objetivo.

¡Increíble! El sitio web ahora captura los objetivos de promoción social personalizados con Marketo.

>[!MORELIKETHIS]
>
>* [Especificar objetivo para oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Crear una oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implementar Social en el sitio web](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
