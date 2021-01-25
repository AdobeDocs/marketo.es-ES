---
unique-page-id: 7504676
description: Explicación de los costos de período - Documentos de marketing - Documentación del producto
title: Explicación de los costos de período
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Explicación de los costos de período {#understanding-period-costs}

## Información general {#overview}

Los costos de período se refieren al dinero que usted gasta en un mes específico en un programa.

>[!NOTE]
>
>**Ejemplo**
>
>Si gasta $1000 para contratar un ilustrador para un eBook que se lanza en julio, el programa de eBook tendría un costo de período de $1000 en julio.
>
>Si gasta $200 al mes en Google Adwords - el programa Google Adwords tendría un costo de período de $200 **cada mes**.

>[!NOTE]
>
>[Explicación de los Programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Explicación de la pertenencia a Programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Cómo se calculan los costos de período {#how-period-costs-are-calculated}

Imagine un evento, como un seminario web, que se produce en marzo. Las personas nuevas se adquieren de antemano de la publicidad en enero y febrero. También se adquieren nuevos contactos después del evento, cuando las personas descargan el seminario web en los meses de abril y mayo.

1. Con un solo costo de período atribuido a marzo...

   ![](assets/graph1.png)

   ...los contactos agregados en los meses anteriores y posteriores sólo *a1/> contarán hacia marzo.*

   ![](assets/graph2.png)

1. Con los costes de período atribuidos a enero, febrero y marzo...

   ![](assets/graph3.png)

   ...los contactos agregados sólo en los meses posteriores a marzo contarán hacia marzo.

   ![](assets/graph4.png)

1. Con los costes del período atribuidos a enero y abril...

   ![](assets/graph5.png)

   ...los contactos agregados en los meses de enero a marzo contarán hacia enero. Los contactos agregados en los meses de abril y mayo contarán hacia abril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >En resumen: los meses sin costes de período definidos se desplazarán &quot;hacia atrás&quot; hasta el último que se haya definido. Si no hay ningún costo de período anterior, los meses se pasarán &quot;hacia adelante&quot; al siguiente que se haya definido. Si no se ha definido un costo de período para _cualquier_ meses, el sistema de informes en RCE no estará disponible para el programa.

   >[!MORELIKETHIS]
   >
   >* [Uso de los costos de período en un Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrar un informe de Programa por costo de período](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

