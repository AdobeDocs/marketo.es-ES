---
unique-page-id: 10094188
description: Aprobar un objeto personalizado - Documentos de marketing - Documentación del producto
title: Aprobar un objeto personalizado
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Aprobar un objeto personalizado {#approve-a-custom-object}

Debe aprobar un objeto personalizado para poder utilizarlo. El proceso es ligeramente diferente para los nuevos objetos personalizados y los que ha editado.

## Aprobar un nuevo objeto personalizado {#approve-a-new-custom-object}

Ha creado un objeto personalizado completamente nuevo. Así es como aprobarlo.

1. En Administración, haga clic en **Marcar objetos personalizados** y seleccione un objeto que esté en estado Borrador.

   ![](assets/one.png)

1. Haga clic en la lista desplegable **Acciones de objeto personalizado** y seleccione **Aprobar objeto**.

   ![](assets/two.png)

1. El estado cambia a Aprobado.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Un objeto personalizado utilizado en una estructura _uno a varios_ debe tener al menos un campo de desduplicación, un campo de vínculo, un nombre de objeto vinculado y un nombre de campo vinculado para ser aprobado.
   >
   >Un objeto personalizado utilizado en una _estructura de varios a varios_ **no necesita** un campo de vínculo, un nombre de objeto vinculado o un nombre de campo vinculado al aprobarlo (porque residen en el objeto intermedio).
   >
   >Un objeto personalizado utilizado como _objeto intermediario_ requiere un campo de vínculo, un nombre de objeto vinculado y un nombre de campo vinculado, pero **no requiere** un campo de desduplicación.
   >
   >Consulte [Explicación de los objetos personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obtener más información.

¡Eso es todo! Ahora puede seleccionar el objeto personalizado con las restricciones de los filtros y déclencheur que desee utilizar en las campañas.

## Aprobar un objeto personalizado editado {#approve-an-edited-custom-object}

Después de editar un objeto personalizado aprobado, debe aprobar el borrador para devolver el objeto personalizado a un estado Aprobado.

1. Cuando edita un objeto personalizado ya aprobado, recibe un estado Aprobado con borrador.

   ![](assets/four.png)

1. Cuando esté listo para aprobar el borrador, haga clic en la lista desplegable **Acciones de objeto personalizado** y seleccione **Aprobar objeto**.

   ![](assets/five-1.png)

1. Una previsualización muestra los elementos que se cambiaron en el borrador. Haga clic en **Aprobar**.

   ![](assets/six-1.png)
