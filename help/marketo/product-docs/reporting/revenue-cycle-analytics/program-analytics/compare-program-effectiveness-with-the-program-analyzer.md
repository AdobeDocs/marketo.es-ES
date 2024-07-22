---
unique-page-id: 2360403
description: Comparar la eficacia del programa con el analizador de programas - Documentos de Marketo - Documentación del producto
title: Comparar la eficacia del programa con el analizador de programas
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Comparar la eficacia del programa con el analizador de programas {#compare-program-effectiveness-with-the-program-analyzer}

Utilice el Analizador de programas para identificar los programas más eficaces y los menos eficaces, comparando los costes de los programas, las adquisiciones de miembros, la canalización y los ingresos.

>[!PREREQUISITES]
>
>[Crear un analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Haga clic en **Analytics**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Seleccione el analizador de programas.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Cambie la vista a Por programa.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Utilice el filtro de canal para reducir la vista a uno o dos canales. Por ahora, veremos los programas en el canal de Ferias.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Una forma rápida de filtrar programas a un solo canal es seleccionar **Ver** > **Por canal**, hacer clic en la burbuja de ese canal y, a continuación, hacer clic en el nombre del canal en el cuadro de diálogo emergente.

1. Utilice la lista desplegable Eje X para elegir una métrica para el eje horizontal. Empezaremos con Costo de programa.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Utilice la lista desplegable Eje Y para elegir una métrica para el eje vertical. Vamos a elegir Nuevos nombres para encontrar programas que sean buenos para capturar nuevos posibles clientes.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Encienda los controles deslizantes para aumentar.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >También puede intentar mejorar la vista cambiando de una escala lineal a una logarítmica o viceversa. Utilice el menú **Escala** de la parte superior.

1. Explore el gráfico resultante.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   En nuestro ejemplo, nos enteramos de que la Origami Expo es mucho mejor que todos los demás programas de ese canal en la captura de nuevos nombres, y a un costo medio. Pero esa no es toda la historia. Agregaremos dos métricas más para llegar a una comprensión más profunda.

1. Utilice la lista desplegable Tamaño de burbuja para elegir una métrica que comparar según el tamaño de las burbujas. Elegiremos (FT) Ingresos ganados para nuestro ejemplo.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Muchas de las métricas que puede elegir en el analizador de programas están disponibles con cálculos de primer toque (FT) y de múltiples contactos (MT). Es importante entender la [diferencia entre la atribución de FTP y MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Observe cómo las burbujas cambian de tamaño en el gráfico.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   Al agregar **(FT) Ingresos Ganados**, vemos rápidamente que, si bien la Origami Expo adquirió muchos nombres nuevos, resulta en relativamente pocos ingresos. Además, vemos que el programa Paper Fest 12 está recibiendo menos pero mejores nombres, ya que influye en más ingresos ganados (burbuja más grande).

1. Utilice la lista desplegable Color para añadir una cuarta métrica. Vamos a ver (FT) Ingresos a la Inversión.

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Observe cómo cambian los colores en el gráfico.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Vemos que el programa Paper Fest 12 no solo influye en más ingresos (burbuja más grande), sino que a pesar de su costo de programa relativamente alto (en el lado más a la derecha), tiene el mejor retorno a la inversión (burbuja más verde) de todos los programas en el canal de Ferias.

>[!TIP]
>
>Puede comparar rápidamente los programas de un canal con los de otro. Solo tienes que usar el **Filtro de canal** en la parte superior de la ventana para agregar más canales.

>[!MORELIKETHIS]
>
>* [Explorar detalles de programas y canales con el analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparar la eficacia del canal con el analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
