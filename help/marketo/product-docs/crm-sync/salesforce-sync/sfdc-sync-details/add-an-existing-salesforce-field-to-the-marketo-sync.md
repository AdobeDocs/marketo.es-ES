---
unique-page-id: 4719308
description: Aprenda a añadir un campo de Salesforce existente a la sincronización de Marketo. Hacer que el campo sea visible para el usuario de sincronización en Salesforce para que se sincronice en el siguiente ciclo.
title: Añadir un campo de Salesforce existente a la sincronización de Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/Vb-1DhNwUPQSPYuCkVzzSDDqWd4tvO-XoPhXn58hj6E'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 8%
---
# Agregar un campo [!DNL Salesforce] existente a la sincronización de Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Normalmente, los nuevos campos personalizados de Salesforce se sincronizan automáticamente con Marketo Engage. Si no es así, es posible que los campos no sean visibles para el usuario de sincronización de Marketo. Así es como puedes arreglar esto.

1. Haz clic en tu nombre y selecciona **[!UICONTROL Configuración]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Escriba &quot;perfil&quot; en la barra de búsqueda izquierda y haga clic en **[!UICONTROL Perfiles]** en **[!UICONTROL Administrar usuarios]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. En la sección **[!UICONTROL Seguridad de nivel de campo]**, haga clic en **[!UICONTROL Ver]** junto al objeto que contiene el campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Haga clic en **[!UICONTROL Editar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Marque la casilla de verificación **[!UICONTROL Visible]** del campo que desee agregar a la sincronización y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   En el siguiente ciclo de sincronización, Marketo verá el campo e iniciará el proceso mágico.

   >[!NOTE]
   >
   > Si el campo ya tiene valores en [!DNL Salesforce], esos valores no se sincronizan con Marketo hasta la siguiente actualización del registro.
