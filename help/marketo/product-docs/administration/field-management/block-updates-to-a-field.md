---
unique-page-id: 2360291
description: 'Bloquear actualizaciones en un campo: Documentos de Marketo: Documentación del producto'
title: Bloquear actualizaciones de un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Bloquear actualizaciones de un campo {#block-updates-to-a-field}

Bloquear actualizaciones en un campo le permite escribir en él una vez y, a continuación, conservar el valor original durante toda la vida del campo. Esto puede resultar útil para un campo como Fuente de persona.

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Vaya a **Admin** y haga clic en **Administración de campos**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Busque el campo, selecciónelo y, a continuación, en **Acciones de campo**, haga clic en **Bloquear actualizaciones de campo**.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >También puede bloquear actualizaciones en [Campos personalizados de miembro del programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Seleccione las **Fuentes de entrada** que desee bloquear y haga clic en **Aplicar**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Al realizar una importación de lista, el estado de un campo bloqueado en la vista previa de importación solo se mostrará si Marketo reconoce automáticamente el campo en función del nombre del campo que coincida con _exactamente_ (o si se han establecido alias). Si el campo se elige manualmente en la lista desplegable Campo Marketo , el estado bloqueado no se mostrará en la vista previa de importación, pero el bloqueo de actualización a ese campo seguirá implementándose.
