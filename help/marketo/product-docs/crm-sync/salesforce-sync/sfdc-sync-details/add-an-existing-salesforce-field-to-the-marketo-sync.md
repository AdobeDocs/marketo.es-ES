---
unique-page-id: 4719308
description: Agregar un campo de Salesforce existente a la sincronización de Marketo - Marketo Docs - Documentación del producto
title: Agregar un campo de Salesforce existente a la sincronización de Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 81bc90bcccc8073511c9f331471c0cda9f4147cb
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Agregar un campo de Salesforce existente a la sincronización de Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Normalmente, los nuevos campos personalizados de Salesforce se sincronizan automáticamente con Marketo. Si no es así, es posible que el usuario de Marketo Sync no pueda ver los campos. Así es como se puede arreglar esto.

1. Haga clic en su nombre y, a continuación, seleccione **Configuración**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Entrar **perfil** en la barra de búsqueda izquierda y haga clic en **Perfiles** under **Administrar usuarios**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. En el **Seguridad a nivel de campo** , haga clic en **Ver** junto al objeto que contiene el campo .

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Haga clic en **Editar**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Marque la **Visible** casilla del campo que desea agregar a la sincronización y haga clic en **Guardar**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   ¡Dulce! En el siguiente ciclo de sincronización, Marketo verá el campo e iniciará la magia.

   >[!NOTE]
   >
   > Si el campo ya tiene valores en Salesforce, esos valores no se sincronizan con Marketo hasta la siguiente actualización del registro.
