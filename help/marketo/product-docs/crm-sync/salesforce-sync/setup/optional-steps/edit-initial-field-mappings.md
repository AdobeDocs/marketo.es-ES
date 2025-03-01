---
unique-page-id: 4719287
description: 'Editar asignaciones de campo iniciales: documentos de Marketo: documentación del producto'
title: Editar asignaciones de campo iniciales
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Editar asignaciones de campo iniciales {#edit-initial-field-mappings}

>[!NOTE]
>
>Solo se puede acceder a esta función antes de la sincronización inicial con Salesforce. Una vez que pulse el botón **[!UICONTROL Sincronizar ahora]**, ya no podrá hacerlo.

Durante la sincronización inicial con Salesforce, Marketo Engage combina automáticamente campos personalizados con nombres similares en un único campo del lado de Marketo para garantizar que los datos se puedan intercambiar con los objetos de posible cliente y contacto en CRM. Este artículo explica cómo personalizar estas asignaciones.

## Asignar campos no asignados {#map-unmapped-fields}

Cuando ve un campo en la carpeta [!UICONTROL Campos no asignados], significa que no está asignado a un campo similar del posible cliente o contacto en Salesforce. Puedes arreglar eso.

1. Haga clic en **[!UICONTROL Editar asignaciones]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Abra la carpeta **[!UICONTROL Campos personalizados sin asignar]**.

   ![](assets/two.png)

1. Arrastre un campo personalizado sin asignar a otro para asignarlo juntos.

   >[!NOTE]
   >
   >Solo puede editar asignaciones de campos personalizados. No se pueden modificar las asignaciones de campo estándar.

   ![](assets/three.png)

1. Haga clic en **[!UICONTROL Finalizar asignaciones]** cuando haya terminado.

   ![](assets/four.png)

## Romper asignación existente {#break-existing-mapping}

Si tiene campos con nombres similares en el posible cliente y en el objeto de contacto, Marketo los asignará automáticamente. Puede considerar que son diferentes y que contienen datos diferentes. Rompa la asignación de esta manera.

1. Haga clic en **[!UICONTROL Editar asignaciones]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Resalte un campo asignado y haga clic en **[!UICONTROL Romper asignación]** para separar los campos.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Haga clic en **[!UICONTROL Finalizar asignaciones]** cuando haya terminado.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   ¡Bonito! Casi has terminado con la sincronización inicial.

## Restablecer esquema {#reset-schema}

1. Si realiza algunos cambios en el esquema de Salesforce mientras trabaja en las asignaciones, puede extraer los cambios haciendo clic en **[!UICONTROL Restablecer esquema]**.

   * Se restablecerán todos los cambios de asignación.
   * Al restablecer el esquema, solo se añaden campos, no se eliminan (aunque se oculten al usuario de sincronización).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
