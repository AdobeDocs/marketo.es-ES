---
unique-page-id: 7504676
description: Explicación de los costes de periodo - Documentos de Marketo - Documentación del producto
title: Explicación de Costes de Período
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Explicación de Costes de Período {#understanding-period-costs}

## Información general {#overview}

Los costos de período se refieren al dinero que gasta en un mes específico en un programa.

>[!NOTE]
>
>**Ejemplo**
>
>Si gasta 1000 dólares para contratar un ilustrador para un libro electrónico que se lanza en julio, el programa de libros electrónicos tendría un costo de 1000 dólares en julio.
>
>Si gasta 200 $ al mes en Google Adwords, el programa Google Adwords tendría un coste de 200 $ **cada mes**.

>[!NOTE]
>
>[Explicación de programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Explicación de la pertenencia al programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Cálculo de Costes de Período {#how-period-costs-are-calculated}

Imagine un evento, como un seminario web, que se produce en marzo. Las nuevas personas son adquiridas de antemano de la publicidad en enero y febrero. Nuevos contactos también se adquieren después del evento, cuando la gente descarga el seminario web en los meses de abril y mayo.

1. Con un solo periodo de coste atribuido a marzo...

   ![](assets/graph1.png)

   ... los contactos añadidos en los meses anteriores y posteriores *solamente* Contar hacia marzo.

   ![](assets/graph2.png)

1. Con los costes del periodo atribuidos a enero, febrero y marzo...

   ![](assets/graph3.png)

   ...los contactos añadidos solo en los meses posteriores a marzo se contarán hacia marzo.

   ![](assets/graph4.png)

1. Con los costes del periodo atribuidos a enero y abril...

   ![](assets/graph5.png)

   ...los contactos agregados en los meses de enero a marzo se contarán hacia enero. Los contactos agregados en los meses de abril y mayo se contarán hacia abril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >En resumen: los meses sin un periodo definido, los costes se desplazarán &quot;hacia atrás&quot; hasta el último que se haya definido. Si no hay ningún coste de periodo anterior, los meses se trasladan &quot;hacia delante&quot; al siguiente que se haya definido. Si no se ha definido un coste de período para _cualquiera_ meses, los informes en RCE no estarán disponibles para el programa.

   >[!MORELIKETHIS]
   >
   >* [Uso de Costes de Período en un Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrado de un informe de programa por coste de período](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
