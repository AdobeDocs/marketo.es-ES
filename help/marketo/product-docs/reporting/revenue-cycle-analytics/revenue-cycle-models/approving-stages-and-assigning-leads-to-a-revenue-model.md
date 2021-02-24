---
unique-page-id: 4718683
description: Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos - Documentos de marketing - Documentación del producto
title: Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos {#approving-stages-and-assigning-leads-to-a-revenue-model}

Ponga en marcha el **Modelo de ingresos** agregando leads existentes, creando reglas de asignación para posibles clientes nuevos.

## Aprobación de etapas {#approving-stages}

Aprobemos las etapas del modelo antes de agregar posibles clientes.

1. Vaya al área **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Seleccione el modelo cuyas etapas desee aprobar.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. En **Acciones de modelo**, seleccione **Aprobar etapas**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Te recibirán con una alerta; haga clic en **Asignar leads**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

¡Excelente! Sigamos y asignemos esos leads.

## Asignación de leads existentes {#assigning-existing-leads}

[Cree una ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) lista inteligente para identificar los leads de una etapa del modelo en la base de datos de posibles clientes.

1. Una vez que haya [creado la Lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), haga clic en la ficha **Posibles clientes**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Haga clic en **Seleccionar todo** para seleccionar los leads.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Abra la lista desplegable **Acciones de posibles clientes** y seleccione **Especial**. Haga clic en **Cambiar etapa de ingresos**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Seleccione el **modelo** correcto y el **escenario** correcto. Haga clic en **Ejecutar ahora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Repita el proceso hasta que todos los leads se asignen a las distintas etapas del modelo.

¡bueno! Para especificar cómo se asignan nuevos leads a las fases, cree reglas de asignación.

>[!NOTE]
>
>Si el modelo está en el estado Fases aprobadas, no verá ningún evento de la etapa de cambio de ingresos en los registros de actividades de leads. Si el modelo está totalmente aprobado, este paso de flujo se omitirá si mueve un lead a la misma etapa en la que se encuentra actualmente.

## Nuevos leads: Crear reglas de asignación {#new-leads-create-assignment-rules}

1. Haga clic de nuevo en **Inicio de marketing** y seleccione **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Haga clic en el modelo en el árbol y, a continuación, en el menú **Acciones del modelo**, seleccione **Reglas de asignación**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Si las reglas de asignación contienen más de una opción predeterminada, haga clic en **Escenario**, realice la selección y haga clic en **Añadir opción**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Ejemplo de regla de asignación {#example-assignment-rule}

Cree una regla de Puntuación de posible cliente para asignar los nuevos leads con una puntuación mínima a un paso adecuado.

1. En **Si**, seleccione **Puntuación de posible cliente**. A continuación, elija **al menos**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Escriba **40** en el campo y seleccione **Líder de ventas** como una etapa. Haga clic en **Guardar** para completar.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Para aprobar su modelo, lea nuestra página de ayuda en **[Aprobación y desaprobación de un modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
