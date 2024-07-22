---
unique-page-id: 2360401
description: Comparación de la eficacia del canal con el analizador de programas - Documentos de Marketo - Documentación del producto
title: Comparación de la eficacia del canal con el analizador de programas
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Comparación de la eficacia del canal con el analizador de programas {#compare-channel-effectiveness-with-the-program-analyzer}

Utilice el analizador de programas para comparar los costes de canal, la adquisición de miembros, la canalización, los ingresos y mucho más, a fin de identificar los canales más eficaces y los menos eficaces.

>[!PREREQUISITES]
>
>[Crear un analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Haz clic en **Analytics** en **Mi Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Seleccione su **Analizador de programas**.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Cambiar la vista a **Por canal**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Utilice la lista desplegable **Eje X** para elegir una métrica para el eje horizontal. Empecemos con **Costo de programa**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Utilice la lista desplegable Eje Y para elegir una métrica para el eje vertical. Aquí, iremos con la canalización **(FT) creada**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Muchas de las métricas que puede elegir en el analizador de programas están disponibles con cálculos de primer toque (FT) y de múltiples contactos (MT). Es importante entender la [diferencia entre la atribución de FTP y MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Utilice la lista desplegable **Eje Y** para elegir **(MT) Canalización creada**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   En esta vista de atribución multitáctil, vemos que el canal Seminario web tiene más influencia en la canalización creada y cuesta menos que los canales de la Feria comercial y de Advertising en línea.

   Ahora vamos a añadir dos dimensiones más.

1. Utilice la lista desplegable **Tamaño de burbuja** para seleccionar una medida adicional, como **Nombres nuevos**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Observe cómo cambia el gráfico.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vemos que el canal del seminario web se encoge, según las mediciones de **Nuevos nombres**. Podemos concluir que, si bien tiene muchos miembros, es menos eficaz en la generación de nuevas pistas que el canal de la Feria.

1. Finalmente, utilice la lista desplegable Color para añadir la cuarta dimensión. Vamos a seleccionar **(FT) Ingresos obtenidos**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Observe cómo cambian los colores en el gráfico.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   A partir de los colores, nos enteramos de que el canal de la feria, la burbuja más verde, ha influido en los mayores ingresos obtenidos, según se mide por la atribución de primer contacto.

1. Ahora, si cambiamos la métrica Color a **(MT) Ingresos obtenidos**, vemos que el canal Advertising en línea, ahora el más ecológico, influyó más en los ingresos -con el tiempo- que los canales Seminario web y Feria comercial.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

En nuestro ejemplo, vemos que el canal de feria es el más caro (el más a la derecha) y el más exitoso (el más alto en el eje Y) al medir la canalización creada por el primer contacto. Ahora, consideremos la canalización de cada canal creada según lo medido por atribución multitáctil.

>[!TIP]
>
>Los ejemplos de estos pasos miden la eficacia en función de la canalización creada. Utilice la lista desplegable Eje Y para seleccionar otras formas de medir la eficacia del canal, como Nuevos nombres, Miembros, Coste por éxito, etc.

>[!MORELIKETHIS]
>
>* [Explorar detalles de programas y canales con el analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparar la eficacia del programa con el analizador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
