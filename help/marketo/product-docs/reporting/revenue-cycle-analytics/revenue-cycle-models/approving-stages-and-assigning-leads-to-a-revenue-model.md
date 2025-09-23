---
unique-page-id: 4718683
description: Aprobación de etapas y asignación de posibles clientes a un modelo de ingresos - Documentos de Marketo - Documentación del producto
title: Aprobación de fases y asignación de posibles clientes a un modelo de ingresos
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 5%

---

# Aprobación de fases y asignación de posibles clientes a un modelo de ingresos {#approving-stages-and-assigning-leads-to-a-revenue-model}

Ponga en marcha su **Modelo de ingresos** agregando posibles clientes existentes y creando reglas de asignación para nuevos posibles clientes.

## Aprobando etapas {#approving-stages}

Vamos a aprobar las etapas del modelo antes de agregar cualquier posible cliente.

1. Vaya al área de **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Seleccione el modelo cuyas fases desee aprobar.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. En **[!UICONTROL Acciones de modelo]**, seleccione **[!UICONTROL Aprobar etapas]**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Se le enviará una alerta; haga clic en **[!UICONTROL Asignar posibles clientes]**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

¡Excelente! Vamos a seguir adelante y asignar esos posibles clientes.

## Asignación de posibles clientes existentes {#assigning-existing-leads}

[Cree una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para identificar los posibles clientes de una etapa del modelo en la base de datos de posibles clientes.

1. Una vez que hayas [creado tu lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), haz clic en la ficha **[!UICONTROL Posibles clientes]**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Haga clic en **[!UICONTROL Seleccionar todo]** para seleccionar los posibles clientes.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Abra la lista desplegable **[!UICONTROL Acciones de posible cliente]** y seleccione **[!UICONTROL Especial]**. Haga clic en **[!UICONTROL Cambiar etapa de ingresos...]**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Seleccione el **[!UICONTROL Modelo]** correcto y el **[!UICONTROL Escenario]** correcto. Haga clic en **[!UICONTROL Ejecutar ahora]**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Repita el proceso hasta que todos los posibles clientes se asignen a las distintas fases del modelo.

¡Excelente! Para especificar cómo se asignan los nuevos posibles clientes a las fases, cree reglas de asignación.

>[!NOTE]
>
>Si el modelo está en el estado Etapas aprobadas, no verá ningún evento de etapa de ingresos de cambio en los registros de actividad de los posibles clientes. Si el modelo está totalmente aprobado, este paso de flujo se omitirá si mueve un posible cliente al mismo escenario en el que se encuentra actualmente.

## Nuevos posibles clientes: Crear reglas de asignación  {#new-leads-create-assignment-rules}

1. Vuelva a hacer clic en **Inicio de Marketo** y, a continuación, seleccione **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Haga clic en el modelo en el árbol, luego en el menú **[!UICONTROL Acciones de modelo]** y seleccione **[!UICONTROL Reglas de asignación]**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Si las reglas de asignación contienen más de una opción predeterminada, haga clic en **[!UICONTROL Fase]**, realice la selección y luego haga clic en **[!UICONTROL Agregar opción]**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Ejemplo de regla de asignación {#example-assignment-rule}

Cree una regla de [!UICONTROL puntuación del posible cliente] para asignar los nuevos posibles clientes con una puntuación mínima a un paso apropiado.

1. En **[!UICONTROL Si]**, seleccione **[!UICONTROL Puntuación de posible cliente]**. Entonces elige **[!UICONTROL al menos]**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Escriba **40** en el campo y seleccione **[!UICONTROL Posible cliente de ventas]** como [!UICONTROL escenario]. Haga clic en **[!UICONTROL Guardar]** para completar la acción.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Para aprobar el modelo, lea nuestra página de ayuda sobre **[Aprobación y desaprobación de un modelo de ingresos](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
