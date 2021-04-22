---
unique-page-id: 10094188
description: Aprobar un objeto personalizado - Documentos de Marketo - Documentación del producto
title: Aprobar un objeto personalizado
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Aprobar un objeto personalizado {#approve-a-custom-object}

Debe aprobar un objeto personalizado para poder utilizarlo. El proceso es ligeramente diferente para los nuevos objetos personalizados y los que ha editado.

## Aprobar un nuevo objeto personalizado {#approve-a-new-custom-object}

Ha creado un objeto personalizado completamente nuevo. Así es como aprobarlo.

1. En Administración, haga clic en **Marketo Custom Objects** y seleccione un objeto que esté en estado de borrador.

   ![](assets/one.png)

1. Haga clic en la lista desplegable **Acciones de objeto personalizado** y seleccione **Aprobar objeto**.

   ![](assets/two.png)

1. El estado cambia a Aprobado.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Un objeto personalizado utilizado en una estructura _uno a varios_ debe tener al menos un campo de deduplicación, un campo de vínculo, un nombre de objeto vinculado y un nombre de campo vinculado que se va a aprobar.
   >
   >Un objeto personalizado utilizado en una _estructura de varios a varios_ **no necesita** un campo de vínculo, un nombre de objeto vinculado o un nombre de campo vinculado al aprobarlo (ya que residen en el objeto intermedio).
   >
   >Un objeto personalizado utilizado como _objeto intermedio_ requiere un campo de vínculo, un nombre de objeto vinculado y un nombre de campo vinculado, pero **no** requiere un campo de deduplicación.
   >
   >Consulte [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obtener más información.

¡Eso es todo! Ahora, puede seleccionar el objeto personalizado en las restricciones de los filtros y déclencheur que desee utilizar en las campañas.

## Aprobar un objeto personalizado editado {#approve-an-edited-custom-object}

Después de editar un objeto personalizado aprobado, debe aprobar el borrador para devolver el objeto personalizado a un estado Aprobado.

1. Cuando edita un objeto personalizado ya aprobado, recibe un estado Approved with Draft .

   ![](assets/four.png)

1. Cuando esté listo para aprobar el borrador, haga clic en la lista desplegable **Acciones de objeto personalizado** y seleccione **Aprobar objeto**.

   ![](assets/five-1.png)

1. Una vista previa muestra los elementos que se han cambiado en el borrador. Haga clic en **Aprobar**.

   ![](assets/six-1.png)
