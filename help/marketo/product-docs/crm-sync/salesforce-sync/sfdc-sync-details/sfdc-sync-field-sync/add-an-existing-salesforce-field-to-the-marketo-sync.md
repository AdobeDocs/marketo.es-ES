---
unique-page-id: 4719308
description: Añadir un campo de Salesforce existente en la sincronización de marketing - Documentos de marketing - Documentación del producto
title: Añadir un campo de Salesforce existente en la sincronización de marketing
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Añadir un campo de Salesforce existente en la sincronización de marketing {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Se requieren permisos de administración**

Normalmente, los nuevos campos personalizados de Salesforce se sincronizan automáticamente con Marketing. De lo contrario, es posible que los campos no estén visibles para el usuario de sincronización de marketing. Así es como puedes arreglar esto.

1. Haga clic en su nombre y, a continuación, seleccione **Ajustes**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Introduzca el **perfil** en la barra de búsqueda izquierda y haga clic en **Perfiles** en **Administrar usuarios**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Haga clic en el perfil del usuario de sincronización.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. En la sección Seguridad **a nivel de** campo, haga clic en **Vista** junto al objeto que contiene el campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Haga clic en **Editar**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Marque la casilla **Visible** para el campo que desee agregar a la sincronización y haga clic en **Guardar**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   ¡Dulce! En el próximo ciclo de sincronización, Marketo verá el campo y inicio la magia.

   >[!NOTE]
   >
   > Si el campo ya tiene valores en Salesforce, esos valores no se sincronizan con Marketing hasta la siguiente actualización del registro.

