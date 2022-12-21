---
unique-page-id: 10095644
description: 'Aprobar un fragmento sin borrador: documentos de Marketo: documentación del producto'
title: Aprobar un fragmento sin borrador
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Aprobar un fragmento sin borrador {#approve-a-snippet-with-no-draft}

## Aprobar el fragmento {#approve-the-snippet}

No se activa el borrador cada vez que se aprueba un fragmento. Esto incluye un fragmento compartido o al que los recursos hacen referencia en otros espacios de trabajo.

1. Vaya a **Design Studio**.

   ![](assets/go-to-design-studio.png)

1. Seleccione un fragmento y, en el **Acciones de fragmento** , elija **Aprobar**.

   ![](assets/approve-snippet.png)

1. Seleccione una opción en el cuadro de diálogo Aprobar fragmento y haga clic en **Aprobar**:

   * **Actualizar todo**: Esta opción no crea borradores de los recursos aprobados con el fragmento. Todos los recursos reciben las actualizaciones y mantienen sus estados anteriores. Aparece un módulo de progreso en la parte superior derecha de la pantalla; se puede cerrar en cualquier momento. Para restaurarla, haga clic con el botón derecho en el nombre del fragmento y seleccione Mostrar estado de aprobación.
   * **Crear borradores**: Esta opción crea borradores de los recursos aprobados utilizando el fragmento . Seleccione esta opción si los cambios de fragmento deben revisarse primero. Todos los borradores deben aprobarse manualmente.

   ![](assets/snippet-dialog-box.png)

   >[!NOTE]
   >
   >Para un nuevo fragmento que aún no se haya utilizado, no aparece esta pantalla Aprobar borrador . Se muestra cuando el fragmento se utiliza en uno o varios recursos.

>[!CAUTION]
>
>Esta función está diseñada para ahorrar tiempo con el flujo de trabajo de aprobación de fragmentos. Sin embargo, hay algunas limitaciones que hay que tener en cuenta. Consulte [este documento](https://nation.marketo.com/docs/DOC-4415) para obtener más información. El documento también contiene información sobre la gestión de errores y la solución de problemas.

>[!MORELIKETHIS]
>
>[Activar sin borrador para fragmentos](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md)
