---
unique-page-id: 4719287
description: Editar asignaciones iniciales de campos - Documentos de marketing - Documentación del producto
title: Editar asignaciones iniciales de campos
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Editar asignaciones iniciales de campos {#edit-initial-field-mappings}

>[!NOTE]
>
>**Recordatorio**
>
>A esta función solo se puede acceder antes de la sincronización inicial con Salesforce. Una vez presionado el botón **Sincronizar ahora** , ya no se puede hacer.

Durante la sincronización inicial con Salesforce, Marketo combina automáticamente campos personalizados con nombres similares en un único campo del lado de Marketing para garantizar que los datos se puedan intercambiar con los objetos Posible cliente y Contacto en CRM. En este artículo se explica cómo personalizar estas asignaciones.

## Asignar campos no asignados {#map-unmapped-fields}

Cuando ve un campo en la carpeta Campos sin asignar, significa que no está asignado a un campo similar en el posible cliente o contacto de Salesforce. Puedes arreglar eso.

1. Haga clic en Editar asignaciones.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Abra la carpeta Campos **personalizados** sin asignar.

   ![](assets/two.png)

1. Arrastre un campo personalizado sin asignar a otro para asignarlos juntos.

   >[!NOTE]
   >
   >Solo puede editar asignaciones de campo personalizadas. No se pueden modificar las asignaciones de campo estándar.

   ![](assets/three.png)

1. Haga clic en **Finalizar asignaciones** cuando haya terminado.

   ![](assets/four.png)

## Desglose de la asignación existente {#break-existing-mapping}

Si tiene campos con nombres similares en el lead y el objeto de contacto Marketing los asignará automáticamente. Puede considerar que son diferentes y que contienen datos diferentes. Rompa la asignación de esta manera.

1. Haga clic en **Editar asignaciones**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Resalte un campo asignado y haga clic en **Dividir asignación** para separar los campos.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Haga clic en **Finalizar asignaciones** cuando haya terminado.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   ¡Bonito! Ya casi has terminado con la sincronización inicial.

## Restablecer Esquema {#reset-schema}

1. Si realiza algunos cambios en el esquema en Salesforce mientras trabaja en las asignaciones, puede extraer los cambios haciendo clic en **Restablecer Esquema**.

   * Se restablecerán todos los cambios de asignación.
   * Restablecer el esquema solo agregará campos, no se eliminará (aunque los oculte del usuario de sincronización).

   ![](assets/image2014-12-9-13-3a32-3a8.png)

