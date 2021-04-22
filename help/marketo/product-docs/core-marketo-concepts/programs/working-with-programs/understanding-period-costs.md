---
unique-page-id: 7504676
description: 'Explicación de los costes de período: Documentos de Marketo: Documentación del producto'
title: Explicación de los costes de período
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Explicación de los costes de período {#understanding-period-costs}

## Información general {#overview}

Los costos de período se refieren al dinero que se gasta en un mes específico en un programa.

>[!NOTE]
>
>**Ejemplo**
>
>Si gasta $1000 para contratar un ilustrador para un eBook que se inicia en julio, el programa eBook tendría un costo de período de $1000 en julio.
>
>Si gasta $200 al mes en Google AdWords, el programa Google AdWords tendría un coste de período de $200 **cada mes**.

>[!NOTE]
>
>[Explicación de los programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Explicación de la pertenencia al programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Cómo se calculan los costes de período {#how-period-costs-are-calculated}

Imagine un evento, como un seminario web, que se produce en marzo. Las personas nuevas se adquieren de antemano a partir de la publicidad de enero y febrero. También se adquieren nuevos contactos después del evento, cuando las personas descargan el seminario web en los meses de abril y mayo.

1. Con un solo coste de período atribuido a marzo...

   ![](assets/graph1.png)

   ...los contactos agregados en los meses anteriores y posteriores *solo* contarán hacia marzo.

   ![](assets/graph2.png)

1. Con los costes de período atribuidos a enero, febrero y marzo...

   ![](assets/graph3.png)

   ...los contactos agregados solo en los meses posteriores a marzo contarán hacia marzo.

   ![](assets/graph4.png)

1. Con costes de período atribuidos a enero y abril...

   ![](assets/graph5.png)

   ...los contactos agregados en los meses de enero a marzo contarán hacia enero. Los contactos agregados en los meses de abril y mayo contarán hacia abril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >En resumen: los meses sin costes de período definidos se redistribuirán &quot;hacia atrás&quot; hasta el último que se definió. Si no hay ningún coste de período anterior, los meses se pasarán a la siguiente que se haya definido. Si no se ha definido un coste de período para _cualquier_ meses, los informes en RCE no estarán disponibles para el programa.

   >[!MORELIKETHIS]
   >
   >* [Uso de Costes de Periodo en un Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrar un informe de programa por costo de período](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

