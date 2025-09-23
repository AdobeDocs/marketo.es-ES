---
unique-page-id: 2360291
description: 'Bloquear actualizaciones de un campo: documentos de Marketo, documentación del producto'
title: Bloquear actualizaciones de un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 5%

---

# Bloquear actualizaciones de un campo {#block-updates-to-a-field}

Bloquear las actualizaciones de un campo permite escribir en él una vez y, a continuación, conservar el valor original durante toda la duración del campo. Esto puede resultar útil en un campo como [!UICONTROL Source de persona].

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Haga clic en **[!UICONTROL Administración de campos]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Busque el campo, selecciónelo y en **[!UICONTROL Acciones de campo]**, haga clic en **[!UICONTROL Bloquear actualizaciones de campo]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >También puede bloquear actualizaciones de [Campos personalizados de miembros del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Seleccione las **[!UICONTROL fuentes de entrada]** que desee bloquear y haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Al importar una lista, el estado de un campo bloqueado en la vista previa de importación solo se mostrará si Marketo lo reconoce automáticamente en función del nombre del campo que coincida con _exactamente_ (o si se han establecido alias). Si el campo se elige manualmente desde la lista desplegable Campo de Marketo, el estado de bloqueo no se muestra en la Vista previa de importación, pero se siguen implementando los bloqueos de actualización en ese campo.
