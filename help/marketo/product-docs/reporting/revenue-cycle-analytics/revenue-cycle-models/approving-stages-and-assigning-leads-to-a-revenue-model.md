---
unique-page-id: 4718683
description: Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos - Documentos de Marketo - Documentación del producto
title: Aprobación de fases y asignación de posibles clientes a un modelo de ingresos
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Aprobación de fases y asignación de posibles clientes a un modelo de ingresos {#approving-stages-and-assigning-leads-to-a-revenue-model}

Obtenga su **Modelo de ingresos** poner en marcha mediante la adición de posibles clientes existentes, la creación de reglas de asignación para cualquier posible cliente nuevo.

## Aprobación de etapas {#approving-stages}

Vamos a aprobar las etapas del modelo antes de agregar cualquier posible cliente.

1. Vaya a la **Analytics** área.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Seleccione el modelo cuyas fases desee aprobar.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. En **Acciones de modelo**, seleccione **Aprobar fases**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Se le recibirá con una alerta; haga clic en **Asignar posibles clientes**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

¡Excelente! Vamos a seguir adelante y asignar esos posibles clientes.

## Asignación de posibles clientes existentes {#assigning-existing-leads}

[Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para identificar los posibles clientes para una fase del modelo en la base de datos de posibles clientes.

1. Una vez que haya [ha creado su lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), haga clic en **Posibles clientes** pestaña.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Clic **Seleccionar todo** para seleccionar los posibles clientes.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Abra el **Acciones de posible cliente** y seleccione. **Especial**. Clic **Cambiar etapa de ingresos**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Seleccione el correcto **Modelo** y el correcto **Fase**. Clic **Ejecutar ahora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Repita el proceso hasta que todos los posibles clientes se asignen a las distintas fases del modelo.

Excelente! Para especificar cómo se asignan los nuevos posibles clientes a las fases, cree reglas de asignación.

>[!NOTE]
>
>Si el modelo está en el estado Etapas aprobadas, no verá ningún evento de etapa de ingresos de cambio en los registros de actividad de los posibles clientes. Si el modelo está totalmente aprobado, este paso de flujo se omitirá si mueve un posible cliente al mismo escenario en el que se encuentra actualmente.

## Nuevos posibles clientes: Crear reglas de asignación  {#new-leads-create-assignment-rules}

1. Clic **Inicio de Marketo** de nuevo y seleccione **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Haga clic en el modelo en el árbol y, a continuación, en la variable **Acciones de modelo** menú, seleccionar **Reglas de asignación**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Si las reglas de asignación contienen varias opciones predeterminadas, haga clic en **Fase**, realice la selección y haga clic en **Agregar opción**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Ejemplo de regla de asignación {#example-assignment-rule}

Cree una regla de puntuación de posible cliente para asignar los nuevos posibles clientes con una puntuación mínima a un paso adecuado.

1. En **If**, seleccione **Puntuación de posibles clientes**. A continuación, elija **al menos**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Entrar **40** en el campo y seleccione **Posible cliente** como escenario. Clic **Guardar** para completar.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Para aprobar el modelo, lea nuestra página de ayuda sobre **[Aprobación y desaprobación de un modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
