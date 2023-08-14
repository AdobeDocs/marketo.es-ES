---
unique-page-id: 9438139
description: 'Añadir persona a la Lista de bloqueados: documentos de Marketo, documentación del producto'
title: Añadir persona a la Lista de bloqueados
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# Añadir persona a la Lista de bloqueados {#add-person-to-blocklist}

Agregar personas a la Lista de bloqueados impide que reciban la correspondencia.

1. [Crear un nuevo programa predeterminado](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) y asígnele un nombre **Añadir a la Lista de bloqueados**.

1. Clic **Nuevo** y seleccione **Nuevo recurso local**.

   ![](assets/add-person-to-blocklist-1.png)

1. Seleccionar **Lista inteligente**.

   ![](assets/add-person-to-blocklist-2.png)

1. Asigne un nombre a la lista y haga clic en **Crear**.

   ![](assets/add-person-to-blocklist-3.png)

1. Agregar todas las personas a su **Lista inteligente** que desee añadir a su Lista de bloqueados.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Las personas de su Lista de bloqueados no recibirán correos electrónicos operativos.

1. Vuelva a su programa.

   ![](assets/add-person-to-blocklist-5.png)

1. Clic **Nuevo** y seleccione **Nueva campaña inteligente**.

   ![](assets/add-person-to-blocklist-6.png)

1. Asigne un nombre al **Nueva campaña inteligente**. Haga clic en **Crear**.

   ![](assets/add-person-to-blocklist-7.png)

1. Arrastrar y soltar **Miembro de lista inteligente**.

   ![](assets/add-person-to-blocklist-8.png)

1. Seleccione la lista inteligente recién creada.

   ![](assets/add-person-to-blocklist-9.png)

1. Haga clic en **Flujo** pestaña. Arrastre y suelte el **Cambiar valor de datos** Acción de flujo.

   ![](assets/add-person-to-blocklist-10.png)

1. En el **Atributo** selección desplegable **Bloquear enumerados** y establecer **Nuevo valor** hasta **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. Haga clic en **Programación** y seleccione **Ejecutar una vez**.

   ![](assets/add-person-to-blocklist-12.png)

1. Seleccionar **Ejecutar ahora** y haga clic en **Ejecutar**.

   ![](assets/add-person-to-blocklist-13.png)

1. Clic **Ejecutar** otra vez.

   ![](assets/add-person-to-blocklist-14.png)

Estas personas ya no recibirán correos electrónicos.

>[!TIP]
>
>Crear un [campaña inteligente de déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) usando **Cambiar valor de datos** con **Bloquear en la lista es verdadero** para todas las personas del futuro que tengan atributos que permitan la lista de bloqueados.
