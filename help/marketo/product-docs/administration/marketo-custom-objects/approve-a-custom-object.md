---
unique-page-id: 10094188
description: Cómo aprobar objetos personalizados nuevos o editados en Administración, incluidos los requisitos para objetos "uno a varios", "varios a varios" e intermediarios.
title: Aprobar un objeto personalizable
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 40d7e8a0723946970c49a6dfc4f0de4c71b0df65
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 2%

---

# Aprobar un objeto personalizable {#approve-a-custom-object}

Debe aprobar un objeto personalizado para poder utilizarlo. El proceso es ligeramente diferente para los nuevos objetos personalizados y los que ha editado.

## Aprobar un nuevo objeto personalizado {#approve-a-new-custom-object}

Se ha creado un nuevo objeto personalizado. Siga los pasos a continuación para aprobarla.

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/approve-a-custom-object-1.png)

1. Haga clic en **[!UICONTROL Objetos personalizados de Marketo]**.

   ![](assets/approve-a-custom-object-2.png)

1. Seleccione un objeto que esté en estado Borrador.

   ![](assets/approve-a-custom-object-3.png)

1. Haga clic en el menú desplegable **[!UICONTROL Acciones de objeto personalizadas]** y seleccione **[!UICONTROL Aprobar objeto]**.

   ![](assets/approve-a-custom-object-4.png)

1. El estado cambia a [!UICONTROL Aprobado].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Un objeto personalizado utilizado en una _estructura &quot;uno a varios&quot;_ debe tener al menos un campo desduplicado, un campo de vínculo, un nombre de objeto vinculado y un nombre de campo vinculado para ser aprobado.
   >
   >Un objeto personalizado utilizado en una estructura _varios a varios_ **no** necesita un campo de vínculo, un nombre de objeto vinculado o un nombre de campo vinculado cuando lo aprueba (ya que residen en el objeto intermedio).
   >
   >Un objeto personalizado utilizado como _objeto intermedio_ requiere un campo de vínculo, un nombre de objeto vinculado y un nombre de campo vinculado, pero **no** requiere un campo desduplicado.
   >
   >Consulte [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obtener más información.

Ahora puede seleccionar el objeto personalizado dentro de las restricciones de los filtros y déclencheur para utilizarlo en sus campañas.

## Aprobar un objeto personalizado editado {#approve-an-edited-custom-object}

Después de editar un objeto personalizado aprobado, debe aprobar el borrador para devolver el objeto personalizado a un estado Aprobado.

1. Cuando edita un objeto personalizado ya aprobado, recibe un estado [!UICONTROL Aprobado con Borrador].

   ![](assets/approve-a-custom-object-6.png)

1. Cuando esté listo para aprobar el borrador, haga clic en la lista desplegable **[!UICONTROL Acciones de objeto personalizadas]** y seleccione **[!UICONTROL Aprobar objeto]**.

   ![](assets/approve-a-custom-object-7.png)

1. Una vista previa muestra los elementos modificados en el borrador. Haga clic en **[!UICONTROL Aprobar]**.

   ![](assets/approve-a-custom-object-8.png)
