---
unique-page-id: 9438139
description: 'Agregar persona a Lista de bloqueados: Marketo Docs: documentación del producto'
title: Agregar persona a Lista de bloqueados
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Agregar persona a Lista de bloqueados {#add-person-to-blocklist}

Añadir personas a la Lista de bloqueados impide que reciban su correspondencia.

>[!NOTE]
>
>Marketo está cambiando términos como Lista negra y Lista blanca a Lista de bloqueados y Lista de permitidos en nuestro producto. Durante esta actualización, es posible que vea los términos antiguos en nuestra interfaz de usuario y en las capturas de pantalla de la documentación, así como los términos nuevos en nuestro texto de documentación. Pedimos disculpas por cualquier confusión.

1. [Crear un nuevo programa predeterminado](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) y asígnele un nombre **Agregar a Lista de bloqueados**.

1. Haga clic en **Nuevo** y seleccione **Nuevo recurso local**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Asigne un nombre a la lista y haga clic en **Crear**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Agregue todas las personas a su **Lista inteligente** desea añadirlo a su Lista de bloqueados.

   >[!NOTE]
   >
   >Las personas de la Lista de bloqueados no recibirán correos electrónicos operativos.

   ![](assets/three-6.png)

1. Haga clic en **Nuevo** y seleccione **Nueva campaña inteligente**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Asigne un nombre a la variable **Nueva campaña inteligente**. Haga clic en **Crear**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Arrastrar y soltar **Miembro de la lista inteligente**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Seleccione la lista inteligente que acaba de crear.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Arrastrar y soltar **Cambiar valor de datos**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Para la variable **Flujo**, introduzca **Bloque enumerado** para el **Atributo** y establezca **Nuevo valor** a **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. En el **Programación** , seleccione **Ejecutar una vez**.

   ![](assets/ten.png)

1. Select **Ejecutar ahora** y haga clic en **Ejecutar**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   ¡YAY! Estas personas ya no recibirán correos electrónicos.

   >[!TIP]
   >
   >Cree un [campaña inteligente de déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) using **Cambiar valor de datos** con **El bloque enumerado es verdadero** para todas las personas en el futuro que tengan atributos que permitan la lista de bloqueados.
