---
unique-page-id: 4719308
description: Añadir un campo de Salesforce existente a la sincronización de Marketo - Documentos de Marketo - Documentación del producto
title: Añadir un campo de Salesforce existente a la sincronización de Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Añadir un campo de Salesforce existente a la sincronización de Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Permisos de administración necesarios**

Normalmente, los nuevos campos personalizados de Salesforce se sincronizan automáticamente con Marketo Engage. Si no es así, es posible que los campos no sean visibles para el usuario de sincronización de Marketo. Así es como puedes arreglar esto.

1. Haga clic en su nombre y seleccione **[!UICONTROL Configurar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Introduzca &quot;perfil&quot; en la barra de búsqueda izquierda y haga clic en **[!UICONTROL Perfiles]** bajo **[!UICONTROL Administrar usuarios]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. En el **[!UICONTROL Seguridad de nivel de campo]** , haga clic en **[!UICONTROL Ver]** situado junto al objeto que contiene el campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Clic **[!UICONTROL Editar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Compruebe la **[!UICONTROL Visible]** para el campo que desea añadir a la sincronización y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   En el siguiente ciclo de sincronización, Marketo verá el campo e iniciará el proceso mágico.

   >[!NOTE]
   >
   > Si el campo ya tiene valores en Salesforce, esos valores no se sincronizan con Marketo hasta la siguiente actualización del registro.
