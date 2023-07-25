---
unique-page-id: 2360327
description: Asignación de particiones de persona con reglas de asignación - Documentos de Marketo - Documentación del producto
title: Asignación de Particiones de Personas con Reglas de Asignación
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Asignación de Particiones de Personas con Reglas de Asignación {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Permisos de administración necesarios**

>[!PREREQUISITES]
>
>[Crear una partición de persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Cuando utilice particiones de persona, configure reglas de asignación para enrutar a las personas creadas desde su CRM a sus particiones respectivas.

>[!NOTE]
>
>Solo las personas creadas en Marketo desde su CRM y mediante la API de SOAP tendrán reglas de asignación aplicadas.

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Clic **[!UICONTROL Espacios de trabajo y particiones]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. En el **[!UICONTROL Particiones de persona]** pestaña, haga clic en **[!UICONTROL Reglas de asignación]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Clic **[!UICONTROL Agregar opción]** para agregar condiciones para enrutar personas en particiones de persona.

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

1. Clic **[!UICONTROL Guardar]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

¡Y ahí lo tienen! ¡Ha asignado reglas para rellenar las particiones de persona con personas!

>[!NOTE]
>
>La opción predeterminada se aplica si no se cumple ninguna de las condiciones anteriores.
