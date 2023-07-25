---
unique-page-id: 2360291
description: 'Bloquear actualizaciones de un campo: documentos de Marketo, documentación del producto'
title: Bloquear actualizaciones de un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Bloquear actualizaciones de un campo {#block-updates-to-a-field}

Bloquear las actualizaciones de un campo permite escribir en él una vez y, a continuación, conservar el valor original durante toda la duración del campo. Esto puede resultar útil para un campo como [!UICONTROL Origen de persona].

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/block-updates-to-a-field-1.png)

1. Clic **[!UICONTROL Administración de campos]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Busque el campo, selecciónelo y, a continuación, en **[!UICONTROL Acciones de campo]**, haga clic en **[!UICONTROL Bloquear actualizaciones de campos]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Puede bloquear las actualizaciones de [Campos personalizados de miembro de programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) y también.

1. Seleccione el **[!UICONTROL Fuentes de entrada]** desea bloquear y hacer clic en **[!UICONTROL Aplicar]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Al importar una lista, el estado de un campo que se está bloqueando en la vista previa de importación solo se mostrará si Marketo reconoce el campo automáticamente en función del nombre del campo que coincida _exacto_ (o si se han establecido alias). Si el campo se elige manualmente desde la lista desplegable Campo de Marketo, el estado de bloqueo no se muestra en la Vista previa de importación, pero se siguen implementando los bloqueos de actualización en ese campo.
