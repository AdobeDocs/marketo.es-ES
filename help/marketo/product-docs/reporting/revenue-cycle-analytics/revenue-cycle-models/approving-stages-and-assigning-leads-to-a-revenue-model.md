---
unique-page-id: 4718683
description: Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos - Marketo Docs - Documentación del producto
title: Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos {#approving-stages-and-assigning-leads-to-a-revenue-model}

Obtenga su **Modelo de ingresos** para su ejecución, agregue posibles clientes existentes y cree reglas de asignación para cualquier posible cliente nuevo.

## Aprobación de etapas {#approving-stages}

Aprobemos las etapas del modelo antes de agregar posibles clientes.

1. Vaya a la **Analytics** .

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Seleccione el modelo cuyas etapas desee aprobar.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. En **Acciones de modelo**, seleccione **Aprobar etapas**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Te recibirán con una alerta; click **Asignar posibles clientes**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

¡Excelente! Sigamos y asignemos esos posibles clientes.

## Asignación de posibles clientes existentes {#assigning-existing-leads}

[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para identificar los posibles clientes para una etapa del modelo en la base de datos de posibles clientes.

1. Una vez que haya [crear la lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), haga clic en **Posibles clientes** pestaña .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Haga clic en **Seleccionar todo** para seleccionar los posibles clientes.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Abra el **Acciones de posible cliente** y seleccione **Especial**. Haga clic en **Etapa de cambio de ingresos**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Seleccione el **Modelo** y la **Prueba**. Haga clic en **Ejecutar ahora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Repita el proceso hasta que todos los posibles clientes se asignen a las distintas etapas del modelo.

¡Excelente! Para especificar cómo se asignan nuevos posibles clientes a las etapas, cree reglas de asignación.

>[!NOTE]
>
>Si el modelo se encuentra en el estado Etapas aprobadas , no verá ningún evento de Etapa de cambio de ingresos en los registros de actividad de los posibles clientes. Si el modelo está totalmente aprobado, este paso de flujo se omitirá si mueve un posible cliente a la misma etapa en la que se encuentra actualmente.

## Nuevos posibles clientes: Crear reglas de asignación  {#new-leads-create-assignment-rules}

1. Haga clic en **Página principal de Marketo** de nuevo y, a continuación, seleccione **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Haga clic en el modelo en el árbol y luego en la variable **Acciones de modelo** menú, seleccionar **Reglas de asignación**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Si las reglas de asignación contienen más de una opción predeterminada, haga clic en **Prueba**, realice la selección y haga clic en **Agregar opción**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Ejemplo de regla de asignación {#example-assignment-rule}

Cree una regla de Puntuación de posible cliente para asignar los nuevos posibles clientes con una puntuación mínima a un paso adecuado.

1. En **If**, seleccione **Puntuación de posible cliente**. A continuación, elija **al menos**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Entrar **40** en el campo y seleccione **Cliente potencial de ventas** como escenario. Haga clic en **Guardar** para completar.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Para aprobar el modelo, lea nuestra página de ayuda en **[Aprobación y desaprobación de un modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
