---
unique-page-id: 2950561
description: Script de conversión para eventos personalizados - Documentos de Marketo - Documentación del producto
title: Script de conversión para eventos personalizados
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Script de conversión para eventos personalizados {#conversion-script-for-custom-events}

El objetivo de cumplimiento se define al crear una oferta de referente. Si la acción que cuenta hacia el objetivo es un evento específico en su propia página web, puede utilizar un script de conversión para llamar a nuestra API de JavaScript.

## Recuperar el script de conversión {#retrieve-the-conversion-script}

1. Dentro del editor de ofertas de referente, haga clic en **Detalles de la oferta** y, a continuación, seleccione **Evento JavaScript del cliente** desde la lista desplegable objetivo de cumplimiento.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie la secuencia de comandos superior en el cuadro gris y colóquela en la página web dentro del `<body>` etiquetas. La secuencia de comandos inferior se coloca dentro de la variable `<header>` etiquetas.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Recuerde copiar y pegar ambos scripts si se dirigen a un sitio web que no sea de Marketo.

## Recuperar el script del cargador {#retrieve-the-loader-script}

1. Seleccione la oferta de referente en el árbol y haga clic en **Acciones de oferta de referencia** y **Código incrustado**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Haga clic con el botón derecho en el **Código de encabezado** e insértela en el encabezado de su página web. A continuación, haga lo mismo para la variable **Código de cuerpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Pegar las secuencias de comandos en la página web {#pasting-the-scripts-onto-your-webpage}

Pegue las secuencias de comandos de conversión en el HTML del cuerpo y el encabezado. A continuación, coloque las secuencias de comandos del cargador en el HTML del cuerpo y el encabezado.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conexión del script de conversión {#connecting-the-conversion-script}

Aquí es donde escribirá una función de JavaScript que utilice el identificador de HTML específico del elemento de página en el que desee almacenar en déclencheur la finalización de objetivos. Por ejemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

En este ejemplo hay un botón en la página web con un id de &quot;#myButtonId&quot;. Cuando se hace clic en ese botón, la persona se registra como que ha completado el objetivo.

¡Increíble! El sitio web ahora captura los objetivos de promoción social personalizados con Marketo.

>[!MORELIKETHIS]
>
>* [Especificar objetivo para la oferta de reenvío](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Creación de una oferta de referencia](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implementar Social en el sitio web](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

