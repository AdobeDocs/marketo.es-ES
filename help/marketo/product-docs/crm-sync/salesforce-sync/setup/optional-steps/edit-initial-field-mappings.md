---
unique-page-id: 4719287
description: Editar asignaciones de campos iniciales - Documentos de Marketo - Documentación del producto
title: Editar asignaciones de campo iniciales
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Editar asignaciones de campo iniciales {#edit-initial-field-mappings}

>[!NOTE]
>
>Solo se puede acceder a esta función antes de la sincronización inicial con Salesforce. Una vez presionado el botón **Sincronizar ahora**, ya no se puede hacer.

Durante la sincronización inicial con Salesforce, Marketo combina automáticamente campos personalizados con nombres similares en un único campo del lado de Marketo para garantizar que los datos se puedan intercambiar con los objetos posible cliente y Contacto en CRM. Este artículo explica cómo personalizar estas asignaciones.

## Asignar campos no asignados {#map-unmapped-fields}

Cuando ve un campo en la carpeta Campos sin asignar, significa que no está asignado a un campo similar en el posible cliente o contacto de Salesforce. Puedes arreglar eso.

1. Haga clic en **Editar asignaciones**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Abra la carpeta **Campos personalizados sin asignar**.

   ![](assets/two.png)

1. Arrastre un campo personalizado sin asignar a otro para asignarlos juntos.

   >[!NOTE]
   >
   >Solo puede editar asignaciones de campos personalizados. Las asignaciones de campos estándar no se pueden modificar.

   ![](assets/three.png)

1. Haga clic en **Finalizar asignaciones** cuando haya terminado.

   ![](assets/four.png)

## Romper la asignación existente {#break-existing-mapping}

Si tiene campos con nombres similares en el posible cliente y el objeto de contacto Marketo los asignará juntos automáticamente. Puede considerar que son diferentes y que contienen datos diferentes. Rompa la asignación de esta manera.

1. Haga clic en **Editar asignaciones**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Resalte un campo asignado y haga clic en **Break Mapping** para separar los campos.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Haga clic en **Finalizar asignaciones** cuando haya terminado.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   ¡Muy bien! Casi terminas con la sincronización inicial.

## Restablecer esquema {#reset-schema}

1. Si realiza algunos cambios en el esquema en Salesforce mientras trabaja en las asignaciones, puede extraer los cambios haciendo clic en **Restaurar esquema**.

   * ¡Se restablecerán todos los cambios de asignación!
   * Restablecer el esquema solo agregará campos, no se eliminará (aunque los oculte del usuario de sincronización).
   ![](assets/image2014-12-9-13-3a32-3a8.png)
