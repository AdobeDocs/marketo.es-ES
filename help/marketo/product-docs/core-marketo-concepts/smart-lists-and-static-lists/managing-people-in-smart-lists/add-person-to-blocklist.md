---
unique-page-id: 9438139
description: Añadir persona a Lista de bloqueados - Documentos de marketing - Documentación del producto
title: Añadir persona a Lista de bloqueados
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Añadir persona a Lista de bloqueados {#add-person-to-blocklist}

Añadir personas a tu Lista de bloqueados impide que reciban tu correspondencia.

>[!NOTE]
>
>Marketing está en proceso de cambiar términos como Lista negra y Lista blanca a Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, puede ver los términos antiguos en nuestra interfaz de usuario y en las capturas de pantalla de documentación, así como los nuevos términos en el texto de la documentación. Pedimos disculpas por cualquier confusión.

1. [Cree un nuevo programa](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) predeterminado y asígnele un nombre que **Añada a la Lista de bloqueados**.
1. Haga clic en **Nuevo** y seleccione **Nuevo recurso** local.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Asigne un nombre a la lista y haga clic en **Crear**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Añada todas las personas a la Lista **** inteligente que desee agregar a la Lista de bloqueados.

   >[!NOTE]
   >
   >Las personas de su Lista de bloqueados no recibirán correos electrónicos operativos.

   ![](assets/three-6.png)

1. Haga clic en **Nuevo** y seleccione **Nueva Campaña** inteligente.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Asigne un nombre a la **nueva Campaña** inteligente. Haga clic en **Crear**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Arrastre y suelte **Miembro de Lista** inteligente.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Seleccione la lista inteligente que acaba de crear.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Arrastre y suelte **Cambiar valor** de datos.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Para el **flujo**, introduzca **Bloque enumerado** para el **atributo** y defina **Nuevo valor** en **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. En la ficha **Programar** , seleccione **Ejecutar una vez**.

   ![](assets/ten.png)

1. Seleccione **Ejecutar ahora** y haga clic en **Ejecutar**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   ¡YAY! Estas personas ya no recibirán correos electrónicos.

   >[!TIP]
   >
   >Crear una campaña [inteligente de](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) activación mediante **Cambiar valor** de datos con **bloque enumerado es verdadero** para todas las personas en el futuro que tengan atributos que permitan la lista de bloqueados.

