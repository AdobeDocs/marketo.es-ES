---
unique-page-id: 10095644
description: 'Aprobar un fragmento sin borrador: documentos de Marketo, documentación del producto'
title: Aprobar un fragmento sin borrador
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
feature: Snippets
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Aprobar un fragmento sin borrador {#approve-a-snippet-with-no-draft}

## Aprobar el fragmento {#approve-the-snippet}

La opción Sin borrador se activa cada vez que se aprueba un fragmento. Esto incluye un fragmento de código compartido o referenciado por recursos de otros espacios de trabajo.

1. Ir a **Design Studio**.

   ![](assets/go-to-design-studio.png)

1. Seleccione un fragmento de código y, en **Acciones de fragmento** menú desplegable, elija **Aprobar**.

   ![](assets/approve-snippet.png)

1. Seleccione una opción en el cuadro de diálogo Aprobar fragmento y haga clic en **Aprobar**:

   * **Actualizar todo**: Esta opción no creará borradores de los recursos aprobados mediante el fragmento. Todos los recursos reciben las actualizaciones y mantienen sus estados anteriores. Aparece un módulo de progreso en la parte superior derecha de la pantalla; se puede cerrar en cualquier momento. Para restaurarlo, haga clic con el botón derecho en el nombre del fragmento y seleccione Mostrar estado de aprobación.
   * **Crear borradores**: Esta opción creará borradores de los recursos aprobados utilizando el fragmento. Seleccione esta opción si primero deben revisarse los cambios de fragmento. Todos los borradores deben aprobarse manualmente.

   ![](assets/snippet-dialog-box.png)

   >[!NOTE]
   >
   >Para un nuevo fragmento de código que aún no se ha utilizado, esta pantalla Aprobar borrador no aparece. Se muestra cuando el fragmento se utiliza en uno o varios recursos.

>[!CAUTION]
>
>Esta función está diseñada para ahorrar tiempo con el flujo de trabajo de aprobación de fragmentos. Sin embargo, hay que tener en cuenta algunas limitaciones. Consulte lo siguiente [este documento](https://nation.marketo.com/docs/DOC-4415) para obtener más información. El documento también contiene información sobre la gestión de errores y la resolución de problemas.

>[!MORELIKETHIS]
>
>[Habilitar la opción Sin borrador para fragmentos](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md)
