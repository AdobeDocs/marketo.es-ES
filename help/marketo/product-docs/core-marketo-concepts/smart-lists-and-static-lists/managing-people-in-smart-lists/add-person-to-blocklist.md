---
unique-page-id: 9438139
description: 'Añadir persona a la Lista de bloqueados: documentos de Marketo, documentación del producto'
title: Añadir persona a la lista de bloqueados
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 5%

---

# Añadir persona a la lista de bloqueados {#add-person-to-blocklist}

Agregar personas a la Lista de bloqueados impide que reciban la correspondencia.

1. Cree un nuevo [programa predeterminado](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} y asígnele el nombre &quot;Agregar a Lista de bloqueados&quot;.

1. Haga clic en **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo recurso local]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Seleccione **[!UICONTROL Lista inteligente]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Asigne un nombre a la lista y haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Agregue todas las personas a la lista inteligente que desee agregar a la Lista de bloqueados.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Las personas de su Lista de bloqueados no recibirán correos electrónicos operativos.

1. Vuelva a su programa.

   ![](assets/add-person-to-blocklist-5.png)

1. Haga clic en **[!UICONTROL Nueva]** y seleccione **[!UICONTROL Nueva campaña inteligente]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Asigne un nombre a la nueva campaña inteligente. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Arrastre y suelte **[!UICONTROL Miembro de la lista inteligente]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Seleccione la lista inteligente que acaba de crear.

   ![](assets/add-person-to-blocklist-9.png)

1. Haga clic en la ficha **[!UICONTROL Flujo]**. Arrastre y suelte la acción de flujo **[!UICONTROL Cambiar valor de datos]**.

   ![](assets/add-person-to-blocklist-10.png)

1. En la lista desplegable **[!UICONTROL Atributo]**, seleccione **[!UICONTROL Bloquear incluido]** y establezca **[!UICONTROL Nuevo valor]** en **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Haga clic en la ficha **[!UICONTROL Programar]** y seleccione **[!UICONTROL Ejecutar una vez]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Seleccione **[!UICONTROL Ejecutar ahora]** y haga clic en **[!UICONTROL Ejecutar]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Vuelva a hacer clic en **[!UICONTROL Ejecutar]**.

   ![](assets/add-person-to-blocklist-14.png)

Estas personas ya no recibirán correos electrónicos.

>[!TIP]
>
>Crear una [campaña de Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} usando **Cambiar valor de datos** con **Bloquear en la lista es verdadero** para todas las personas en el futuro que tengan atributos para lista de bloqueados.
