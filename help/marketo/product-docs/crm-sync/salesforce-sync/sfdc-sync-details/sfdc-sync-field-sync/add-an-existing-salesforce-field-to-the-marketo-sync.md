---
unique-page-id: 4719308
description: Agregar un campo de Salesforce existente a la sincronización de Marketo - Marketo Docs - Documentación del producto
title: Agregar un campo de Salesforce existente a la sincronización de Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Agregar un campo de Salesforce existente a la sincronización de Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administrador**

Normalmente, los nuevos campos personalizados de Salesforce se sincronizan automáticamente con Marketo. Si no es así, es posible que el usuario de Marketo Sync no pueda ver los campos. Así es como se puede arreglar esto.

1. Haga clic en su nombre y, a continuación, seleccione **Setup**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Introduzca **profile** en la barra de búsqueda izquierda y haga clic en **Profiles** en **Administrar usuarios**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. En la sección **Field-Level Security**, haga clic en **View** junto al objeto que contiene el campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Haga clic en **Editar**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Marque la casilla **Visible** para el campo que desee agregar a la sincronización y haga clic en **Guardar**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   ¡Dulce! En el siguiente ciclo de sincronización, Marketo verá el campo e iniciará la magia.

   >[!NOTE]
   >
   > Si el campo ya tiene valores en Salesforce, esos valores no se sincronizan con Marketo hasta la siguiente actualización del registro.
