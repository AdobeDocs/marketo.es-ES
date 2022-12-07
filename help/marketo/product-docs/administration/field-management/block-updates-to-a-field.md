---
unique-page-id: 2360291
description: 'Bloquear actualizaciones en un campo: Documentos de Marketo: Documentación del producto'
title: Bloquear actualizaciones de un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Bloquear actualizaciones de un campo {#block-updates-to-a-field}

Bloquear actualizaciones en un campo le permite escribir en él una vez y, a continuación, conservar el valor original durante toda la vida del campo. Esto puede resultar útil para un campo como Fuente de persona.

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Vaya a la **Administrador** .

   ![](assets/block-updates-to-a-field-1.png)

1. Haga clic en **Gestión de las actividades sobre el terreno**.

   ![](assets/block-updates-to-a-field-2.png)

1. Busque el campo , selecciónelo y, a continuación, debajo de **Acciones de campo**, haga clic en **Bloquear actualizaciones de campos**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Puede bloquear las actualizaciones a [Campos personalizados de miembro del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) también.

1. Seleccione el **Fuentes de entrada** desea bloquear y hacer clic en **Aplicar**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Al realizar una importación de lista, el estado de un campo bloqueado en la vista previa de importación solo se mostrará si Marketo reconoce automáticamente el campo en función del nombre del campo que coincida _Exactamente_ (o si se establecen alias). Si el campo se elige manualmente en la lista desplegable Campo Marketo , el estado bloqueado no se mostrará en la vista previa de importación, pero el bloqueo de actualización a ese campo seguirá implementándose.
