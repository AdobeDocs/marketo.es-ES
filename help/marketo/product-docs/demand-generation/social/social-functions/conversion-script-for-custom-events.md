---
unique-page-id: 2950561
description: Secuencia de comandos de conversión para Eventos personalizados - Documentos de marketing - Documentación del producto
title: Secuencia de comandos de conversión para Eventos personalizados
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Secuencia de comandos de conversión para Eventos personalizados {#conversion-script-for-custom-events}

El objetivo de cumplimiento se define al crear una oferta de referencia. Si la acción que cuenta hacia el objetivo es un evento específico en su propia página web, puede utilizar una secuencia de comandos de conversión para llamar a nuestra API de JavaScript.

## Recuperar la secuencia de comandos de conversión {#retrieve-the-conversion-script}

1. Dentro del editor de ofertas de referencia, haga clic en Detalles **de** Oferta y, a continuación, seleccione Evento **de JavaScript de** cliente en la lista desplegable de objetivos de cumplimiento.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie la secuencia de comandos superior del cuadro gris y colóquela en la página web dentro de las `<body>` etiquetas . La secuencia de comandos inferior se coloca dentro de las `<header>` etiquetas .

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**Recordatorio**
   >
   >
   >Recuerde copiar y pegar ambas secuencias de comandos si se encuentran en un sitio web que no es de marketing.

## Recuperar la secuencia de comandos del cargador {#retrieve-the-loader-script}

1. Seleccione la oferta de referencia en el árbol y, a continuación, haga clic en Acciones **de Oferta de** referencia y **Código** incrustado.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Haga clic con el botón secundario en el código **de** encabezado e insértelo en el encabezado de la página web. A continuación, haga lo mismo con el Código **de** cuerpo.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Pegar las secuencias de comandos en la página web {#pasting-the-scripts-onto-your-webpage}

Pegue las secuencias de comandos de conversión en el HTML para el cuerpo y el encabezado. A continuación, coloque las secuencias de comandos del cargador en el HTML para el cuerpo y el encabezado.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conexión de la secuencia de comandos de conversión {#connecting-the-conversion-script}

Aquí es donde escribirá una función de JavaScript que utiliza la identificación HTML específica del elemento de página en el que desee activar la finalización de objetivos. Por ejemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

En este ejemplo hay un botón en la página web con un id. de &quot;#myButtonId&quot;. Cuando se hace clic en ese botón, la persona se registrará como que ha completado el objetivo.

¡Increíble! El sitio web ahora está capturando objetivos de promoción social personalizados con Marketing.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Especificar objetivo para la Oferta de referencia](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Crear una Oferta de referencia](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implementar Social en el sitio web](deploy-social-on-your-website.md)

