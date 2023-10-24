---
unique-page-id: 9438139
description: 'Añadir persona a la Lista de bloqueados: documentos de Marketo, documentación del producto'
title: Añadir persona a la Lista de bloqueados
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Añadir persona a la Lista de bloqueados {#add-person-to-blocklist}

Agregar personas a la Lista de bloqueados impide que reciban la correspondencia.

1. Crear un nuevo [programa predeterminado](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} y asígnele el nombre &quot;Agregar a Lista de bloqueados&quot;.

1. Clic **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nuevo recurso local]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Seleccionar **[!UICONTROL Lista inteligente]**.

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

1. Clic **[!UICONTROL Nuevo]** y seleccione **[!UICONTROL Nueva campaña inteligente]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Asigne un nombre a la nueva campaña inteligente. Haga clic en **[!UICONTROL Crear]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Arrastrar y soltar **[!UICONTROL Miembro de lista inteligente]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Seleccione la lista inteligente que acaba de crear.

   ![](assets/add-person-to-blocklist-9.png)

1. Haga clic en **[!UICONTROL Flujo]** pestaña. Arrastre y suelte el **[!UICONTROL Cambiar valor de datos]** Acción de flujo.

   ![](assets/add-person-to-blocklist-10.png)

1. En el **[!UICONTROL Atributo]** selección desplegable **[!UICONTROL Bloquear enumerados]** y establecer **[!UICONTROL Nuevo valor]** hasta **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Haga clic en **[!UICONTROL Programación]** y seleccione **[!UICONTROL Ejecutar una vez]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Seleccionar **[!UICONTROL Ejecutar ahora]** y haga clic en **[!UICONTROL Ejecutar]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Clic **[!UICONTROL Ejecutar]** otra vez.

   ![](assets/add-person-to-blocklist-14.png)

Estas personas ya no recibirán correos electrónicos.

>[!TIP]
>
>Crear un [Campaña de déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} usando **Cambiar valor de datos** con **Bloquear en la lista es verdadero** para todas las personas del futuro que tengan atributos que permitan la lista de bloqueados.
