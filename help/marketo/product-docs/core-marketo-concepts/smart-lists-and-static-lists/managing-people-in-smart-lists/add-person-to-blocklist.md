---
unique-page-id: 9438139
description: 'Añadir persona a la Lista de bloqueados: documentos de Marketo, documentación del producto'
title: Añadir persona a la Lista de bloqueados
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Añadir persona a la Lista de bloqueados {#add-person-to-blocklist}

Agregar personas a la Lista de bloqueados impide que reciban la correspondencia.

>[!NOTE]
>
>Marketo está cambiando términos como Lista negra y Lista blanca por Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, es posible que vea los términos antiguos en nuestras capturas de pantalla de la interfaz de usuario y la documentación, y los nuevos términos en nuestro texto de documentación. Pedimos disculpas por cualquier confusión.

1. [Crear un nuevo programa predeterminado](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) y asígnele un nombre **Añadir a la Lista de bloqueados**.

1. Clic **Nuevo** y seleccione **Nuevo recurso local**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Asigne un nombre a la lista y haga clic en **Crear**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Agregar todas las personas a su **Lista inteligente** que desee añadir a su Lista de bloqueados.

   >[!NOTE]
   >
   >Las personas de su Lista de bloqueados no recibirán correos electrónicos operativos.

   ![](assets/three-6.png)

1. Clic **Nuevo** y seleccione **Nueva campaña inteligente**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Asigne un nombre al **Nueva campaña inteligente**. Haga clic en **Crear**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Arrastrar y soltar **Miembro de lista inteligente**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Seleccione la lista inteligente recién creada.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Arrastrar y soltar **Cambiar valor de datos**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Para el **Flujo**, introduzca **Bloquear enumerados** para el **Atributo** y establecer **Nuevo valor** hasta **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. En el **Programación** pestaña, seleccione **Ejecutar una vez**.

   ![](assets/ten.png)

1. Seleccionar **Ejecutar ahora** y haga clic en **Ejecutar**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   ¡SÍ! Estas personas ya no recibirán correos electrónicos.

   >[!TIP]
   >
   >Crear un [campaña inteligente de déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) usando **Cambiar valor de datos** con **Bloquear en la lista es verdadero** para todas las personas del futuro que tengan atributos que permitan la lista de bloqueados.
