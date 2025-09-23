---
unique-page-id: 2360327
description: Asignación de particiones de persona con reglas de asignación - Documentos de Marketo - Documentación del producto
title: Asignación de particiones de personas con reglas de asignación
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 8%

---

# Asignación de particiones de personas con reglas de asignación {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Se requieren permisos de administración**

>[!PREREQUISITES]
>
>[Crear una partición de persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Cuando utilice particiones de persona, configure reglas de asignación para enrutar a las personas creadas desde su CRM a sus particiones respectivas.

>[!NOTE]
>
>Solo las personas creadas en Marketo desde su CRM y mediante la API de SOAP tendrán reglas de asignación aplicadas.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Haga clic en **[!UICONTROL Espacios de trabajo y particiones]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. En la ficha **[!UICONTROL Particiones de persona]**, haga clic en **[!UICONTROL Reglas de asignación]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Haga clic en **[!UICONTROL Agregar opción]** para agregar condiciones para enrutar personas a particiones de persona.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Seleccione el campo en el que se debe crear la condición.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Seleccione el operador de opción e introduzca un valor.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Seleccione la partición de personas en la que desea que caigan las personas que cumplan las condiciones.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Puede agregar tantas opciones como desee.

1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

¡Y ahí lo tienen! ¡Ha asignado reglas para rellenar las particiones de persona con personas!

>[!NOTE]
>
>La opción predeterminada se aplica si no se cumple ninguna de las condiciones anteriores.
