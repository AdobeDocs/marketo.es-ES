---
unique-page-id: 2360403
description: Comparar la eficacia del programa con el Analizador de programas - Documentos de Marketo - Documentación del producto
title: Comparar la eficacia del programa con el analizador de programas
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Comparar la eficacia del programa con el analizador de programas {#compare-program-effectiveness-with-the-program-analyzer}

Utilice el Analizador de programas para identificar los programas más y menos eficaces, comparando costos de programa, adquisición de miembros, canalización e ingresos.

>[!PREREQUISITES]
>
>[Crear un analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Haga clic en **Analytics**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Seleccione el Analizador de programas.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Cambie Ver a Por programa.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Utilice el filtro de canal para reducir la vista a uno o dos canales. Por ahora, veremos los programas en el canal Tradeshow.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Una forma rápida de filtrar programas a un solo canal es seleccionar **Ver** > **Por canal**, haga clic en la burbuja de ese canal y, a continuación, haga clic en el nombre del canal en el cuadro de diálogo emergente.

1. Utilice la lista desplegable Eje X para elegir una métrica para el eje horizontal. Empezaremos con Costo del programa.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Utilice la lista desplegable Eje Y para elegir una métrica para el eje vertical. Elijamos Nuevos Nombres para encontrar programas que sean buenos para capturar nuevos posibles clientes.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Active los controles deslizantes para aumentar.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >También puede intentar mejorar la vista cambiando de una escala lineal a una logarítmica o viceversa. Utilice la variable **Escala** en la parte superior.

1. Explorar el gráfico resultante.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   En nuestro ejemplo, aprendemos que la Exposición Origami es mucho mejor que todos los demás programas de ese canal para capturar nuevos nombres y a un costo medio. Pero esa no es toda la historia. Agregaremos dos métricas más para comprender mejor.

1. Utilice la lista desplegable Tamaño de burbujas para elegir una métrica que comparar según el tamaño de las burbujas. Seleccionaremos (FT) Ingresos Ganados para nuestro ejemplo.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Muchas de las métricas que puede elegir en el analizador de programas están disponibles con cálculos de primer toque (FT) y de varios contactos (MT). Es importante comprender el [diferencia entre la atribución de FT y MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Observe cómo las burbujas cambian de tamaño en el gráfico.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   Añadiendo **(FT) Ganancias**, vemos rápidamente que, mientras la Exposición Origami adquirió muchos nombres nuevos, resulta en ingresos comparativamente bajos. Además, vemos que el programa del Festival de Papel 12 está obteniendo menos pero mejores nombres, ya que influye en más ingresos ganados (burbuja mayor).

1. Utilice la lista desplegable Color para añadir una cuarta métrica. Observaremos los ingresos de inversión (FT).

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Observe cómo cambian los colores en el gráfico.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Vemos que el programa del Festival de Papel 12 no sólo influye en más ingresos (burbuja mayor), sino que, a pesar de su costo relativamente alto del programa (en el extremo derecho), tiene el mejor retorno a la inversión (burbuja más verde) de todos los programas del canal de Tradeshow.

>[!TIP]
>
>Puede comparar rápidamente los programas de un canal con los de otro. Utilice el **Filtro de canal** en la parte superior de la ventana para añadir más canales.

>[!MORELIKETHIS]
>
>* [Exploración de los detalles del programa y el canal con el analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparar la eficacia del canal con el analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)

